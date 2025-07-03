# Clusterctl

## Compatibility notice

The `clusterctl` CLI is developed in lock-step with Cluster API. We strongly recommend using the latest released version for the series you're using. For example, if you're managing clusters with Cluster API v0.3.7, the `clusterctl` version should be >= v0.3.7.

When this package is used as a library, we do not currently provide any compatibility guarantees. We will make reasonable efforts to follow a typical deprecation period prior to removal, but breaking changes can happen when necessary.


## Local changes

Support for local run to delete resources only in source cluster. Just to manual handle situations when we have resources in multiple management cluster and want to remove it from others to keep resources in single cluster
```
bin/clusterctl move --kubeconfig ./<source-cluster>.config  --namespace  <traget-cluster> --delete

```
