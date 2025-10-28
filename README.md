# Azure Infrastructure as Code (IaC) ☁️

ARM + Terraform templates for secure, governed Azure deployments at scale.

[![Azure](https://img.shields.io/badge/Azure-Cloud%20Platform-blue.svg)](https://azure.microsoft.com)
[![ARM](https://img.shields.io/badge/ARM-Templates-orange.svg)](#)
[![Terraform](https://img.shields.io/badge/Terraform-Infrastructure-purple.svg)](#)
[![PowerShell](https://img.shields.io/badge/PowerShell-Automation-blue.svg)](#)

> **Enterprise Azure infrastructure automation and deployment templates for scalable cloud operations**

A professional collection of **Azure Resource Manager (ARM) templates**, **Terraform configurations**, and **PowerShell automation scripts**.

---

## ⚡ How to review in 2 minutes
1) ARM Hub VNet (dev parameters)
```
az group create -n iac-demo-rg -l westeurope
az deployment group create \
 --resource-group iac-demo-rg \
 --template-file ./Security-Templates/virtual-network-hub-spoke.json \
 --parameters @./Security-Templates/virtual-network-hub-spoke.parameters.json
```
2) Log Analytics Workspace
```
az deployment group create \
 --resource-group iac-demo-rg \
 --template-file ./Monitoring-Solutions/log-analytics-workspace.json
```
3) Terraform quick start
```
cd terraform
terraform init && terraform apply -auto-approve
```

---

## 📁 Structure
- Security-Templates/virtual-network-hub-spoke.json
- Security-Templates/virtual-network-hub-spoke.parameters.json
- Monitoring-Solutions/log-analytics-workspace.json
- Scripts/Deploy-Infrastructure.ps1
- terraform/main.tf

## 👤 Author
**Julien Chevallier** — Senior IT Support Engineer

---

⭐ Star this repo if it helped accelerate your Azure cloud journey.
