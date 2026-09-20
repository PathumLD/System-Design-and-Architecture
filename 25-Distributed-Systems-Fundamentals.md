# Lesson 25 --- Distributed Systems Fundamentals

## Core difficulty

Independent processes communicate over networks that can fail partially.

## Failure modes

-   Timeout
-   Lost response
-   Duplicate request
-   Partial completion
-   Network partition
-   Replica lag
-   Leader failure
-   Unknown external outcome

## Key tools

-   Timeouts
-   Backoff + jitter
-   Idempotency
-   Quorum awareness
-   Fencing
-   Circuit breakers
-   Bulkheads
-   Tracing

## CAP/PACELC

Distributed systems force trade-offs involving consistency,
availability, partition tolerance, latency, and operational behavior.

## Important principle

A timeout does not prove that the remote operation failed.
