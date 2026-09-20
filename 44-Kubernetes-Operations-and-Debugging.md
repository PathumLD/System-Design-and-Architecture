# Lesson 44 --- Kubernetes Operations and Debugging

## Debug flow

``` text
External request
 ↓
Gateway
 ↓
Service
 ↓
Pod
 ↓
Application
 ↓
Database
```

## Useful commands

``` text
kubectl get
kubectl describe
kubectl logs
kubectl events
kubectl exec
kubectl top
kubectl rollout
```

## Common states

-   CrashLoopBackOff
-   ImagePullBackOff
-   Pending
-   OOMKilled
-   Running but not Ready

## Principle

Running does not mean healthy. Readiness determines whether traffic
should reach the workload.
