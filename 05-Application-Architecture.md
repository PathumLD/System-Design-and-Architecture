# Lesson 05 --- Application Architecture

## Principles

-   Separation of concerns
-   Single responsibility
-   High cohesion
-   Low coupling
-   Dependency injection
-   Dependency inversion
-   Explicit boundaries

## Typical layers

``` text
Presentation
    ↓
Application
    ↓
Domain
    ↓
Infrastructure
```

## Better modular organization

Feature or business boundaries often scale better than a huge technical
folder structure.

## Important distinction

DTOs represent contracts. Domain objects represent business behavior and
invariants. Infrastructure implements technical concerns.
