# Virtual Machines Requirements

This document outlines the virtual machine (VM) requirements for development, staging, and production environments, including infrastructure and service VMs.

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

| Environment   | vCPU | RAM   | HDD   | OS      |
|---------------|------|-------|-------|---------|
| Development   | 2    | 4 GB  | 50 GB | Ubuntu  |
| Staging       | 2    | 6 GB  | 75 GB | Ubuntu  |
| Production    | 4    | 8 GB  | 100 GB| Ubuntu  |

**Service:**

- SSH (all environments)
- Database like as SQL Servier/MongoDb/Elastic Search/Redis (all environments)
- Bus service such as Apache Kafka/ (all environments)
- Nginx

## 2. Service VM

| Environment   | vCPU | RAM   | HDD   | OS      |
|---------------|------|-------|-------|---------|
| Development   | 2    | 4 GB  | 50 GB | Ubuntu  |
| Staging       | 2    | 6 GB  | 75 GB | Ubuntu  |
| Production    | 4    | 8 GB  | 100 GB| Ubuntu  |

**Service:**

- Docker (all environments)
- Docker Orcasrator such as Swarm/Kuberneties (all environments)
- SSH (all environments)
- Backend services

## 3. Nexus Repository VM (shared in products)

| Environment   | vCPU | RAM   | HDD    | OS      |
|---------------|------|-------|--------|---------|
|shared for envs| 4    | 8 GB  | 200 GB | Ubuntu  |

**Service:**

- Java 11+ (all environments)
- Nexus repository services
- Docker registry
- SSH

## 4. Code Repository VM (shared in products)

| Environment   | vCPU | RAM   | HDD    | OS      |
|---------------|------|-------|--------|---------|
|shared for envs| 4    | 8 GB  | 100 GB | Ubuntu  |

**Service:**

- Docker
- SSH
- Self hosted Microsft Azur/GitLab

## 5. CI/CD Pipeline Runner VM (shared in products)

| Environment   | vCPU | RAM   | HDD   | OS      |
|---------------|------|-------|-------|---------|
|shared for envs| 4    | 6 GB  | 50 GB | Ubuntu  |

**Service:**

- Gitlap runner/Azur Pipelin
- Docker
- SSH

**Note:** Adjust resources based on workload and scaling needs.
