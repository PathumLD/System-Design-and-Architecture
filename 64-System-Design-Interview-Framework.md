# Lesson 64 --- System Design Interview Framework

## Master sequence

``` text
Requirements
  ↓
Constraints
  ↓
Capacity
  ↓
APIs
  ↓
Data model
  ↓
High-level architecture
  ↓
Deep dive
  ↓
Scaling
  ↓
Reliability
  ↓
Security
  ↓
Trade-offs
```

## 1. Clarify requirements

Identify: - users - functional requirements - non-functional
requirements - scale - availability - latency - geography - consistency

## 2. Identify invariants

Ask: \> What must never happen?

For booking: \> Two confirmed bookings must not overlap the same
protected resource/time.

## 3. Estimate capacity

Use rough order-of-magnitude calculations.

``` text
RPS ≈ requests/day ÷ 86,400
Peak RPS ≈ average RPS × peak factor
```

Estimate storage and growth.

## 4. APIs

Define the major external contracts before discussing every
implementation detail.

## 5. Data model

Start from business entities and ownership.

## 6. High-level architecture

Start simple. Add complexity only when a requirement or bottleneck
justifies it.

## 7. Deep dive

Discuss: - consistency - concurrency - caching - queues - scaling -
failures - security

## 8. Trade-offs

Explain why a choice is appropriate and what it costs.

## Interview principle

Do not answer: \> "Which technology is best?"

Answer: \> "Which design satisfies these requirements with acceptable
complexity and trade-offs?"

## Useful interview language

-   "I'll clarify the requirements first."
-   "The key invariant is..."
-   "I'll estimate order-of-magnitude capacity."
-   "I'll start simple and evolve based on bottlenecks."
-   "This operation requires strong consistency."
-   "This side effect can be eventually consistent."
-   "The consumer must be idempotent because delivery is at least once."
