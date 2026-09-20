# Lesson 63 --- Multi-Tenant SaaS Architecture

## Tenant model

A tenant is a business/organization. A user can belong to one or more
tenants through memberships.

## Isolation models

1.  Shared DB / shared schema + `tenant_id`
2.  Shared DB / separate schemas
3.  Database per tenant
4.  Hybrid

## Recommended starting model

Shared PostgreSQL database/schema with strong tenant-aware design: -
`tenant_id` - composite uniqueness - composite foreign keys where
appropriate - tenant-aware indexes - application tenant context -
optional PostgreSQL RLS as defense in depth

## Tenant resolution

Possible sources: - subdomain - authenticated membership - route -
controlled application context

Never blindly trust a client-supplied tenant ID.

## Tenant context

``` csharp
public interface ICurrentTenant
{
    Guid TenantId { get; }
}
```

## Tenant boundary everywhere

Tenant context must be considered in: - SQL - EF Core filters - Redis
keys - Blob object paths - Service Bus messages - background jobs -
logs - audit records

## Control plane vs data plane

Control plane manages: - tenant registry - plans - lifecycle -
provisioning - quotas

Data plane executes tenant business operations.

## Noisy neighbors

Use: - rate limits - quotas - concurrency limits - queue fairness -
per-tenant usage controls

## Evolution

A tenant can later migrate from shared storage to a dedicated database.
A tenant resolver can route requests to the appropriate storage
location.

## Security

Platform admin/support access should be explicitly scoped and audited.
Impersonation should be deliberate and logged.
