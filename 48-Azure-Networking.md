# Lesson 48 --- Azure Networking

## Components

-   VNet
-   Subnet
-   NSG
-   Route table
-   NAT Gateway
-   Private Endpoint
-   Private DNS
-   VNet integration
-   VNet peering
-   VPN
-   ExpressRoute

## Important distinction

Outbound VNet integration and inbound private access are different
concepts.

## Architecture

``` text
Internet
   ↓
Front Door
   ↓
Private application origin
   ↓
Private database
```

## Design goal

Keep data services private and explicitly control outbound internet
access.
