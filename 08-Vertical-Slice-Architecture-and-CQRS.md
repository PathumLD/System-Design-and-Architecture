# Lesson 08 --- Vertical Slice Architecture and CQRS

## Vertical Slice

Organize code around business capabilities/use cases rather than only
technical layers.

Example:

``` text
Booking/
  CreateBooking/
  CancelBooking/
  ConfirmBooking/
```

## CQRS

Command = changes state. Query = reads state.

The read model can be optimized independently from the write model.

## Important rule

CQRS does not require separate databases, microservices, or event
sourcing. A single PostgreSQL database can support CQRS very
effectively.
