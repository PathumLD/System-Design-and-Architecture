# Lesson 06 --- Layered Architecture and Domain Invariants

## Layers

-   Presentation handles HTTP concerns.
-   Application coordinates use cases.
-   Domain owns business rules.
-   Infrastructure handles databases, messaging, external systems, and
    technical adapters.

## Domain invariant

An invariant is a rule that must remain true.

Example: \> A confirmed booking must not overlap another confirmed
booking for the same staff member.

## Transaction principle

Keep related state changes inside the smallest transaction that truly
needs atomicity.

## Authorization

Authentication answers "who are you?" Authorization answers "what may
you do?" Resource authorization answers "may you perform this action on
this particular resource?"
