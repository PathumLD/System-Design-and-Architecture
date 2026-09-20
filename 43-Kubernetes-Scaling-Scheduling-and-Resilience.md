# Lesson 43 --- Kubernetes Scaling, Scheduling and Resilience

## Scaling

-   HPA
-   VPA
-   Cluster/node autoscaling
-   Custom metrics
-   Queue-driven scaling

## Scheduling

-   Affinity
-   Anti-affinity
-   Topology spread
-   Taints/tolerations

## Availability

-   PodDisruptionBudget
-   Rolling updates
-   Zone distribution

## Key warning

Scaling must respect downstream limits such as database connections and
third-party API quotas.
