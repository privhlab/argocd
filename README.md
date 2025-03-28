# ArgoCD Helm Charts for Homelab

This repository contains independent Helm charts for deploying and managing ArgoCD in a Homelab environment. ArgoCD is a declarative, GitOps continuous delivery tool for Kubernetes.

## Features

- Customizable Helm charts tailored for Homelab setups.
- Simplified deployment of ArgoCD on Kubernetes clusters.
- Support for GitOps workflows to manage Kubernetes resources.

## Prerequisites

- Kubernetes cluster (v1.20 or later recommended).
- Helm (v3 or later).
- Basic knowledge of Kubernetes and Helm.

## Installation

1. Add dependencies to your Helm repositories:

```bash
helm dependency build
```

2. Install the chart:
```bash
helm install argocd . --values values_dev.yaml --namespace argocd --create-namespace
```

3. Customize the chart values [values_dev.yaml](values_dev.yaml) to suit your environment.

4. Upgrade the deployment:

```bash
helm upgrade argocd . --values values_dev.yaml --namespace argocd
```

## Automated Deployment via ArgoCD

- tbd