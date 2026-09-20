# Lesson 19 --- Authentication and Authorization

## Authentication

Establishes identity.

## Authorization

Determines permissions.

## Models

-   Cookies
-   JWT
-   OAuth 2.0
-   OpenID Connect
-   PKCE
-   MFA
-   Passkeys
-   Entra ID

## Authorization layers

``` text
Identity
  ↓
Tenant membership
  ↓
Permission
  ↓
Resource ownership
```

## Security principle

A valid token does not automatically grant access to every resource
represented by an ID in the URL.
