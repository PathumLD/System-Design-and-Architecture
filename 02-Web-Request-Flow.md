# Lesson 02 --- How a Web Request Travels

## Request path

``` text
Browser
  ↓
DNS
  ↓
IP address
  ↓
Firewall / Edge
  ↓
Reverse Proxy / Load Balancer
  ↓
Kestrel / ASP.NET Core
  ↓
Application
  ↓
PostgreSQL / External APIs
```

## Important concepts

-   DNS resolves names to IP addresses.
-   HTTP provides the request/response protocol.
-   TLS protects traffic in transit.
-   Cookies and tokens carry client authentication state.
-   Kestrel is the ASP.NET Core web server.
-   Middleware processes requests in a defined pipeline.
-   Stateless APIs allow horizontal scaling more easily.

## Key lesson

A request crosses multiple failure and trust boundaries. Production
architecture must account for each one.
