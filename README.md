# Terraform AWS Infrastructure for Java Microservices

This project provisions foundational AWS infrastructure using **Terraform** to deploy a collection of **Java-based microservices** on **Amazon ECS with Fargate**, along with **Cloud Map for DNS-based service discovery**.

---

## Infrastructure Overview

### What This Creates:
- A **VPC** with public and private subnets
- An **ECS Cluster (Fargate)** to run containerized Java services
- A **Cloud Map Private DNS Namespace** for service discovery
- An **Application Load Balancer (ALB)** (optional, for ingress)
- **Security Groups**, **IAM Roles**, and supporting components

### DNS-Based Service Discovery:
Each microservice is registered with **AWS Cloud Map**, enabling it to communicate with others using DNS names like:

