# Lesson 53 --- Azure Service Bus

## Messaging

-   Queue: one logical work stream
-   Topic: publish/subscribe
-   Subscription: independent consumer view

## Delivery

PeekLock supports processing before settlement.

## Reliability

Use: - Idempotency - Duplicate detection where useful - Dead-letter
queue - Retry - Sessions for ordered related messages where required

## Large payloads

Store large files in Blob Storage and send a secure/reference pointer
through the message.

## Identity

Prefer managed identity and least-privileged messaging roles.
