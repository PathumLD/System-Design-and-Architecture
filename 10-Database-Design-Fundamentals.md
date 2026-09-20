# Lesson 10 --- Database Design Fundamentals

## Relational model

-   Tables represent structured data.
-   Primary keys identify rows.
-   Foreign keys represent relationships.
-   Cardinality describes one-to-one, one-to-many, and many-to-many
    relationships.
-   Junction tables model many-to-many relationships.

## SaaS example

``` text
Tenant
 ├── Staff
 ├── Services
 └── Bookings
```

## Multi-tenancy

Tenant identity is part of the data-isolation boundary. Design
tenant-aware keys, constraints, indexes, and authorization from the
beginning.
