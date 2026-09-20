# Lesson 34 --- Observability

## Three pillars

``` text
Logs
Metrics
Traces
```

## Useful metrics

RED: - Rate - Errors - Duration

USE: - Utilization - Saturation - Errors

## SaaS-specific telemetry

Track: - Tenant - Trace ID - Correlation ID - Business operation - Queue
age - Booking success - Payment outcomes

Avoid high-cardinality dimensions that explode telemetry cost.

## OpenTelemetry

Use OpenTelemetry for portable instrumentation across services and cloud
platforms.
