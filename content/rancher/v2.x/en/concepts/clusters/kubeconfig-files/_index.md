---
title: Kubeconfig Files
weight: 2100
---

A _kubeconfig file_ is a file used to configure access to Kubernetes when used in conjunction with the kubectl commandline tool (or other clients).

For more details on how kubeconfig and kubectl work together, see the [Kubernetes documentation](https://kubernetes.io/docs/tasks/access-application-cluster/configure-access-multiple-clusters/).

When you create a cluster using the Rancher GUI, Rancher automatically creates a kubeconfig for your cluster.

This kubeconfig file and its contents are specific to the cluster you are viewing. You will need a separate kubeconfig file for each cluster that you have access to in Rancher.

For more information, see [Using kubectl to Access a Cluster]({{< baseurl >}}/rancher/v2.x/en/tasks/clusters/using-kubectl-to-access-a-cluster).

>**Note:** By default, kubectl checks `~/.kube/config` for kubeconfig files, but you can use any directory you want using the `--kubeconfig` flag. For example:
>```
kubectl --kubeconfig /custom/path/kube.config get pods
```


