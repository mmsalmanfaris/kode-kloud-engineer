# Kubernetes Task 1: Create Nginx Pod

Run the following command to create the pod:

```bash
kubectl run pod-nginx \
  --image=nginx:latest \
  --labels=app=nginx_app \
  --restart=Never \
  --dry-run=client -o yaml \
| sed 's/name: pod-nginx/name: nginx-container/' \
| kubectl apply -f -
```
