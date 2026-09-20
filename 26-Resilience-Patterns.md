# Lesson 26 --- Resilience Patterns

## Patterns

-   Timeout
-   Retry
-   Circuit breaker
-   Bulkhead
-   Rate limiting
-   Load shedding
-   Backpressure
-   Graceful degradation

## Retry rule

Retry only operations that are safe and failures that are plausibly
transient.

Use exponential backoff and jitter.

## Cascading failure

An overloaded dependency can cause upstream retries, which create more
load, which causes more failure.

## Payment example

A payment timeout may mean:

``` text
Unknown
```

not automatically:

``` text
Failed
```

Reconciliation may be required.
