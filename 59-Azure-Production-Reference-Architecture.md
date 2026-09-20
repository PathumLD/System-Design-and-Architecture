# Lesson 59 --- Azure Production Reference Architecture

## Reference

``` text
Internet
  ↓
Azure Front Door Premium + WAF
  ↓
Private Link
  ↓
Container Apps Environment
  ├── API
  ├── Workers
  └── Jobs
  ↓
Private data services
  ├── PostgreSQL Flexible Server
  ├── Azure Managed Redis
  ├── Blob Storage
  └── Service Bus
```

## Platform

``` text
ACR
Key Vault
Managed Identity
OpenTelemetry
Azure Monitor
GitHub Actions + OIDC
Bicep
```

## Principles

-   PostgreSQL is authoritative.
-   Redis is a cache.
-   Blob stores file bytes.
-   Service Bus carries durable asynchronous work.
-   API and workers scale independently.
-   Keep the public surface small.
-   Use zone HA before adding multi-region complexity unless
    requirements demand otherwise.
