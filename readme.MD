# ops-infra-argo

to install argo: 

```
kubectl create namespace argo

helm install argocd argocd-install/argocd/ -f .\argocd-install\argocd\values.yaml --namespace argo

helm install argocd-apps argocd-install/argocd-apps/ -f .\argocd-install\argocd-apps\values.yaml --namespace "argo"
```