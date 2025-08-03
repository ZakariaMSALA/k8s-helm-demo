# ☸️ Kubernetes Helm Demo

This repository demonstrates how to deploy a simple web application using **Helm** on a Kubernetes cluster.

## 🧱 Project Structure

```
k8s-helm-demo/
├── helm/
│   └── myapp/
│       ├── Chart.yaml
│       ├── values.yaml
│       └── templates/
│           ├── deployment.yaml
│           └── service.yaml
```

## 🚀 How to Use

### 1. Prerequisites

- A Kubernetes cluster (e.g., Minikube, kind, EKS, GKE, etc.)
- Helm installed (`helm version`)

### 2. Install the Chart

```bash
cd helm
helm install myapp ./myapp
```

### 3. Check the Deployment

```bash
kubectl get all
```

### 4. Uninstall

```bash
helm uninstall myapp
```

## 🔧 Customize

Edit `values.yaml` to change:
- Image name and tag
- Replica count
- Port number

You can also add Ingress, ConfigMaps, or Secrets to extend the chart.

## 📬 Author

Zakaria Msala – Freelance DevOps Engineer  
[LinkedIn](https://linkedin.com/in/zakaria-msala)
