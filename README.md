# DevOps Project 03 — Kubernetes + ArgoCD GitOps

This project demonstrates real-world Kubernetes and GitOps workflows using ArgoCD as the GitOps controller.

## Kubernetes
- Application deployment using Kubernetes Deployments
- Service exposure using NodePort (Minikube)
- Horizontal scaling by adjusting replica count
- Zero-downtime rolling updates
- Instant rollbacks to previous application versions

## GitOps with ArgoCD
- Git as the single source of truth for cluster state
- Automatic synchronization between GitHub and Kubernetes
- Drift detection when manual changes are made in the cluster
- Self-healing: automatic restoration of desired state from Git

## Key Outcomes
- No manual `kubectl apply` required after GitOps setup
- Any configuration drift is automatically corrected by ArgoCD
- Changes are applied declaratively through Git commits

This setup reflects production-grade DevOps practices used in modern cloud-native environments.


This repo contains Kubernetes manifests managed via GitOps using ArgoCD.

## Manifests
- `manifests/deployment.yaml` — runs the app in Kubernetes
- `manifests/service.yaml` — exposes it via NodePort (Minikube)

## Expected flow
1. Commit/push changes to GitHub
2. ArgoCD detects changes and syncs the cluster automatically
