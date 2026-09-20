# System Design & Software Architecture Course

This package contains one Markdown file per chapter/lesson from the
system-design course covered in the conversation.

> **Content note:** These files are structured course notes
> reconstructed from the lesson content available in the conversation
> context. They are not claimed to be verbatim transcripts of every
> earlier assistant message.

## Course map

1.  [Software Systems
    Fundamentals](./01-Software-Systems-Fundamentals.md)
2.  [Web Request Flow](./02-Web-Request-Flow.md)
3.  [Networking Fundamentals](./03-Networking-Fundamentals.md)
4.  [Servers Processes Threads and
    Async](./04-Servers-Processes-Threads-and-Async.md)
5.  [Application Architecture](./05-Application-Architecture.md)
6.  [Layered Architecture and Domain
    Invariants](./06-Layered-Architecture-and-Domain-Invariants.md)
7.  [Clean Onion and Hexagonal
    Architecture](./07-Clean-Onion-and-Hexagonal-Architecture.md)
8.  [Vertical Slice Architecture and
    CQRS](./08-Vertical-Slice-Architecture-and-CQRS.md)
9.  [Monolith Modular Monolith and
    Microservices](./09-Monolith-Modular-Monolith-and-Microservices.md)
10. [Database Design Fundamentals](./10-Database-Design-Fundamentals.md)
11. [Database Normalization](./11-Database-Normalization.md)
12. [Database Constraints and
    Integrity](./12-Database-Constraints-and-Integrity.md)
13. [Indexes and Query
    Performance](./13-Indexes-and-Query-Performance.md)
14. [Transactions Concurrency and
    Idempotency](./14-Transactions-Concurrency-and-Idempotency.md)
15. [SQL vs NoSQL](./15-SQL-vs-NoSQL.md)
16. [Database Connections and
    Pooling](./16-Database-Connections-and-Pooling.md)
17. [Database Scaling and High
    Availability](./17-Database-Scaling-and-High-Availability.md)
18. [REST API Design](./18-REST-API-Design.md)
19. [Authentication and
    Authorization](./19-Authentication-and-Authorization.md)
20. [Practical ASP.NET Authentication
    Architecture](./20-Practical-ASP-NET-Authentication-Architecture.md)
21. [Authorization Architecture](./21-Authorization-Architecture.md)
22. [Caching Fundamentals](./22-Caching-Fundamentals.md)
23. [Background Jobs Queues and Async
    Processing](./23-Background-Jobs-Queues-and-Async-Processing.md)
24. [Event Driven Architecture and
    Messaging](./24-Event-Driven-Architecture-and-Messaging.md)
25. [Distributed Systems
    Fundamentals](./25-Distributed-Systems-Fundamentals.md)
26. [Resilience Patterns](./26-Resilience-Patterns.md)
27. [Load Balancers Reverse Proxies and
    Gateways](./27-Load-Balancers-Reverse-Proxies-and-Gateways.md)
28. [Application Scalability and
    Autoscaling](./28-Application-Scalability-and-Autoscaling.md)
29. [Data Partitioning and
    Sharding](./29-Data-Partitioning-and-Sharding.md)
30. [Distributed Caching and
    Redis](./30-Distributed-Caching-and-Redis.md)
31. [Object Storage and CDN File
    Delivery](./31-Object-Storage-and-CDN-File-Delivery.md)
32. [CDN Edge and Global Traffic](./32-CDN-Edge-and-Global-Traffic.md)
33. [Multi Region Data DR and Business
    Continuity](./33-Multi-Region-Data-DR-and-Business-Continuity.md)
34. [Observability Logs Metrics and
    Traces](./34-Observability-Logs-Metrics-and-Traces.md)
35. [Performance Engineering and Load
    Testing](./35-Performance-Engineering-and-Load-Testing.md)
36. [Security Architecture](./36-Security-Architecture.md)
37. [Secrets Encryption PKI and Key
    Management](./37-Secrets-Encryption-PKI-and-Key-Management.md)
38. [Docker Fundamentals](./38-Docker-Fundamentals.md)
39. [Nginx Reverse Proxy
    Architecture](./39-Nginx-Reverse-Proxy-Architecture.md)
40. [CI CD and Safe Deployments](./40-CI-CD-and-Safe-Deployments.md)
41. [Kubernetes Fundamentals](./41-Kubernetes-Fundamentals.md)
42. [Kubernetes Networking and
    Storage](./42-Kubernetes-Networking-and-Storage.md)
43. [Kubernetes Scaling Scheduling and
    Resilience](./43-Kubernetes-Scaling-Scheduling-and-Resilience.md)
44. [Kubernetes Operations and
    Debugging](./44-Kubernetes-Operations-and-Debugging.md)
45. [Kubernetes Security](./45-Kubernetes-Security.md)
46. [Stateful Workloads and
    StatefulSets](./46-Stateful-Workloads-and-StatefulSets.md)
47. [Azure Architecture
    Fundamentals](./47-Azure-Architecture-Fundamentals.md)
48. [Azure Networking](./48-Azure-Networking.md)
49. [Azure Identity](./49-Azure-Identity.md)
50. [Azure Compute](./50-Azure-Compute.md)
51. [Azure PostgreSQL
    Architecture](./51-Azure-PostgreSQL-Architecture.md)
52. [Azure Blob Storage](./52-Azure-Blob-Storage.md)
53. [Azure Service Bus](./53-Azure-Service-Bus.md)
54. [Azure Managed Redis](./54-Azure-Managed-Redis.md)
55. [Azure Front Door Application Gateway and
    WAF](./55-Azure-Front-Door-Application-Gateway-and-WAF.md)
56. [Azure Monitor Application Insights and
    OpenTelemetry](./56-Azure-Monitor-Application-Insights-and-OpenTelemetry.md)
57. [Azure Container Registry and Supply
    Chain](./57-Azure-Container-Registry-and-Supply-Chain.md)
58. [Azure CI CD Bicep and IaC](./58-Azure-CI-CD-Bicep-and-IaC.md)
59. [Azure Production Reference
    Architecture](./59-Azure-Production-Reference-Architecture.md)
60. [AWS and GCP Architecture
    Mapping](./60-AWS-and-GCP-Architecture-Mapping.md)
61. [Domain Driven Design in
    Depth](./61-Domain-Driven-Design-in-Depth.md)
62. [CQRS Sagas Outbox Inbox and Event Driven
    Workflows](./62-CQRS-Sagas-Outbox-Inbox-and-Event-Driven-Workflows.md)
63. [Multi Tenant SaaS
    Architecture](./63-Multi-Tenant-SaaS-Architecture.md)
64. [System Design Interview
    Framework](./64-System-Design-Interview-Framework.md)
65. [Production Architecture Review and
    ADRs](./65-Production-Architecture-Review-and-ADRs.md)

## Primary stack

-   ASP.NET Core
-   PostgreSQL
-   Azure
-   Docker
-   Kubernetes concepts
-   Redis / Azure Managed Redis
-   Azure Service Bus
-   Blob Storage
-   OpenTelemetry
-   CI/CD and Infrastructure as Code

## Core architectural progression

Requirements → Domain → Data → APIs → Transactions → Messaging → Scaling
→ Security → Cloud → Operations → Production architecture.
