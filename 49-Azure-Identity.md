# Lesson 49 --- Azure Identity

## Entra concepts

-   User
-   Group
-   Application registration
-   Service principal
-   Managed identity

## RBAC

``` text
Principal + Role + Scope
```

## Managed identity

Prefer workload identity over storing cloud credentials.

## Separate identities

Use different identities for: - API - Worker - Migration - CI/CD

## CI/CD

OIDC federation can provide short-lived cloud access without long-lived
deployment secrets.
