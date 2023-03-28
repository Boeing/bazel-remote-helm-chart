# bazel-remote-helm-chart

[Bazel Remote Cache](https://github.com/buchgr/bazel-remote)

[Bazel Build System](https://bazel.build/)
                           
## TL;DR

```bash
$ helm upgrade -i bazel-cache -n bazel-cache ./
```

There should be more values overrides allowed, so this chart needs more work and parameterization.

## Introduction

This chart bootstraps a Bazel Remote cache on a [Kubernetes](https://kubernetes.io) cluster using the [Helm](https://helm.sh) package manager.

## Prerequisites

- Kubernetes 1.19+ ?
  - kubectl
  - kube config file setup to use with kubectl
- Helm 3.2.0+ ?

## Installing the Chart

To install the chart with the release name `bazel-cache`:

```bash
$ helm upgrade -i bazel-cache -n bazel-cache --create-namespace ./
```

> **Tip**: List all releases using `helm list`

## Uninstalling the Chart

To uninstall/delete the `bazel-cache` deployment:

```bash
$ helm delete bazel-cache -n bazel-cache
```

The command removes all the Kubernetes components associated with the chart and deletes the release.
