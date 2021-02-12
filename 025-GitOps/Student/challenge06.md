# What The Hack - Gitops enabled Kubernetes Hack

## Challenge 6 – Setup HelmRelease Operator

[Back](challenge05.md) - [Home](../readme.md) - [Next](challenge07.md)

### Introduction

In this challenge we will use the helm-controller to declaratively manage Helm chart releases with Kubernetes manifests.The helm-controller is part of the default toolkit installation. This challenge will help understand how helm releases can be done declaratively using GitOps.

### Challenge

1. Define a HelmRepository chart source to release a Helm chart. This is the source that will contain the chart.
2. Define a HelmRelease to release the new chart.
3. Pass in configuration values using HelmRelease.
1. Evaluate options to pass in values through config map and secrets.
1. Distinguish between standard helm deployments and HelmRelease.

### Success Criteria

This challenge will be complete when the application is deployed in the cluster using HelmRelease after it is committed to the git repository.

[Back](challenge05.md) - [Home](../readme.md) - [Next](challenge07.md)
