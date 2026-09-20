# Lesson 46 --- Stateful Workloads

## Deployment vs StatefulSet

Deployments suit interchangeable stateless replicas.

StatefulSets provide: - Stable identities - Stable network names -
Persistent volume association - Ordered lifecycle behavior

## Critical warning

A StatefulSet does not automatically make PostgreSQL highly available.

For databases, consider: - Managed PostgreSQL - Replication - Failover -
Fencing - Backups - PITR - Operators when self-hosting is justified

## Principle

Use stateful orchestration only when the workload requires it.
