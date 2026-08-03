# Minimal Helm Chart

A lightweight, production-ready Helm chart for deploying microservices with strict resource constraints, readiness/liveness probes, and configurable ingress. Designed for local development and edge deployments.

## Features
- Minimal resource footprints with configurable CPU/memory limits.
- Robust health checks (readiness and liveness probes).
- Configurable service and ingress parameters.

## Configuration

| Parameter | Description | Default |
| --------- | ----------- | ------- |
| `replicaCount` | Number of replicas | 2 |
| `image.repository` | Image repository | nginx |
| `image.tag` | Image tag | 1.25-alpine |
| `resources.limits.cpu` | CPU limit | 200m |
| `resources.limits.memory` | Memory limit | 256Mi |
| `resources.requests.cpu` | CPU request | 100m |
| `resources.requests.memory` | Memory request | 128Mi |
