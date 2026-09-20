# Lesson 20 --- Practical ASP.NET Authentication Architecture

## Core entities

``` text
Users
Tenants
Memberships
Roles
Permissions
Sessions
```

## Application abstractions

``` csharp
ICurrentUser
ICurrentTenant
```

Use request-scoped context rather than passing identity details through
every method manually.

## Token/session security

Refresh-token rotation, expiry, MFA, session revocation, secure cookie
configuration, and least privilege all matter.

## Production separation

Runtime identities and migration/deployment identities should have
different permissions.
