# Lesson 50 --- Azure Compute Choices

## Spectrum

``` text
App Service
   ↓
Container Apps
   ↓
AKS
   ↓
VMs
```

As you move toward VMs, you gain control but also gain operational
responsibility.

## Container Apps

Useful for: - HTTP services - Workers - Jobs - Revisions - Traffic
splitting - KEDA-based scaling

## AKS

Use when Kubernetes capabilities themselves are a requirement.

## Default for this course

Azure Container Apps is the preferred baseline for the SaaS unless
requirements justify AKS.
