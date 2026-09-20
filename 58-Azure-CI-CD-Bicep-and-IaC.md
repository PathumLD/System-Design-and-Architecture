# Lesson 58 --- Azure CI/CD, Bicep and Infrastructure as Code

## Bicep

Bicep is Azure's declarative infrastructure language compiled to ARM
templates.

## Pipeline

``` text
Git
 ↓
Test
 ↓
Bicep lint
 ↓
What-If
 ↓
Infrastructure deployment
 ↓
Build image
 ↓
Scan/SBOM
 ↓
Deploy
```

## Important concepts

-   Modules
-   Parameters
-   Explicit/implicit dependencies
-   Incremental deployments
-   Deployment Stacks where appropriate
-   OIDC
-   Environment separation
-   Drift detection
-   Policy/cost controls

IaC describes infrastructure. It is not a replacement for backups.
