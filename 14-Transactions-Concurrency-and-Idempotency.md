# Lesson 14 --- Transactions, Concurrency and Idempotency

## ACID

-   Atomicity
-   Consistency
-   Isolation
-   Durability

## MVCC

PostgreSQL uses multi-version concurrency control to support concurrent
transactions.

## Concurrency strategies

-   Optimistic concurrency
-   Pessimistic locking
-   Unique/exclusion constraints
-   Appropriate transaction isolation

## Idempotency

Repeating the same logical operation should not create unintended
duplicate effects.

Use idempotency keys for operations such as payment or booking creation
where clients may retry.

## External side effects

Database transactions do not automatically include external APIs. Use
patterns such as Outbox and Saga when cross-system reliability is
required.
