## 🚀 Helm Charts Repository

A centralized Helm charts repository designed to manage, version, and deploy multiple Kubernetes applications using **standardized, reusable, and production-ready configurations**.

---

## 🌐 Overview

This repository serves as a **scalable Helm chart hub**, enabling consistent and repeatable deployments of cloud-native applications across Kubernetes environments. It reflects real-world DevOps practices by combining **Helm packaging, version control, and repository-based distribution**.

---

## 📁 Repository Structure

```
.
├── index.yaml
├── cloud-native-todo-app-0.1.0.tgz
├── <future-app>-<version>.tgz
└── README.md
```

---

## 📦 Available Charts

| Chart Name            | Version | Description                                  |
| --------------------- | ------- | -------------------------------------------- |
| cloud-native-todo-app | 0.1.0   | Cloud-native To-Do application on Kubernetes |
| *(more coming soon)*  | —       | Additional applications will be added        |

---

## ⚙️ Prerequisites

* Kubernetes Cluster
* Helm (v3 or above)

---

## 🔧 Add Helm Repository

```
helm repo add avindock https://Avinash8600.github.io/helm-charts
helm repo update
```

---

## 🔍 Search Charts

```
helm search repo avindock
```

---

## 🚀 Install Application

```
helm install prd-todo-app avindock/cloud-native-todo-app -n todo-ns
```

---

## 🔄 Upgrade Application

```
helm upgrade prd-todo-app avindock/cloud-native-todo-app -n todo-ns
```

---

## ❌ Uninstall Application

```
helm uninstall prd-todo-app -n todo-ns
```

---

## 📌 Versioning Strategy

All charts follow **Semantic Versioning**:

**MAJOR.MINOR.PATCH**

* `0.1.0` → Initial release
* `0.2.0` → Feature enhancements
* `1.0.0` → Stable production release

---

## 🔄 Publishing / Updating Charts

```
helm package <chart-directory>
helm repo index . --merge index.yaml
git add .
git commit -m "Add/Update Helm chart"
git push
```

---

## 🧠 Key Highlights

* Centralized Helm repository supporting multiple applications
* Reusable and standardized Kubernetes deployment configurations
* Version-controlled releases for consistent environments
* Lightweight Helm hosting using GitHub Pages
* Implementation of production-style DevOps workflows

---

## 🎯 Why This Repository Stands Out

This project demonstrates how modern DevOps teams:

* Package applications as Helm charts
* Maintain centralized repositories
* Enable consistent, scalable deployments across environments

It reflects a **real-world cloud-native deployment approach**, making it highly relevant for production scenarios.

---

## 🚀 Roadmap

* Add multiple application Helm charts
* Implement CI/CD for automated chart publishing
* Integrate Helm OCI registry support
* Introduce environment-based configurations (dev/staging/prod)

---

## 👨‍💻 Author

**Avinash Wagh**
Software Engineer | DevOps & Cloud Enthusiast

---

## 📄 License

This project is licensed under the MIT License.
