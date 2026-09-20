# Lesson 28 --- Application Scalability and Autoscaling

## Horizontal scaling

Add more instances.

## Vertical scaling

Give an instance more resources.

## Scaling signals

CPU alone is often insufficient. Consider: - Requests/sec - Concurrent
requests - Queue depth - Queue age - Latency - Custom business load

## Little's Law

``` text
L = λW
```

Concurrency is related to throughput and response time.

## Important warning

Autoscaling can overload downstream systems. Bound scaling with database
and provider capacity.
