# Lesson 09 --- Monolith, Modular Monolith and Microservices

## Options

-   Traditional monolith: one deployable unit with weak or strong
    internal boundaries.
-   Modular monolith: one deployable unit with explicit business
    modules.
-   Microservices: independently deployable services with distributed
    communication and data ownership.

## Common failure

A distributed monolith creates network boundaries without gaining real
independence.

## Recommended default

For many small and medium SaaS products, start with a modular monolith
and extract services only when a measured requirement justifies it.

## Extraction

The Strangler approach allows gradual extraction when a module genuinely
needs independent scaling, deployment, or isolation.
