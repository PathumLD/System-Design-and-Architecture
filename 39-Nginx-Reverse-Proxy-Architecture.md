# Lesson 39 --- Nginx and Reverse Proxies

## Role

Nginx can terminate TLS, route requests, serve static assets, enforce
limits, and proxy traffic to Kestrel.

``` text
Internet
  ↓
Nginx
  ↓
Kestrel
```

## Important settings

-   Forwarded headers
-   Timeouts
-   Upload limits
-   WebSockets
-   Upstream health
-   TLS
-   Connection limits

## Cloud mapping

Managed Azure load balancers/gateways often replace some Nginx
responsibilities, but the underlying proxy concepts remain important.
