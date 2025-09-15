<!-- markdownlint-disable MD041 -->
<p align="center">
  <img width="400px" height="auto" src="./bitmoa.png" />
</p>

bitmoa comes from two Korean words: “빛” (bit, meaning light) and “모아” (moa, meaning to gather). The name symbolizes the idea of gathering individual lights together to create a brighter, shared future. At its core, bitmoa represents a community-driven spirit, where collaboration and collective growth shine more brightly than any effort alone.

<p align="center">
    <a href="https://github.com/bitmoa/charts-dev"><img src="https://badgen.net/github/stars/bitmoa/charts-dev?icon=github" /></a>
    <a href="https://github.com/bitmoa/charts-dev"><img src="https://badgen.net/github/forks/bitmoa/charts-dev?icon=github" /></a>
    <a href="https://github.com/bitmoa/charts-dev/actions/workflows/cd-pipeline.yml"><img src="https://github.com/bitmoa/charts-dev/actions/workflows/cd-pipeline.yml/badge.svg" /></a>
</p>

# The Bitmoa Library for Kubernetes

Popular applications, provided by [Bitmoa](https://bitmoa.net), ready to launch on Kubernetes using [Kubernetes Helm](https://github.com/helm/helm).

## TL;DR

```console
helm install my-release oci://registry-1.docker.io/bitmoacharts/<chart>
```


## Vulnerabilities scanner

Each Helm chart contains one or more containers. Those containers use images provided by Bitmoa and other upstream projects. The exact image registries and tags are defined per chart (see the values.yaml of each chart). Bitmoa-published images are primarily available at ghcr.io/bitmoa and docker.io as specified by each chart.

As part of our release process, images and charts are scanned and validated. We focus on ensuring the Helm charts work as expected and follow best practices. See our testing strategy in TESTING.md for more details.

## Before you begin

### Prerequisites

- Kubernetes 1.23+
- Helm 3.8.0+

### Setup a Kubernetes Cluster

The quickest way to set up a Kubernetes cluster to install Bitnami Charts is by following the "Bitnami Get Started" guides for the different services:

- [Get Started with Bitnami Charts using VMware Tanzu Kubernetes Grid (TKG)](https://docs.bitnami.com/kubernetes/get-started-tkg/)
- [Get Started with Bitnami Charts using VMware Tanzu Mission Control (TMC)](https://docs.bitnami.com/kubernetes/get-started-tmc/)
- [Get Started With Bitnami Charts Using Azure Marketplace Kubernetes Applications](https://docs.bitnami.com/kubernetes/get-started-cnab/)
- [Get Started with Bitnami Charts using the Amazon Elastic Container Service for Kubernetes (EKS)](https://docs.bitnami.com/kubernetes/get-started-eks/)
- [Get Started with Bitnami Charts using the Google Kubernetes Engine (GKE)](https://docs.bitnami.com/kubernetes/get-started-gke/)

For setting up Kubernetes on other cloud platforms or bare-metal servers refer to the Kubernetes [getting started guide](https://kubernetes.io/docs/getting-started-guides/).

### Install Helm

Helm is a tool for managing Kubernetes charts. Charts are packages of pre-configured Kubernetes resources.

To install Helm, refer to the [Helm install guide](https://github.com/helm/helm#install) and ensure that the `helm` binary is in the `PATH` of your shell.

### Using Helm

Once you have installed the Helm client, you can deploy a Bitmoa Helm Chart into a Kubernetes cluster.

Please refer to the [Quick Start guide](https://helm.sh/docs/intro/quickstart/) if you wish to get running in just a few commands, otherwise, the [Using Helm Guide](https://helm.sh/docs/intro/using_helm/) provides detailed instructions on how to use the Helm client to manage packages on your Kubernetes cluster.

Useful Helm Client Commands:

- Install a chart: `helm install my-release oci://registry-1.docker.io/bitmoacharts/<chart>`
- Upgrade your application: `helm upgrade my-release oci://registry-1.docker.io/bitmoacharts/<chart>`

## License

Copyright &copy; 2025 Broadcom. The term "Broadcom" refers to Broadcom Inc. and/or its subsidiaries.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

<http://www.apache.org/licenses/LICENSE-2.0>

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
