# argo-deployments

### Installation

``` 
argocd app create apps \
    --dest-namespace argocd \
    --dest-server https://kubernetes.default.svc \
    --repo https://github.com/cdutten/argo-deployments.git \
    --path apps-of-apps
argocd app sync apps 
```