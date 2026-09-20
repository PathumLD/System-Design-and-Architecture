# Lesson 24 --- Event-Driven Architecture and Messaging

## Commands vs events

Command: \> Do this.

Event: \> This happened.

Commands express intent; events express facts.

## Event types

-   Domain events
-   Integration events

## Reliability

Use Outbox for reliable publication and Inbox/idempotency for reliable
consumption.

## Ordering

Prefer ordering within a business entity/aggregate rather than assuming
global ordering.

## Saga

A Saga coordinates multiple local transactions when one database
transaction cannot cover the whole workflow.

## Choreography vs orchestration

Choreography is decentralized; orchestration makes the workflow state
explicit.

## Event sourcing

Event-driven architecture, Outbox, CQRS, Saga, and event sourcing are
separate concepts and should not be conflated.
