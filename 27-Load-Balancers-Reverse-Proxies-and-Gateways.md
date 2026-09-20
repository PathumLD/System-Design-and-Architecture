# Lesson 27 --- Load Balancers, Reverse Proxies and API Gateways

## Traffic path

``` text
DNS / Edge
  ↓
Reverse Proxy / Load Balancer
  ↓
Application
  ↓
Database
```

## L4 vs L7

-   L4 routes network connections.
-   L7 understands application protocols such as HTTP.

## Responsibilities

-   TLS termination
-   Routing
-   Health checks
-   Connection draining
-   Rate limiting
-   Header forwarding
-   WebSocket support
-   Gateway policies

## Scaling warning

Sticky sessions can hide statefulness. Prefer stateless applications
with externalized shared state where practical.
