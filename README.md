# 🚀 Projet React + Node.js avec Pipeline DevOps

## 📌 Description
Ce projet est une application **fullstack** composée :
- **Frontend** : React (interface utilisateur moderne)
- **Backend** : Node.js / Express (API REST)

L’objectif est de montrer la mise en place d’un **workflow DevOps complet** depuis le développement jusqu’au déploiement automatisé sur une infrastructure virtualisée avec **Proxmox**.

---

## 🏗️ Architecture

---

## ⚙️ Outils utilisés

- **Gestion d’infrastructure**
  - Proxmox (virtualisation)
  - Terraform + Cloud-init (provisionnement automatisé des VM)
  - Ansible (déploiement et configuration automatisés)

- **Conteneurisation & Orchestration**
  - Docker
  - Kubernetes (CNI Flannel)
  - Trivy (scan de vulnérabilités)

- **CI/CD & Qualité**
  - Jenkins (pipelines CI/CD)
  - SonarQube (analyse qualité du code)

- **Monitoring & Observabilité**
  - Grafana
  - Prometheus

---

## 🚀 Déploiement

1. **Provisioning des serveurs**
   - Terraform + Cloud-init pour créer automatiquement les VMs sur Proxmox
   - Ansible pour configurer l’environnement (installation Docker, K8s, etc.)

2. **CI/CD**
   - Jenkins pipeline qui :
     - clone le dépôt GitHub
     - construit les images Docker
     - lance les tests
     - déploie sur Kubernetes

3. **Orchestration**
   - Kubernetes gère le déploiement et le scaling
   - Flannel pour le réseau
   - Trivy scanne les images Docker

4. **Monitoring**
   - Prometheus collecte les métriques
   - Grafana les visualise (dashboards)

---

## 📂 Structure du dépôt

