# Lesson 07 --- Clean, Onion and Hexagonal Architecture

## Core idea

Business rules should not depend directly on frameworks, databases, or
external services.

``` text
Infrastructure
      ↓
Application
      ↓
Domain
```

## Ports and adapters

The application/domain defines what it needs; adapters implement those
needs.

Example:

``` csharp
public interface IClock
{
    DateTimeOffset UtcNow { get; }
}
```

## Modular monolith

A modular monolith can provide strong business boundaries without
immediately paying the operational cost of microservices.
