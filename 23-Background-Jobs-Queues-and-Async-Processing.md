# Lesson 23 --- Background Jobs, Queues and Async Processing

## Why queues?

Queues decouple producers and consumers, absorb bursts, and move slow
work away from request paths.

## Delivery

Most practical systems should assume at-least-once delivery.

Therefore consumers need: - Idempotency - Retry handling - Dead-letter
queues - Poison-message handling

## Options

-   Hangfire
-   RabbitMQ
-   Azure Service Bus
-   AWS SQS
-   PostgreSQL `SKIP LOCKED` job queues

## Decision

Use the simplest durable mechanism that satisfies the requirement.
