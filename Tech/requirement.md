# Virtual Machines Requirements

This document outlines the virtual machine (VM) requirements for development, staging, and production environments, including infrastructure and service VMs. Each VM also specifies its deployment location.

## Environments

- **Development**
- **Staging**
- **Production**

## VM Roles

- **Infrastructure VM**
- **Service VM**
- **Nexus Repository VM**
- **Code Repository VM**
- **CI/CD Pipeline Runner VM**

---

## 1. Infrastructure VM

| Environment   | vCPU | RAM   | HDD   | OS      | Location |
|---------------|------|-------|-------|---------|----------|
| Development   | 2    | 4 GB  | 50 GB | Ubuntu  | Iran     |
| Staging       | 2    | 6 GB  | 75 GB | Ubuntu  | Iran     |
| Production    | 4    | 8 GB  | 100 GB| Ubuntu  | Iran     |

**Services:**

- SSH (all environments)
- Database such as SQL Server/MongoDB/Elasticsearch/Redis (all environments)
- Bus service such as Apache Kafka (all environments)
- Nginx

## 2. Service VM

| Environment   | vCPU | RAM   | HDD   | OS      | Location |
|---------------|------|-------|-------|---------|----------|
| Development   | 2    | 4 GB  | 50 GB | Ubuntu  | Iran     |
| Staging       | 2    | 6 GB  | 75 GB | Ubuntu  | Iran     |
| Production    | 4    | 8 GB  | 100 GB| Ubuntu  | Iran     |

**Services:**

- Docker (all environments)
- Docker Orchestrator such as Swarm/Kubernetes (all environments)
- SSH (all environments)
- Backend services

## 3. Nexus Repository VM (shared in products)

| Environment   | vCPU | RAM   | HDD    | OS      | Location      |
|---------------|------|-------|--------|---------|---------------|
|shared for envs| 4    | 8 GB  | 200 GB | Ubuntu  |Foreign country|

**Services:**

- Java 11+ (all environments)
- Nexus repository services
- Docker registry
- SSH

## 4. Code Repository VM (shared in products)

| Environment   | vCPU | RAM   | HDD    | OS      | Location |
|---------------|------|-------|--------|---------|----------|
|shared for envs| 4    | 8 GB  | 100 GB | Ubuntu  | Iran     |

**Services:**

- Docker
- SSH
- Self-hosted Microsoft Azure/GitLab

## 5. CI/CD Pipeline Runner VM (shared in products)

| Environment   | vCPU | RAM   | HDD   | OS      | Location |
|---------------|------|-------|-------|---------|----------|
|shared for envs| 4    | 6 GB  | 50 GB | Ubuntu  | Iran     |

**Services:**

- GitLab runner/Azure Pipeline
- Docker
- SSH
