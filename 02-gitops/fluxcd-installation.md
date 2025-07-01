# Installing FluxCD on a Kubernetes Cluster

## Commands Used
```
flux install

flux create source git my-app \
  --url=https://github.com/myuser/app \
  --branch=main \
  --interval=30s

flux create kustomization my-app \
  --target-namespace=default \
  --source=GitRepository/my-app \
  --path="./manifests" \
  --prune=true \
  --interval=5m

```
