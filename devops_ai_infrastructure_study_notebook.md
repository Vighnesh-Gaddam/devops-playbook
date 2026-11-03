# DevOps & AI Infrastructure — Study Notebook

**60-Day Learning Roadmap | Theory + Practical + Interview Preparation**

> Use this as a topic checklist. Mark each item as you study it, practise it, and revise it.

---

# 60-Day Study Timeline

| Phase | Days | Focus |
|---|---:|---|
| Phase 1 — Foundations | 1–20 | SDLC, OS, Linux, scripting, networking, Git, Python, Docker and cloud basics |
| Phase 2 — Core DevOps | 21–40 | Kubernetes, CI/CD, GitOps, Terraform, monitoring and an end-to-end project |
| Phase 3 — AI Infrastructure | 41–50 | GPU, CUDA, model serving, inference, distributed storage, MLOps and LLMOps |
| Phase 4 — System Design | 51–60 | Scalability, caching, load balancing, databases, queues and architecture diagrams |

---

## Table of Contents

1. [Computer Fundamentals](#1-computer-fundamentals)
2. [Operating Systems (OS)](#2-operating-systems-os)
3. [Virtualization & Containers](#3-virtualization--containers)
4. [SDLC & Agentic SDLC](#4-sdlc--agentic-sdlc)
5. [Linux Fundamentals](#5-linux-fundamentals)
6. [Shell Scripting](#6-shell-scripting)
7. [Computer Networking](#7-computer-networking)
8. [Git & GitHub](#8-git--github)
9. [Python for Automation](#9-python-for-automation)
10. [Docker](#10-docker)
11. [Cloud Computing (AWS / Azure / GCP)](#11-cloud-computing-aws--azure--gcp)
12. [Kubernetes](#12-kubernetes)
13. [CI/CD](#13-cicd)
14. [Infrastructure as Code (IaC)](#14-infrastructure-as-code-iac)
15. [GitOps](#15-gitops)
16. [Monitoring & Observability](#16-monitoring--observability)
17. [AI Infrastructure](#17-ai-infrastructure)
18. [System Design](#18-system-design)
19. [60-Day Study Timeline](#60-day-study-timeline)
20. [Notebook Format for Every Topic](#notebook-format-for-every-topic)
21. [Connect DevOps Concepts to Full-Stack Development](#connect-devops-concepts-to-full-stack-development)

---

## 1. Computer Fundamentals

- [ ] What is a computer?
- [ ] Hardware vs. software
- [ ] Input and output devices
- [ ] CPU (Central Processing Unit)
- [ ] ALU and Control Unit
- [ ] CPU cores and threads
- [ ] RAM (Random Access Memory)
- [ ] ROM (Read-Only Memory)
- [ ] Cache memory (L1, L2, L3)
- [ ] HDD vs. SSD
- [ ] Primary vs. secondary memory
- [ ] 32-bit vs. 64-bit architecture
- [ ] BIOS and UEFI
- [ ] Booting process
- [ ] Motherboard and its components

## 2. Operating Systems (OS)

### Fundamentals
- [ ] What is an operating system?
- [ ] Why do we need an OS?
- [ ] Types of operating systems
- [ ] OS architecture
- [ ] Kernel and shell
- [ ] User mode vs. kernel mode
- [ ] System calls
- [ ] Hardware resource management
- [ ] Process management
- [ ] Memory management
- [ ] File-system management
- [ ] Device management

### Important concepts

| Topic | What to understand |
|---|---|
| Process | A program currently in execution |
| Thread | A unit of CPU execution within a process |
| RAM | Temporary working memory |
| Virtual memory | Disk-backed extension of available memory |
| Paging | Dividing memory into fixed-size pages |
| Segmentation | Dividing memory into logical segments |
| Context switching | Switching CPU execution between processes or threads |
| Scheduling | Deciding which process gets CPU time |
| Deadlock | Processes waiting indefinitely for resources |
| Interrupt | A signal that requires CPU attention |
| Hypervisor | Software layer that manages virtual machines |
| Virtual machine (VM) | A software-based computer that runs an operating system |

### Process management
- [ ] Process vs. program
- [ ] Process states
- [ ] Process Control Block (PCB)
- [ ] Process scheduling
- [ ] FCFS, SJF and Round Robin
- [ ] Multitasking vs. multiprocessing
- [ ] Multithreading
- [ ] Inter-process communication (IPC)
- [ ] Mutex and semaphore
- [ ] Race conditions
- [ ] Deadlocks

### Memory management
- [ ] RAM and virtual memory
- [ ] Paging and segmentation
- [ ] Page fault
- [ ] Page-replacement algorithms
- [ ] Thrashing
- [ ] Stack vs. heap
- [ ] Memory allocation
- [ ] Cache memory

## 3. Virtualization & Containers

- [ ] What is virtualization?
- [ ] Why is virtualization used?
- [ ] Physical machine vs. virtual machine
- [ ] Hypervisor
- [ ] Type 1 vs. Type 2 hypervisors
- [ ] VMware, VirtualBox and KVM
- [ ] What is a container?
- [ ] VM vs. container
- [ ] Docker architecture
- [ ] Container runtime
- [ ] Container isolation
- [ ] Namespaces and cgroups
- [ ] Container images

## 4. SDLC & Agentic SDLC

- [ ] What is SDLC?
- [ ] Planning
- [ ] Requirement gathering
- [ ] System design
- [ ] Development
- [ ] Testing
- [ ] Deployment
- [ ] Maintenance
- [ ] Waterfall vs. Agile
- [ ] Scrum and Kanban
- [ ] What is Agentic SDLC?
- [ ] AI agents in software development
- [ ] AI-assisted testing and deployment

## 5. Linux Fundamentals

### Core concepts
- [ ] What is Linux?
- [ ] Linux architecture
- [ ] Linux kernel
- [ ] Linux distributions
- [ ] Linux file-system hierarchy
- [ ] Root directory (`/`)
- [ ] Absolute vs. relative paths
- [ ] File permissions
- [ ] Users and groups
- [ ] Root user and `sudo`
- [ ] Environment variables
- [ ] Package managers

### Commands to practise

| Category | Commands |
|---|---|
| Navigation | `pwd`, `ls`, `cd` |
| Files | `touch`, `cat`, `less`, `nano` |
| Directories | `mkdir`, `rmdir` |
| File operations | `cp`, `mv`, `rm` |
| Permissions | `chmod`, `chown` |
| Processes | `ps`, `top`, `kill`, `htop` |
| Storage | `df`, `du`, `lsblk` |
| Networking | `ping`, `curl`, `wget`, `ss` |
| Search | `grep`, `find`, `locate` |
| System | `uname`, `free`, `uptime` |
| Services | `systemctl`, `journalctl` |

## 6. Shell Scripting

- [ ] What is a shell?
- [ ] Bash vs. shell
- [ ] Variables
- [ ] Data types
- [ ] User input
- [ ] Conditional statements
- [ ] Loops
- [ ] Functions
- [ ] Arrays
- [ ] Command-line arguments
- [ ] Exit status
- [ ] Pipes and redirection
- [ ] Cron jobs
- [ ] Automating tasks

## 7. Computer Networking

### Fundamentals
- [ ] What is computer networking?
- [ ] LAN, WAN and MAN
- [ ] Client-server architecture
- [ ] IP address
- [ ] IPv4 vs. IPv6
- [ ] Public vs. private IP
- [ ] MAC address
- [ ] Subnet mask
- [ ] Default gateway
- [ ] DNS
- [ ] DHCP
- [ ] NAT

### Networking models
- [ ] OSI model (7 layers)
- [ ] TCP/IP model
- [ ] TCP vs. UDP
- [ ] Encapsulation and decapsulation
- [ ] HTTP vs. HTTPS
- [ ] SSL/TLS

### Important protocols and ports

| Protocol | Port | Purpose |
|---|---:|---|
| HTTP | 80 | Web communication |
| HTTPS | 443 | Secure web communication |
| SSH | 22 | Remote access |
| FTP | 21 | File transfer |
| DNS | 53 | Domain resolution |
| SMTP | 25 | Email transfer |
| DHCP | 67/68 | IP assignment |
| MySQL | 3306 | Database communication |
| PostgreSQL | 5432 | Database communication |

### Advanced concepts
- [ ] Three-way handshake
- [ ] Four-way termination
- [ ] Load balancing
- [ ] Reverse proxy
- [ ] Forward proxy
- [ ] Firewall
- [ ] CDN
- [ ] Socket
- [ ] WebSocket

## 8. Git & GitHub

- [ ] What is version control?
- [ ] Git vs. GitHub
- [ ] Repository
- [ ] Working directory
- [ ] Staging area
- [ ] Commit
- [ ] Branching
- [ ] Merging
- [ ] Merge conflicts
- [ ] Rebase
- [ ] Pull requests
- [ ] Git workflow
- [ ] `.gitignore`
- [ ] GitHub Actions basics

## 9. Python for Automation

- [ ] Variables and data types
- [ ] Lists, tuples, sets and dictionaries
- [ ] Conditions and loops
- [ ] Functions
- [ ] File handling
- [ ] Exception handling
- [ ] Modules and packages
- [ ] `os` module
- [ ] `subprocess` module
- [ ] Requests library
- [ ] JSON handling
- [ ] API automation
- [ ] Basic automation scripts

## 10. Docker

- [ ] What is Docker?
- [ ] Why Docker?
- [ ] Docker architecture
- [ ] Docker Engine
- [ ] Docker client
- [ ] Docker daemon
- [ ] Docker images
- [ ] Docker containers
- [ ] Dockerfile
- [ ] Docker Hub
- [ ] Docker volumes
- [ ] Docker networks
- [ ] Docker Compose
- [ ] Container lifecycle
- [ ] Multi-stage builds
- [ ] Image optimization
- [ ] Docker security

## 11. Cloud Computing (AWS / Azure / GCP)

### Fundamentals
- [ ] What is cloud computing?
- [ ] On-premises vs. cloud
- [ ] Public, private and hybrid cloud
- [ ] IaaS, PaaS and SaaS
- [ ] Scalability vs. elasticity
- [ ] High availability
- [ ] Fault tolerance
- [ ] Regions and availability zones

### Core cloud services
- [ ] Compute — EC2, Virtual Machines
- [ ] Storage — S3, Blob Storage
- [ ] Databases — RDS, DynamoDB
- [ ] Networking — VPC, subnets
- [ ] IAM — Identity and Access Management
- [ ] Security groups and firewalls
- [ ] Load balancers
- [ ] Auto Scaling
- [ ] Monitoring
- [ ] Cloud billing

## 12. Kubernetes

- [ ] What is Kubernetes?
- [ ] Why Kubernetes?
- [ ] Kubernetes architecture
- [ ] Control plane
- [ ] Worker nodes
- [ ] Pods
- [ ] Deployments
- [ ] ReplicaSets
- [ ] Services
- [ ] ClusterIP, NodePort and LoadBalancer
- [ ] Ingress
- [ ] ConfigMaps
- [ ] Secrets
- [ ] Namespaces
- [ ] Persistent Volumes
- [ ] Persistent Volume Claims
- [ ] StatefulSets
- [ ] DaemonSets
- [ ] Jobs and CronJobs
- [ ] `kubectl` commands
- [ ] Helm basics

## 13. CI/CD

- [ ] What is Continuous Integration (CI)?
- [ ] What is Continuous Delivery / Deployment (CD)?
- [ ] Continuous Delivery vs. Continuous Deployment
- [ ] CI/CD pipeline
- [ ] Build stage
- [ ] Testing stage
- [ ] Deployment stage
- [ ] GitHub Actions
- [ ] GitLab CI/CD
- [ ] Jenkins basics
- [ ] Pipeline YAML
- [ ] Environment variables
- [ ] Secrets management
- [ ] Automated testing

## 14. Infrastructure as Code (IaC)

- [ ] What is Infrastructure as Code?
- [ ] Declarative vs. imperative
- [ ] Terraform
- [ ] Terraform providers
- [ ] Resources
- [ ] Variables
- [ ] Outputs
- [ ] State files
- [ ] Modules
- [ ] `terraform init`
- [ ] `terraform plan`
- [ ] `terraform apply`
- [ ] `terraform destroy`

## 15. GitOps

- [ ] What is GitOps?
- [ ] Git as the single source of truth
- [ ] Push vs. pull deployment
- [ ] Reconciliation loop
- [ ] Desired vs. actual state
- [ ] Argo CD
- [ ] Flux
- [ ] GitOps with Kubernetes

## 16. Monitoring & Observability

- [ ] What is monitoring?
- [ ] What is observability?
- [ ] Logs
- [ ] Metrics
- [ ] Traces
- [ ] CPU monitoring
- [ ] Memory monitoring
- [ ] Network monitoring
- [ ] System health
- [ ] Prometheus
- [ ] Grafana
- [ ] Alerting
- [ ] Dashboards

## 17. AI Infrastructure

- [ ] What is AI infrastructure?
- [ ] CPU vs. GPU
- [ ] GPU architecture
- [ ] CUDA
- [ ] GPU memory management
- [ ] AI networking
- [ ] RDMA
- [ ] Distributed storage
- [ ] Object vs. file vs. block storage
- [ ] Model serving
- [ ] Model inference
- [ ] Inference engines
- [ ] Kubernetes for AI workloads
- [ ] Ray and Slurm
- [ ] Model quantization
- [ ] Batching
- [ ] KV cache
- [ ] GPU utilization
- [ ] MLOps
- [ ] LLMOps
- [ ] Model evaluation
- [ ] Model deployment
- [ ] AI infrastructure security

## 18. System Design

- [ ] What is system design?
- [ ] Functional requirements
- [ ] Non-functional requirements
- [ ] Scalability
- [ ] Vertical vs. horizontal scaling
- [ ] Load balancing
- [ ] Caching
- [ ] CDN
- [ ] Database indexing
- [ ] SQL vs. NoSQL
- [ ] Database replication
- [ ] Database sharding
- [ ] Message queues
- [ ] Rate limiting
- [ ] Microservices
- [ ] Monolithic architecture
- [ ] API gateway
- [ ] Fault tolerance
- [ ] High availability
- [ ] CAP theorem
- [ ] Architecture diagrams

---

# Notebook Format for Every Topic

Use this structure when writing detailed notes for an individual concept.

## Example: Process in Operating System

### 📌 Definition
A process is a program that is currently being executed.

### ⭐ Why do we need it?
To manage and execute multiple programs efficiently.

### 📝 Important Concepts
- Process states
- Process Control Block (PCB)
- Process scheduling
- Context switching

### 📂 Example
Opening Chrome creates a process. Opening multiple tabs may create additional processes or threads.

### ⚠️ Important Points
- Every process has its own virtual address space.
- A process can contain multiple threads.

### 🎯 Interview Questions
1. What is a process?
2. Process vs. thread?
3. What is context switching?
4. What is a deadlock?

### 🧠 Memory Trick
Program = Instructions. Process = Running program.

---

# Connect DevOps Concepts to Full-Stack Development

| Full-stack experience | DevOps concept |
|---|---|
| React application | Docker container |
| Node.js server | Linux process |
| PostgreSQL | Cloud database |
| API requests | Networking |
| Vercel deployment | CI/CD concepts |
| Multiple server instances | Load balancing |

**Study advice:** This is a comprehensive topic checklist, not a promise that every topic can be mastered in 60 days. Prioritize OS, Linux, networking, Docker, cloud and Kubernetes first. Connect each concept to practical work instead of memorizing definitions alone.
