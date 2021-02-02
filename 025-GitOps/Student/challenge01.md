# What The Hack - GitOps enabled Kubernetes Hack

## Challenge 1 - Create an AKS cluster

[Back](challenge00.md) - [Home](../readme.md) - [Next](challenge02.md)

### Introduction

Before we begin managing Kubernetes clusters through GitOps, we first need to create Kubernetes clusters. In this challenge we are going to create a AKS cluster

Once this challenge is complete, we will have a cluster deployed and ready to be managed by Gitops. With the cluster deployed, we will be able to manage the cluster centrally via git repository.

### Challenge

1. Deploy a Azure Kubernetes cluster on Azure.
    * Run ```kubectl get nodes -o wide``` with the ```kubectl``` context being that of the newly created AKS cluster

### Success Criteria

This challenge will be complete when a AKS cluster is successfully created and ready to be enabled for GitOps.

[Back](challenge00.md) - [Home](../readme.md) - [Next](challenge02.md)