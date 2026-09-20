# Lesson 11 --- Normalization

## Goals

Normalization reduces update anomalies and unnecessary duplication.

### 1NF

Atomic values and consistent row structure.

### 2NF

No partial dependency on part of a composite key.

### 3NF

Non-key attributes should depend on the key rather than another non-key
attribute.

## Denormalization

Denormalization is intentional duplication for a measured
read/performance requirement. Read models and snapshots are valid
architectural tools when their purpose is explicit.

## Snapshot example

Historical invoice data may store the service name and price at the time
of purchase instead of depending on today's catalog values.
