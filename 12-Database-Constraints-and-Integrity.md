# Lesson 12 --- Constraints, Keys and Integrity

## Database guarantees

-   PRIMARY KEY
-   FOREIGN KEY
-   UNIQUE
-   CHECK
-   NOT NULL
-   Appropriate cascade behavior

## Multi-tenant uniqueness

A value may be unique within a tenant rather than globally.

``` text
UNIQUE(tenant_id, email)
```

Composite foreign keys can enforce tenant-safe relationships.

## Important principle

Application validation improves user experience; database constraints
provide the final integrity boundary.
