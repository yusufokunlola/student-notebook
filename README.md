# 📘 KubeSkills Student Notebook Template

Welcome to your **KubeSkills GitHub Repository of Work (GROW)** notebook!
This repo is your personal space to document everything you learn as you grow your Kubernetes skills.

> ✅ Fork this repo to get started.

---

## 📁 Repository Structure

```
student-notebook/
├── README.md
├── 00-getting-started/
│   └── lab-notes.md
├── 01-kubernetes-fundamentals/
│   └── pod-definition.yaml
├── 02-gitops/
│   ├── fluxcd-installation.md
│   └── kustomize-example.yaml
├── 03-security/
│   └── podsecuritypolicy-example.yaml
├── 99-reflections/
│   └── week1.md
└── .github/
    └── CONTRIBUTING.md
```

---

## 🛠 How to Use This Repo

1. **Document Labs**
   - After each KubeSkills lab or tutorial, copy relevant manifests into the correct folder.
   - Write a short explanation: What did you learn? What was hard? Any commands you used?

2. **Track Your Progress**
   - Add `weekX.md` files under `99-reflections/`.
   - Write 2-3 bullet points about what you accomplished or questions you still have.

3. **Show Your Work**
   - Keep your commits clean and meaningful.
   - Push changes regularly—this becomes part of your portfolio!

---

## ✨ Example Entries

### `01-kubernetes-fundamentals/pod-definition.yaml`
```yaml
apiVersion: v1
kind: Pod
metadata:
  name: my-first-pod
spec:
  containers:
    - name: nginx
      image: nginx
```

### `02-gitops/fluxcd-installation.md`
```
## Installed FluxCD on K3s using the following commands:

```bash
flux install
flux create source git my-app --url=https://github.com/myuser/app --branch=main
```

Learned how GitOps automates deployment using version control!
```

---

## 🧪 Starter Tasks

- [ ] Fork this repository
- [ ] Create a `week1.md` file under `99-reflections/`
- [ ] Complete the "Getting Started" lab and document it
- [ ] Push your changes to GitHub

---

## 🌐 Share & Connect

- Tag us on LinkedIn or X: `#KubeSkills #GROWportfolio`
- Want your notebook featured? Submit it to `notebooks@kubeskills.com`

---

## 📜 License
MIT

Happy learning, and welcome to the community of Kubernetes builders!

— The KubeSkills Team 🚀
