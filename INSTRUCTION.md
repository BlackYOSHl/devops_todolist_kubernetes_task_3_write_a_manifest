# Instructions for Deploying and Testing the ToDo App

## Prerequisites
- Kubernetes cluster (e.g., Minikube, Docker Desktop, etc.)
- `kubectl` installed and configured
- Docker installed and logged into your Docker Hub account

---

## Deployment Steps

1. **Create a namespace**:
   ```bash
   kubectl apply -f .infrastructure/namespace.yml

2. **Deploy the BusyBox Pod**:

kubectl apply -f .infrastructure/busybox.yml

3. **Deploy the ToDo App Pod**:

kubectl apply -f .infrastructure/todoapp-pod.yml

4. **Check the status of the Pods**:

kubectl get pods -n todoapp
