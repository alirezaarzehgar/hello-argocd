# Install ArgoCD on your cluster

Install ArgoCD just like its [official website](https://argo-cd.readthedocs.io/en/stable/getting_started/).

```bash
kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
```

The only manifest that you should apply using `kubectl` is on `application.yaml`.

```
kubectl apply -f ./application.yaml
```
