# Minimal Helm Chart

A lightweight, production-ready Helm chart for deploying microservices with strict resource constraints, readiness/liveness probes, and configurable ingress. Designed for local development and edge deployments.

## Features
- Minimal resource footprints with configurable CPU/memory limits.
- Robust health checks (readiness and liveness probes).
- Configurable service and ingress parameters.
- Built-in horizontal pod autoscaling.

## Configuration

| Parameter | Description | Default |
| :--- | :--- | :--- |
| `replicaCount` | Number of replicas | `2` |
| `image.repository` | Container image repository | `nginx` |
| `resources.limits.cpu` | CPU limit | `200m` |
| `autoscaling.enabled` | Enable HPA | `false` |
