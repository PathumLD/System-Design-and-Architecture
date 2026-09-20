# Lesson 29 --- Data Partitioning and Sharding

## Partitioning

Split data within a database according to a key such as date or tenant.

## Sharding

Distribute data across separate database instances.

## Strategies

-   Range
-   Hash
-   List
-   Directory-based routing
-   Consistent hashing

## SaaS

Tenant-aware routing can support gradual migration from shared storage
to dedicated databases.

## Costs

Sharding introduces: - Cross-shard queries - Routing - Resharding -
Per-shard backups/HA - More operational complexity

Diagnose the bottleneck before sharding.
