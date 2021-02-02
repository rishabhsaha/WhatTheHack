# What The Hack - Gitops enabled Kubernetes Hack

## Challenge 4 – Deploy apps using Gitops

[Back](challenge03.md) - [Home](../readme.md) - [Next](challenge05.md)

### Introduction

Now that you have deployed an application in the cluster using the vanilla k8 constructs, in this challenge we will be doing the same using flux to showcase the benefits of Gitops.

### Challenge

1. Clone the fleet-infra repo created by flux on your local machine.
2. Add the podinfo repository used in the previous challenge to Flux.
3. Deploy podinfo application using flux
4. Watch flux sync the application

### Success Criteria

This challenge will be complete when you can verify that podinfo has been deployed on your cluster.
```
$ kubectl -n default get deployments,services
NAME                      READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/podinfo   2/2     2            2           108s

NAME                 TYPE        CLUSTER-IP       EXTERNAL-IP   PORT(S)             AGE
service/podinfo      ClusterIP   10.100.149.126   <none>        9898/TCP,9999/TCP   108s
```

[Back](challenge03.md) - [Home](../readme.md) - [Next](challenge05.md)
