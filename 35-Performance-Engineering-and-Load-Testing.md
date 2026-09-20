# Lesson 35 --- Performance Engineering

## Performance loop

``` text
Measure
 ↓
Identify bottleneck
 ↓
Hypothesize
 ↓
Change
 ↓
Load test
 ↓
Compare
```

## Test types

-   Benchmark
-   Load
-   Stress
-   Spike
-   Soak

## Measure

-   p50
-   p95
-   p99
-   Throughput
-   Error rate
-   CPU/memory
-   DB latency
-   Pool wait
-   External dependency latency

## Common problems

N+1 queries, poor indexes, serialization overhead, database locks,
connection exhaustion, and slow external APIs.
