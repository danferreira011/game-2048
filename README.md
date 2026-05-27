# 🎮 Deploy do Jogo 2048 no Amazon EKS (AWS Kubernetes)

Projeto prático reproduzido a partir da documentação oficial da AWS para implantação do jogo **2048** em um cluster **Amazon EKS (Elastic Kubernetes Service)**, utilizando **Kubernetes**, **AWS Load Balancer Controller** e **Ingress** para exposição da aplicação.

## 📌 Objetivo

O objetivo deste projeto foi praticar conceitos fundamentais de:

- Kubernetes na AWS
- Provisionamento e gerenciamento de clusters EKS
- Deploy de aplicações containerizadas
- Exposição de aplicações com Ingress
- Integração com AWS Load Balancer Controller
- Troubleshooting em ambiente Kubernetes

Além de reforçar conhecimentos em **Cloud Computing**, **Containers** e **DevOps** através de um cenário real de implantação.

---

## 🏗️ Arquitetura da Solução

A aplicação foi implantada em um cluster **Amazon EKS**, utilizando recursos do Kubernetes para orquestração dos containers.

Fluxo da arquitetura:

```text
Usuário
   ↓
AWS Application Load Balancer (ALB)
   ↓
Kubernetes Ingress
   ↓
Service
   ↓
Pod (Aplicação 2048)

[projeto original](https://docs.aws.amazon.com/eks/latest/userguide/quickstart.html#quickstart-deploy-game)