# What The Hack - Gitops enabled Kubernetes Hack

## Challenge 8 – Using GitOps to Manage HA & DR in AKS

[Back](challenge07.md) - [Home](../readme.md) - [Next](challenge09.md)

### Introduction

In this challenge we will configure a multi-cluster set up and configure AKS services such as AppGW and Traffic Manager(https://docs.microsoft.com/en-us/azure/architecture/high-availability/reference-architecture-traffic-manager-application-gateway)
https://www.azure-heros.com/blog/azure-front-door-vs-azure-traffic-manager-vs-azure-application-gateway-vs-azure-load-balancer-vs-content-delivery-network-cdn
https://docs.microsoft.com/en-us/azure/traffic-manager/traffic-manager-load-balancing-azure


### Challenge

1. Challenge Prerequisites
2. Create another AKS cluster in another region.
3. Repeat steps in Challenge 07 for this new cluster.
1. Create Application Gateway v2
1. Add YAMLs to repo (https://docs.microsoft.com/en-us/azure/application-gateway/ingress-controller-install-new)
    1. Install AppGW Ingress Controller using HelmRelease
    1. Install Azure AD Pod Identity using GitOps
    1. Connect the app service to the ingress controller
    1. Test the ingress set up
    1. Create a configure Traffic Manager to route traffic to both AKS clusters (Optional)


### Success Criteria

This challenge will be complete when new cluster can have the same baseline items applied to it as an existing one. (Learning resources to docs.Internal folks. )

[Back](challenge06.md) - [Home](../readme.md) - [Next](challenge08.md)
