# Lesson 47 --- Azure Architecture Fundamentals

## Resource hierarchy

``` text
Microsoft Entra tenant
  ↓
Management Groups
  ↓
Subscriptions
  ↓
Resource Groups
  ↓
Resources
```

## Key services

-   Azure Container Apps
-   Azure Kubernetes Service
-   App Service
-   Virtual Machines
-   Azure Database for PostgreSQL Flexible Server
-   Azure Managed Redis
-   Blob Storage
-   Service Bus
-   Key Vault
-   Container Registry
-   Front Door
-   Application Gateway
-   Azure Monitor

## Baseline

``` text
Front Door + WAF
        ↓
Container Apps
        ↓
PostgreSQL + Redis + Blob + Service Bus
```

Use the least operationally complex compute that satisfies the
requirements.
