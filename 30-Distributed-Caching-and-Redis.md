# Lesson 30 --- Distributed Caching and Redis

## PostgreSQL remains authoritative

Redis is useful for: - Hot reads - Sessions where appropriate - Rate
limiting - Permission caches - Short-lived coordination state

## Key design

Include tenant and object identity in keys when required.

``` text
tenant:{tenantId}:service:{serviceId}
```

## Stampede protection

Use TTL jitter, request coalescing, locks, or other controlled
strategies.

## Failure

Redis should have a deliberately defined outage behavior. A cache outage
must not automatically cause a database outage.
