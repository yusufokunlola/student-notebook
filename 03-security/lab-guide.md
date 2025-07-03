# Lab: Apply Kubernetes Security Contexts

## 🛠 Task
Secure a pod using the `podsecuritypolicy-example.yaml`.

## ✅ Steps
1. Apply the security policy and observe changes:
```bash
kubectl apply -f podsecuritypolicy-example.yaml
kubectl get psp
```

2. Discuss the security settings used and their impact.

3. Reflect in `99-reflections/week3.md`.

## 📣 Share
Post insights or YAML snippets using `#KubeSkillsGROW` and `#K8sSecurity`.
