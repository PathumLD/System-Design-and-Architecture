# Lesson 04 --- Servers, Processes, Threads and Async

## Concepts

-   A server is a machine or managed compute environment.
-   A process is an isolated running program instance.
-   Threads execute work within a process.
-   Async I/O allows a server to handle many waiting operations
    efficiently.
-   Kestrel hosts ASP.NET Core.
-   Reverse proxies such as Nginx can sit in front of Kestrel.

## Deployment spectrum

``` text
IaaS VM → Containers → PaaS → Serverless
```

## Scaling

Stateless application instances can normally be replicated horizontally.
Shared state should live in external systems such as PostgreSQL, Redis,
object storage, or a durable broker.
