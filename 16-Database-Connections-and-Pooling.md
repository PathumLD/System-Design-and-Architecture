# Lesson 16 --- Database Connections and Pooling

## Why pooling matters

Opening a database connection is expensive. Application frameworks
therefore reuse connections.

## Capacity problem

If each application replica can open many connections, horizontal
scaling can multiply database load.

``` text
10 replicas × 50 connections
= 500 possible connections
```

## Controls

-   Application pool limits
-   PostgreSQL limits
-   PgBouncer where appropriate
-   Separate budgets for API, workers, migrations, and administration

## Principle

Database connection capacity is part of application scaling design.
