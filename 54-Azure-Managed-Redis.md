# Lesson 54 --- Azure Managed Redis

## Role

Redis is a low-latency distributed cache/state system, not the
authoritative business database.

## Design

-   TTL
-   Eviction policy
-   Key namespaces
-   Invalidation
-   Stampede protection
-   Hot-key management
-   Memory budgeting

## Security

Use private connectivity, TLS, and identity/access controls where
supported.

## Failure

Define explicit fallback behavior before depending on Redis for
production traffic.
