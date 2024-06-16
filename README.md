# EKS configs

## Story

Hackers from all around the world could use your cloud resource for bad purposes, and that is why you will need to make sure to protect your data! With handling cloud resources, it is very important to handle sensitive data securely to keep everything safe from exploitation.

## What are you going to learn?

- How to store sensitive information and credentials securly in your k8s cluster
- How to use ConfigMaps to decouple configuration artifacts from image
- How to to check your pod's status with probes

## Tasks

1. Install Prometheus and Grafana with `kubectl`.
    - You can reach Prometheus and Grafana from your browser.

2. Store Grafana passwords in kubernetes `Secret`.
    - Upon getting information about the cluster's secrets, you can see your secret with the grafana credentials inside

3. Set up a 5 sec `livenessProbe` and a 2 min `readinessProbe` for both.
    - livenessProbe successfully added
    - readinessProbe successfully added
    - Upgrade finished successfully

4. Use kubectl to configure the Grafana username and password with `ConfigMap`
    - Grafana is configured with Prometheus as a data source.

## General requirements

None

## Hints

- Use the `prom/prometheus` and `grafana/grafana` docker images

## Background materials

* <i class="far fa-book-open"></i> [Configure a Pod to Use a ConfigMap](https://kubernetes.io/docs/tasks/configure-pod-container/configure-pod-configmap/ )
* <i class="far fa-book-open"></i> [Configure k8s Probes](https://kubernetes.io/docs/tasks/configure-pod-container/configure-liveness-readiness-startup-probes/)
* <i class="far fa-book-open"></i> [Secrets in k8s](https://kubernetes.io/docs/concepts/configuration/secret/)
