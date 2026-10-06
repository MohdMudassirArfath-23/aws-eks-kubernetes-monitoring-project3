# AWS EKS Kubernetes Cluster Setup & Monitoring

##  Project Overview

This project demonstrates the setup, deployment, and monitoring of a Kubernetes application using *Amazon Elastic Kubernetes Service (AWS EKS)*.

An NGINX containerized application was deployed on an AWS EKS cluster using Kubernetes Deployment and Service manifests. The cluster was monitored using *Prometheus and Grafana, with **AWS CloudWatch integrated into Grafana* for additional Kubernetes and infrastructure monitoring.

---

##  Technologies Used

- AWS EKS
- Kubernetes
- Docker
- kubectl
- Helm
- Prometheus
- Grafana
- AWS CloudWatch
- YAML
- AWS Load Balancer

---

##  Project Architecture

```text
                    AWS Cloud
                       │
                       ▼
                 Amazon EKS
                       │
              ┌────────┴────────┐
              │                 │
              ▼                 ▼
       NGINX Application     Monitoring
              │                 │
              ▼                 ├── Prometheus
      Kubernetes Service        │
              │                 └── Grafana
              ▼                       │
       AWS Load Balancer              ▼
                                AWS CloudWatch
                                       │
                                       ▼
                              Container Insights
