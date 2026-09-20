# Lesson 65 --- Production Architecture Review and ADRs

## Architecture is a set of decisions

A diagram alone does not explain: - why components exist - who owns
data - how failures behave - what constraints were accepted - what
trade-offs were chosen

## ADR

Architecture Decision Record:

``` text
Context
Decision
Alternatives
Consequences
Status
```

Use ADRs for important, expensive, cross-cutting, security, data,
scaling, or infrastructure decisions.

## Production review checklist

### Correctness

-   Are business invariants protected?
-   Are concurrency races handled?

### Data ownership

-   Does every domain/module own its data?
-   Are cross-module writes prohibited?

### Transactions

-   What must be atomic?
-   Are external calls kept outside database transactions?

### Failure

-   What happens when PostgreSQL fails?
-   Redis?
-   Service Bus?
-   External payment provider?
-   Workers?

### Messaging

-   Is delivery at least once?
-   Are consumers idempotent?
-   Is there an Inbox?
-   Is there an Outbox?
-   Is there a DLQ?

### Scaling

-   What is the bottleneck?
-   What happens to DB connections when replicas increase?
-   Are downstream quotas respected?

### Security

-   Authentication
-   Authorization
-   Tenant isolation
-   Least privilege
-   Secrets
-   TLS
-   Audit

### Deployment

-   Backward-compatible schemas
-   Expand/migrate/contract
-   Immutable image digests
-   Canary/blue-green/rolling strategy
-   Rollback vs roll-forward

### Observability

-   Logs
-   Metrics
-   Traces
-   Business SLIs
-   Alerts
-   Queue age
-   Database health

### DR

-   RTO
-   RPO
-   Backup
-   PITR
-   Restore testing
-   Region recovery

### Cost

-   Compute
-   Database
-   Cache
-   Messaging
-   Storage
-   Monitoring
-   Network
-   Backups

## Risk register

Track risks with probability, impact, and mitigation rather than
pretending every risk can be eliminated.

## Architect principle

Do not call an architecture "future-proof." Say it is appropriate for
current requirements and has defined evolution paths.
