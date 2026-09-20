# Lesson 40 --- CI/CD

## Pipeline principle

Build once, then promote the same immutable artifact.

``` text
Git
 ↓
Build
 ↓
Test
 ↓
Image
 ↓
Scan
 ↓
Registry
 ↓
Staging
 ↓
Smoke tests
 ↓
Production
```

## Database migrations

Treat migrations as an explicit deployment concern, not an
application-startup side effect.

## Safe schema changes

Use expand → migrate → contract.

## Deployment strategies

-   Rolling
-   Blue/green
-   Canary

## Supply chain

Use OIDC federation, image digests, SBOMs, scanning, signing, and
least-privileged deployment identities.
