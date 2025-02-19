

## Argo Install

```bash
kubectl apply -f k8s/argocd/deployment.yml -n argocd
```

## Get Argo Secret


```bash
kubectl get secret argocd-initial-admin-secret -n argocd -o jsonpath="{.data.password}" | base64 -d
```