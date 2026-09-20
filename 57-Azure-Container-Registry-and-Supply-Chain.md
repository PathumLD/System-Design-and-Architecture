# Lesson 57 --- Azure Container Registry and Supply Chain Security

## Registry

ACR stores OCI container images.

## Tags vs digests

Tags can move. Digests identify exact immutable content.

Use:

``` text
production → exact image digest
```

## Pipeline controls

-   Build once
-   SBOM
-   Vulnerability scanning
-   Image signing
-   Least-privileged registry access
-   OIDC
-   Retention policies

## Rollback

Rollback should reference a known-good immutable digest.
