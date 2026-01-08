# Home Lab

Personal AI/ML infrastructure for development and experimentation.

## Architecture

- **Dev**: MacBook (Apple Silicon) — local development, multi-arch container builds
- **Prod**: Dell XPS (K3s) — single-node Kubernetes cluster for deployments
- **Edge**: Raspberry Pi — face detection, IoT projects

## Stack

- **Orchestration**: K3s (lightweight Kubernetes)
- **Monitoring**: Grafana + Prometheus
- **CI/CD**: GitHub Actions → GitHub Container Registry → K3s
- **Containers**: Docker/Podman with `buildx` for multi-arch (ARM64 + AMD64)

## Workflow

```
Mac (build) → ghcr.io (push) → Dell XPS K3s (deploy)
```

## Projects

- **Eashan Calling Eashan [https://github.com/eashanchawla/eashan-calling-eashan]** — AI telephony agent with voice cloning
- **Visitor Recognition** — Raspberry Pi face detection system
- **Home Automation** — Various automation experiments
