# Lesson 31 --- Object Storage and File Delivery

## Architecture

Keep file bytes in object storage and metadata in PostgreSQL.

``` text
DB
 └── object key / owner / status

Blob
 └── actual bytes
```

## Direct upload

Use server-generated object keys and short-lived signed URLs.

## File lifecycle

``` text
Pending → Uploaded → Scanning → Ready
```

## Security

-   Content validation
-   Malware scanning
-   Access control
-   Short-lived URLs
-   Encryption
-   Tenant isolation

## Large files

Use multipart/chunked upload and checksums when appropriate.
