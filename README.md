# DevOps Project 03 — Kubernetes + ArgoCD GitOps

This repo contains Kubernetes manifests managed via GitOps using ArgoCD.

## Manifests
- `manifests/deployment.yaml` — runs the app in Kubernetes
- `manifests/service.yaml` — exposes it via NodePort (Minikube)

## Expected flow
1. Commit/push changes to GitHub
2. ArgoCD detects changes and syncs the cluster automatically
