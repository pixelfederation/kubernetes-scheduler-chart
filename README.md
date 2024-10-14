# Kubernetes scheduler 

[Kubernetes scheduler](https://kubernetes.io/docs/tasks/extend-kubernetes/configure-multiple-schedulers/) is a control plane process which assigns Pods to Nodes. The scheduler determines which Nodes are valid placements for each Pod in the scheduling queue according to constraints and available resources. The scheduler then ranks each valid Node and binds the Pod to a suitable Node. Multiple different schedulers may be used within a cluster; kube-scheduler is the reference implementation.


## Prerequisites

-	Kubernetes 1.21 or later

## Installing the Chart

The chart can be installed as follows:

```console
$ helm repo add kubernetes-scheduler https://pixelfederation.github.io/kubernetes-scheduler-chart
$ helm --namespace=kube-system install my-scheduler kubernetes-scheduler/kubernetes-scheduler
```

To uninstall/delete the `Kubernetes scheduler` deployment:

```console
$ helm uninstall my-scheduler
```
The command removes all the Kubernetes components associated with the chart and deletes the release.
