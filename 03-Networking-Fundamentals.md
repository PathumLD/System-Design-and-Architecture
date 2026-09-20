# Lesson 03 --- Networking Fundamentals

## Core concepts

-   LAN and WAN
-   Private and public IP addresses
-   CIDR and subnets
-   Default gateway
-   NAT
-   TCP and UDP
-   Ports
-   Firewalls
-   Network Security Groups

## Example

``` text
Internet
   ↓
Public IP
   ↓
Firewall / Load Balancer
   ↓
Private subnet
   ↓
Application
   ↓
Private database subnet
```

## Cloud mapping

Azure uses VNets, subnets, NSGs, route tables, NAT, Private Link, and
private DNS to build controlled network boundaries.

## Architect question

For every connection ask: who can reach whom, on which port, using which
identity, and through which network boundary?
