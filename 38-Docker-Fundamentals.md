# Lesson 38 --- Docker Fundamentals

## Container model

A container packages an application and its dependencies into an
immutable image.

## ASP.NET image pattern

Use multi-stage builds:

``` text
SDK image
   ↓
build/publish
   ↓
small runtime image
```

## Production practices

-   Non-root user
-   Minimal base image
-   No secrets in image
-   Immutable tags/digests
-   Health checks
-   Graceful shutdown
-   Stdout/stderr logging
-   Ephemeral filesystem assumptions

## State

Persistent data belongs in managed databases/object storage/volumes as
appropriate, not inside disposable containers.
