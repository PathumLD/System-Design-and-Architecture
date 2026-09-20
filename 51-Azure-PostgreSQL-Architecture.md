# Lesson 51 --- Azure PostgreSQL

## Consider

-   Compute tier
-   Storage
-   IOPS
-   HA
-   Backups
-   PITR
-   Read replicas
-   Connection pooling
-   Private access
-   Entra authentication

## HA vs backup

Zone-redundant HA reduces service interruption. It does not replace
backup/PITR.

## Connection budget

Application replicas, workers, migrations, and administrative tooling
all consume database connections.
