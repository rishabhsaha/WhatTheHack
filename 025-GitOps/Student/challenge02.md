# What The Hack - GitOps enabled Kubernetes Hack

## Challenge 2 – Set up GitOps on AKS
[Back](challenge01.md) - [Home](../readme.md) - [Next](challenge03.md)

### Introduction

Flux keeps Kubernetes clusters in sync with configuration kept under source control like Git repositories, and automates updates to that configuration when there is new code to deploy. In this challenge, we’ll set up Flux to synchronize changes in the git repository.

### Description

#### Enable GitOps on your cluster

* [Install](https://toolkit.fluxcd.io/get-started/#install-flux-components) Flux components in the cluster
* Set up a GitHub [a personal access token](https://help.github.com/en/github/authenticating-to-github/creating-a-personal-access-token-for-the-command-line) token
* The token must have all permissions under repo checked off. Copy and keep your token handy and in a safe place
* On the command line, export your GitHub personal access token and username on the command line
* Create the Flux reconciliation repository. In this case you’ll call it fleet-infra, but you can call it anything you want. In this step, a private repository is created and all of the controllers will also be installed to your AKS cluster. When bootstrapping a repository with Flux
* Check the cluster for the flux-system namespace with: 
`kubectl get namespaces`
* Clone the fleet-infra repo on your local machine

### Success Criteria

This challenge will be complete once you finish bootstrapping your cluster and see the following: 

```
► connecting to github.com
✔ repository cloned
✚ generating manifests
✔ components manifests pushed
► installing components in flux-system namespace …..
deployment "source-controller" successfully rolled out
deployment "kustomize-controller" successfully rolled out
deployment "helm-controller" successfully rolled out
deployment "notification-controller" successfully rolled out
```

[Back](challenge01.md) - [Home](../readme.md) - [Next](challenge03.md)
