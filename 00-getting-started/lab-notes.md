# 🧪 Lab Notes – Getting Started

Welcome! This is your first notebook entry in the GROW program.  
Use this space to document the setup of your **Kubernetes learning environment** and reflect on what you’re configuring.

---

## ✅ Goals
By the end of this section, you will:
- Install and configure basic Kubernetes CLI tools
- Create your first local Kubernetes cluster using `kind`
- Deploy and inspect your first Pod
- Verify your setup is working for the labs ahead

---

## 🛠️ Step-by-Step Setup Instructions

### Step 1: Install `kubectl`
Follow the official guide:  
➡️ https://kubernetes.io/docs/tasks/tools/install-kubectl/

Verify:
```bash
kubectl version --client
```

### Step 2: Install `kind` (Kubernetes IN Docker)
Follow the official guide:  
➡️ https://kind.sigs.k8s.io/docs/user/quick-start/

Verify:
```bash
kind version
```

---

### Step 3: Create a Local Cluster
```bash
kind create cluster --name grow-lab
```

Check your nodes:
```bash
kubectl get nodes
```

---

### Step 4: Deploy Your First Pod
```bash
kubectl run nginx --image=nginx
kubectl get pods
```

Describe it:
```bash
kubectl describe pod nginx
```

Delete it:
```bash
kubectl delete pod nginx
```

---

## 🧠 What I Did

- Installed `kubectl` and `kind`
- Created a local cluster named `grow-lab`
- Ran and deleted my first Pod using `kubectl`

---

## ❓ Questions I Still Have

- What's the difference between a Deployment and a ReplicaSet?
- How do services expose Pods to the outside world?
- What happens when a Pod crashes?

---

## 🧪 Commands I Used

```bash
kubectl cluster-info
kind create cluster --name grow-lab
kubectl run nginx --image=nginx
kubectl describe pod nginx
kubectl delete pod nginx
```

---

## 📝 Don’t Forget to Reflect

Once you've completed the steps above, open:  
👉 `99-reflections/week1.md`  

Use that file to write:
- ✅ What you learned
- 🤔 What was unclear
- 🔍 Any new commands or tools you used

This is your opportunity to **document your learning** and start building a public, portfolio-ready trail.

---

## 🎯 Next Step

When ready, move on to your first official lab:  
👉 [Kubernetes Fundamentals – Deploying a Pod](../01-kubernetes-fundamentals/lab-guide.md)
