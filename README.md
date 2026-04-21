# 📦 Helm Charts Repository

Centralized Helm charts repository for managing, versioning, and deploying Kubernetes applications using standardized, reusable, and production-ready configurations.

---

## 🚀 Overview

This repository contains Helm charts for deploying and managing containerized applications on Kubernetes. It enables consistent, scalable, and repeatable deployments using Helm packaging and versioning.

---

## 📁 Repository Structure

```
.
├── index.yaml
├── cloud-native-todo-app-0.1.0.tgz
└── README.md
```

---

## 📦 Available Charts

| Chart Name            | Version | Description                                             |
| --------------------- | ------- | ------------------------------------------------------- |
| cloud-native-todo-app | 0.1.0   | A cloud-native To-Do application deployed on Kubernetes |

---

## ⚙️ Prerequisites

* Kubernetes Cluster
* Helm installed (v3+)

---

## 🔧 Add Helm Repository

```bash
helm repo add avindock https://<your-username>.github.io/helm-charts
helm repo update
```

---

## 🔍 Search Charts

```bash
helm search repo avindock
```

---

## 🚀 Install Chart

```bash
helm install prd-todo-app avindock/cloud-native-todo-app -n todo-ns
```

---

## 🔄 Upgrade Chart

```bash
helm upgrade prd-todo-app avindock/cloud-native-todo-app -n todo-ns
```

---

## ❌ Uninstall Chart

```bash
helm uninstall prd-todo-app -n todo-ns
```

---

## 📌 Versioning

Charts follow semantic versioning:

```
MAJOR.MINOR.PATCH
```

Example:

```
0.1.0 → Initial release
```

---

## 🔄 Updating Charts

```bash
helm package .
helm repo index . --merge index.yaml
```

Push updated files to GitHub to reflect changes.

---

## 🧠 Key Features

* 📦 Helm-based packaging
* 🔁 Reusable configurations
* 📊 Version-controlled deployments
* ☁️ Cloud-native architecture
* ⚙️ Easy Kubernetes integration

---

## 👨‍💻 Author

**Avinash Wagh**
Software Engineer | DevOps & Cloud Enthusiast

---

## 📄 License

This project is open-source and available under the MIT License.

---
