# Lesson 17 --- Database Scaling, HA and DR

## Scaling options

-   Vertical scaling
-   Read replicas
-   Partitioning
-   Sharding
-   Caching
-   Read models

## High availability

A primary plus standby can reduce downtime, but HA is not the same as
backup.

## Recovery

-   RTO: how quickly service should recover.
-   RPO: how much data loss is acceptable.

## Backups

Use backups, WAL/PITR where supported, retention, and regular restore
tests.

## Replica warning

A replica can faithfully replicate accidental deletion. It is not a
substitute for backups.
