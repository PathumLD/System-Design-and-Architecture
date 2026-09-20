# Lesson 18 --- REST API Design

## Principles

-   Resource-oriented URLs
-   Appropriate HTTP methods
-   Meaningful status codes
-   DTOs instead of leaking persistence models
-   Consistent error responses
-   Validation
-   Idempotency where needed
-   Pagination
-   Versioning strategy
-   OpenAPI documentation

## Example

``` http
POST /bookings
GET /bookings/{id}
POST /bookings/{id}/cancel
```

## Long-running work

Return `202 Accepted` when work is intentionally asynchronous and
provide a way to observe status.

## Errors

Use a consistent machine-readable problem format rather than exposing
stack traces or internal database details.
