# Lesson 45 --- Kubernetes Security

## Identity

Separate human identities from workload identities.

## Controls

-   RBAC
-   Least privilege
-   Service accounts
-   Workload identity
-   Pod security
-   Non-root
-   No privilege escalation
-   Drop capabilities
-   Read-only filesystem where possible
-   NetworkPolicy
-   Resource limits
-   Image scanning/signing
-   Admission controls

## Azure

AKS Workload Identity allows pods to access Azure resources using
federated workload identity rather than embedded credentials.

## Namespace warning

Namespaces provide organization/isolation boundaries but are not
equivalent to separate virtual machines.
