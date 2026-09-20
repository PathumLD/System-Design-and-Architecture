# Lesson 33 --- Multi-Region Data, DR and Business Continuity

## HA vs DR

HA handles expected component failures. DR handles major outages and
recovery.

## DR levels

-   Cold
-   Warm
-   Hot

## Recovery requirements

Define RTO and RPO based on business impact.

## Data considerations

Asynchronous replication can lose recent writes during a regional
failure. Synchronous strategies reduce loss but increase latency and
coupling.

## DR dependencies

Don't forget: - Identity - DNS - Secrets - Images -
Infrastructure-as-code - Object storage - Messaging - Monitoring -
Backups

## Testing

A DR strategy is incomplete until restoration/failover is tested.
