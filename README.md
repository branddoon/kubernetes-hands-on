# Kubernetes Configurations

A collection of Kubernetes configuration files and exercises covering the main concepts of K8s, organized by topic.

## Requirements

- [Docker](https://docs.docker.com/get-docker/)
- [kubectl](https://kubernetes.io/docs/tasks/tools/)
- [Minikube](https://minikube.sigs.k8s.io/docs/start/) (local cluster)

## Repository Structure

| Folder | Description |
|--------|-------------|
| `pods/` | Basic Pod definitions, multi-container pods, and labels |
| `deployment/` | Deployment configurations |
| `replicaSet/` | ReplicaSet definitions |
| `service/` | Service configurations |
| `ingress/` | Ingress controller and routing rules |
| `namespaces/` | Namespace definitions |
| `configmaps/` | ConfigMap examples |
| `secrets/` | Secrets (env vars and volume mounts) |
| `envs/` | Environment variable injection |
| `volumes/` | PersistentVolumes, PVCs, EmptyDir, and StorageClass |
| `limits-request/` | CPU and RAM resource limits and requests |
| `probes/` | Liveness probes (HTTP, TCP, exec) |
| `RBAC/` | Role-Based Access Control, ClusterRoles, and ServiceAccounts |
| `k8s-hands-on/` | Full hands-on example with frontend and backend |

## Usage

Apply any configuration file with:

```bash
kubectl apply -f <filename>
```

### Common kubectl Commands

```bash
# List resources
kubectl get pods | deployments | services | ...

# Inspect a resource
kubectl describe <resource> <name>

# Delete a resource
kubectl delete -f <filename>

# Create a resource imperatively
kubectl create <resource> <name>

# Edit a live resource
kubectl edit <resource> <name>

# View logs
kubectl logs <pod-name>
```

### Start Minikube

```bash
minikube start
```
