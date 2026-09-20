# Lesson 55 --- Azure Front Door, Application Gateway and WAF

## Front Door

Global Layer-7 edge routing and application acceleration.

## Application Gateway

Regional Layer-7 routing and WAF capabilities.

## Azure Load Balancer

Layer-4 load balancing.

## Typical global architecture

``` text
Internet
  ↓
Front Door Premium + WAF
  ↓
Private origin
  ↓
Application
```

Private origin protection prevents bypassing the edge where the
architecture requires centralized security and routing.
