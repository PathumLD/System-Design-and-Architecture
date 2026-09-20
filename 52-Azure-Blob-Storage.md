# Lesson 52 --- Azure Blob Storage

## Model

``` text
Storage Account
  ↓
Container
  ↓
Blob
```

## Architecture

Keep metadata in PostgreSQL and bytes in Blob Storage.

## Secure uploads

Generate server-controlled object keys and use short-lived user
delegation SAS URLs.

## Lifecycle

Hot → Cool → Cold → Archive can reduce cost for data with changing
access patterns.

## Durability controls

Use appropriate redundancy, soft delete, versioning, retention, and
recovery features based on requirements.
