# Lesson 13 --- Indexes and Query Performance

## Index concepts

-   B-tree
-   Composite indexes
-   Partial indexes
-   Expression indexes
-   INCLUDE columns
-   Query plans

## Diagnostics

Use `EXPLAIN` / `EXPLAIN ANALYZE` and database statistics to identify
real bottlenecks.

## Common problems

-   N+1 queries
-   Missing indexes
-   Over-indexing writes
-   Offset pagination on large datasets
-   Poor query selectivity

## Keyset pagination

For large ordered datasets, use a stable cursor/key rather than
repeatedly scanning skipped rows.

## Rule

Index for real query patterns, then measure.
