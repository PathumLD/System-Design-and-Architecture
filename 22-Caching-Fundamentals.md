# Lesson 22 --- Caching Fundamentals

## Layers

-   In-memory cache
-   Distributed Redis cache
-   HTTP/browser cache
-   CDN

## Cache-aside

``` text
Read
 ↓
Cache?
 ├─ hit → return
 └─ miss → DB → cache → return
```

## Problems

-   Invalidation
-   Stampede
-   Hot keys
-   Negative caching
-   Stale permissions
-   Memory pressure

## Rule

The cache is normally an optimization. Keep an authoritative source of
truth.
