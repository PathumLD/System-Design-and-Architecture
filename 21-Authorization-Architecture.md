# Lesson 21 --- Authorization Architecture

## RBAC

Roles group permissions.

## Resource authorization

A user may have a permission but still be unable to access a particular
resource.

## BOLA/IDOR

Never assume an object ID supplied by the client is authorized.

## SaaS roles

Keep platform, tenant, and support/admin privileges distinct.

## Entitlements

Permissions answer "may this identity perform this action?" Entitlements
answer "does this tenant's plan include this capability?"

## Caching

Authorization decisions can be cached carefully, but revocation and
staleness must be considered.
