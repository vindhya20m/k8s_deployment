# k8s_deployment
# Kubernetes Deployment: Nginx or Node.js App

This setup includes:
- A Deployment with 3 replicas
- ConfigMap for environment variable `APP_ENV=prod`
- ClusterIP Service exposing port 80
- Horizontal Pod Autoscaler (HPA) scaling between 3–10 pods based on CPU usage

## 🛠️ Apply Resources

```bash
kubectl apply -f configmap.yaml
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl apply -f hpa.yaml
