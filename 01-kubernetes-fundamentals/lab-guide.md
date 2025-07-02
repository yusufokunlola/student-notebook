# Lab: Deploy a Basic NGINX Pod

## 🛠 Task
Use `nginx-pod.yaml` to deploy a Pod to your cluster.

## ✅ Steps
1. Apply the YAML:
```bash
kubectl apply -f nginx-pod.yaml
kubectl get pods
kubectl describe pod nginx
```

2. Edit the manifest to add:
```yaml
securityContext:
  runAsNonRoot: true
```

3. Commit your work:
```bash
git commit -am "Added securityContext to nginx pod"
```

4. Reflect in `99-reflections/week1.md`.

## 📣 Share
Post your reflection or screenshot using `#KubeSkillsGROW`.
