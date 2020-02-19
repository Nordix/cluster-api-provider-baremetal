# Cluster API provider Bare Metal

This provider integrates with the
[Cluster API project](https://github.com/kubernetes-sigs/cluster-api).

## Setup

### Pre-requisites

The pre-requisite for the deployment of CAPBM are the following:
- [Baremetal-Operator](https://github.com/metal3-io/baremetal-operator) deployed
- Ironic up and running (inside or outside of the cluster)
- BareMetalHost resources created for all hardware nodes and in "ready" or
  "available" state

### Using clusterctl

Please refer to
[Clusterctl documentation](https://master.cluster-api.sigs.k8s.io/clusterctl/overview.html).
Once the Pre-requisites are fulfilled, you can follow the normal clusterctl
flow.

## Pivoting Ironic

Before running the move command of Clusterctl. Baremetal Operator, Ironic if
applicable, and the BareMetalHost CRs need to be moved to the target cluster.
More information TBA.
