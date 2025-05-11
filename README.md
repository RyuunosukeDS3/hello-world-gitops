# DevSecOps Hello World GitOps

This repository demonstrates a GitOps-based DevSecOps workflow using **Argo CD** and **Helm** to deploy a simple "Hello World" application with frontend and backend services.

The setup uses:

- **Argo CD ApplicationSet** to manage applications declaratively
- **Helm values** to configure each app individually
- **Git as the single source of truth**

---

## 🔧 How It Works

Each component (frontend and backend) is deployed via an Argo CD Application that references:

- An **external Helm chart**
- A `values.yaml` file for configuration
- Optional raw Kubernetes manifests (e.g., secrets, ingress)

---

## 🛡 DevSecOps Practices

This repo serves as an educational example of:

- GitOps with Argo CD and ApplicationSets
- Secure, declarative deployment workflows
- Clear separation of configuration and infrastructure
- Extensible structure for adding CI, policies, or security scanning

---

## 📄 License

[MIT License](LICENSE)
