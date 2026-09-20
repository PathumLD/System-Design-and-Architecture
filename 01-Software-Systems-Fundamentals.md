# Lesson 01 --- Software Systems Fundamentals

## Core idea

A software system is more than application code. It is the combination
of application logic, data, infrastructure, communication, security, and
operations.

## System model

``` text
User
  ↓
Client / Browser
  ↓
Network / DNS / HTTP / TLS
  ↓
Application Server
  ↓
Database / Cache / External Services
  ↓
Infrastructure / Monitoring / Security
```

## Key concepts

-   Functional requirements describe what the system does.
-   Non-functional requirements describe qualities such as availability,
    latency, scalability, security, and durability.
-   Architecture describes major structures and boundaries.
-   System design turns requirements into components, interactions, data
    ownership, and operational decisions.
-   Cloud architecture adds managed infrastructure, regions,
    availability zones, identity, networking, and operational services.

## Architect mindset

Start with requirements and constraints rather than technology names.
Every major component should have a reason to exist.

## Practical baseline

For this course, the primary implementation stack is ASP.NET Core +
PostgreSQL, with Azure as the main cloud and AWS/GCP as comparison
platforms.
