# Lesson 61 --- Domain-Driven Design in Depth

## Strategic DDD

-   Subdomains
-   Core / Supporting / Generic
-   Bounded contexts
-   Ubiquitous language
-   Context maps

A bounded context is a boundary around a model and language. It is not
automatically a microservice or a database.

## Tactical DDD

-   Entity
-   Value Object
-   Aggregate
-   Aggregate Root
-   Invariant
-   Domain Service
-   Repository
-   Domain Event

## Aggregate

An aggregate is a consistency and transaction boundary. Keep it small.

Do not create a giant `Tenant` or `Salon` aggregate containing
everything.

## Modular monolith

Possible PostgreSQL schema organization:

``` text
identity.*
catalog.*
scheduling.*
booking.*
billing.*
notifications.*
```

Modules should not directly update another module's tables. Use explicit
contracts/events.

## External systems

Use an Anti-Corruption Layer when an external model should not leak into
your domain.

## Historical truth

Store snapshots such as price/name when historical documents must remain
correct after catalog changes.
