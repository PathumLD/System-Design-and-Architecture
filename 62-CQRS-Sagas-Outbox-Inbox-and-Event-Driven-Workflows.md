# Lesson 62 --- CQRS, Sagas, Outbox, Inbox and Event-Driven Workflows

## Problem

A multi-step workflow may span multiple contexts and external systems:

``` text
Create Booking
 ↓
Reserve Slot
 ↓
Take Payment
 ↓
Generate Invoice
 ↓
Send Confirmation
```

There may be no single database transaction covering everything.

## CQRS

Separate command/write models from query/read models. A single database
is fine.

## Outbox

Write business state and an outbox message in the same local
transaction.

``` text
BEGIN
  Booking
  Outbox
COMMIT
```

The dispatcher later publishes the message.

## Inbox

Consumers store processed message IDs, typically with a unique
constraint:

``` text
UNIQUE(consumer_name, message_id)
```

## Exactly once

End-to-end exactly-once delivery is generally not a realistic
assumption. Aim for effectively-once business effects using idempotency.

## Saga

A Saga is a stateful workflow composed of local transactions and
compensating actions.

Example states:

``` text
Started
ReservingSlot
AwaitingPayment
CreatingInvoice
Completed
Compensating
Failed
PaymentUnknown
```

## Orchestration

For important payment workflows, explicit orchestration makes state,
timeout, recovery, and compensation visible.

## Compensation

Compensation is not database rollback.

Examples: - Payment fails → release slot. - Payment captured but
workflow fails → refund/void where appropriate. - Invoice exists →
accounting correction may require a credit note rather than deletion. -
Notification fails → retry/DLQ; do not undo the booking.

## Timeouts

Use durable timers, scheduled messages, or jobs. Do not rely on
`Task.Delay` for business workflow timers.

## Observability

Track: - trace ID - saga/correlation ID - causation ID - message ID -
tenant ID - event type/version - queue age - saga state age -
compensation failures

## Testing

Test duplicates, out-of-order messages, crashes after commit, provider
timeouts, payment unknown states, compensation failures, and projection
rebuilds.
