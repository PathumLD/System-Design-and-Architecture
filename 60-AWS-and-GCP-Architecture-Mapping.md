# Lesson 60 --- AWS and GCP Architecture Mapping

## Capability mapping

  ---------------------------------------------------------------------------------
  Capability        Azure             AWS                GCP
  ----------------- ----------------- ------------------ --------------------------
  Containers        Container Apps    ECS/Fargate        Cloud Run

  Kubernetes        AKS               EKS                GKE

  VM                VM                EC2                Compute Engine

  PostgreSQL        Azure PostgreSQL  RDS/Aurora         Cloud SQL/AlloyDB
                                      awareness          awareness

  Redis             Azure Managed     ElastiCache        Memorystore
                    Redis                                

  Object storage    Blob              S3                 Cloud Storage

  Queue             Service Bus Queue SQS                Pub/Sub/Cloud Tasks
                                                         depending semantics

  Registry          ACR               ECR                Artifact Registry

  Secrets           Key Vault         Secrets            Secret Manager/KMS
                                      Manager/KMS        

  Global edge       Front Door        CloudFront + WAF   Global External
                                                         Application LB + CDN

  Network           VNet              VPC                VPC

  Identity          Managed Identity  IAM Role           Service Account

  Observability     Azure Monitor     CloudWatch/X-Ray   Cloud
                                                         Monitoring/Logging/Trace
  ---------------------------------------------------------------------------------

## Principle

Map capabilities, not product names. There is rarely a perfect
one-to-one match.

## Portability

Abstract application boundaries such as `IFileStorage` and
`IMessagePublisher`, but do not abstract every cloud detail just for
theoretical portability.
