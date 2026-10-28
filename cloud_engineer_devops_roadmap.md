# Cloud Engineer + DevOps Roadmap

**Goal:** Become job-ready for entry-level Cloud Engineer, AWS Cloud
Engineer, Junior DevOps Engineer, or Cloud Support roles.\
**Starting point:** MCA student with web-development/full-stack
experience.\
**Plan length:** 9--12 months at 1--2 focused hours/day; extend it if
college or job responsibilities require it.\
**Primary cloud:** AWS. Learn one cloud deeply before adding Azure or
Google Cloud.

> \[!IMPORTANT\] This roadmap is a plan, not a guarantee of a job or
> salary. Certifications can help demonstrate knowledge, but projects,
> troubleshooting ability, communication, and interview performance
> matter too. Do not collect certifications without building and
> explaining real projects.

------------------------------------------------------------------------

## 1. Define the destination

### Main target

By the end, you should be able to:

-   Explain networking, Linux, virtualization, cloud computing, and
    shared responsibility.
-   Deploy a web application to AWS with a database, secure access,
    HTTPS, logs, monitoring, backups, and documented architecture.
-   Use Git, Docker, Terraform, and a CI/CD pipeline.
-   Diagnose common application, networking, permissions, deployment,
    and cost issues.
-   Explain design choices and trade-offs in an interview.
-   Show two or three useful cloud projects on GitHub and your resume.

### Roles to search for

-   Junior Cloud Engineer
-   AWS Cloud Support Associate / Cloud Support Engineer
-   Cloud Operations Engineer
-   Junior DevOps Engineer
-   Infrastructure / Systems Engineer (cloud-focused)
-   Platform Engineering Intern (where suitable)

Do not assume every role has the same requirements. Read 20--30 current
job descriptions in your target market and record recurring skills.

### Goal-setting template

Fill this in before starting:

-   **Target role:** `Junior Cloud Engineer / Junior DevOps Engineer`
-   **Target application date:** `YYYY-MM-DD`
-   **Daily study time:** `___ minutes`
-   **Study days per week:** `___`
-   **Weekly lab target:** `___`
-   **Certification budget:** `₹___`
-   **Cloud spending limit:** `₹___ per month`
-   **Weekly review day:** `___`
-   **GitHub repository:** `cloud-engineering-roadmap`
-   **Progress dashboard:** `Notion / Obsidian / GitHub Projects`

------------------------------------------------------------------------

## 2. Recommended learning sequence

  ------------------------------------------------------------------------
  Phase                           Suggested duration Finish line
  --------------------- ---------------------------- ---------------------
  0\. Setup and career                        1 week Goals, accounts,
  research                                           tracker,
                                                     job-description
                                                     checklist

  1\. Computer networks                   4--6 weeks Explain and practise
  and Linux                                          core networking/Linux
                                                     tasks

  2\. Git, scripting,                     2--3 weeks Git workflow, basic
  and cloud concepts                                 Bash/Python, cloud
                                                     fundamentals

  3\. AWS fundamentals                    6--8 weeks Deploy and secure a
  and core services                                  basic application

  4\. Projects and AWS                    3--5 weeks One polished project;
  certification                                      take an exam only
  preparation                                        when ready

  5\. Docker, CI/CD,                      6--8 weeks Reproducible
  and Terraform                                      deployment pipeline

  6\. Monitoring,                         4--6 weeks Operate and
  security,                                          troubleshoot the
  reliability, and cost                              deployment

  7\. Kubernetes and                      4--8 weeks Deploy a small
  advanced topics                                    containerized
                                                     application to
                                                     Kubernetes

  8\. Portfolio,            Ongoing; focused final 4 Portfolio, resume,
  interviews, and                              weeks interview practice,
  applications                                       applications
  ------------------------------------------------------------------------

These are estimates, not deadlines. If a topic is not understood, spend
more time on labs before moving on.

------------------------------------------------------------------------

# Phase 0 --- Setup and career research

## Checklist

-   [ ] Choose AWS as the first cloud provider.
-   [ ] Create a GitHub repository for notes, diagrams, and lab
    write-ups.
-   [ ] Install VS Code, Git, a terminal, and a Linux environment (WSL2
    on Windows or a Linux VM).
-   [ ] Set up a password manager and enable MFA on important accounts.
-   [ ] Create a weekly tracker with the columns: Date, Topic, Lab,
    Result, Mistake, Next action.
-   [ ] Review at least 20 current job listings for your target role.
-   [ ] Record the skills that appear most often.
-   [ ] Set a cloud budget and learn how to check usage and billing
    before launching resources.

## Weekly routine

A practical 7-hour week could look like this:

-   **2 hours:** course/documentation and notes
-   **3 hours:** hands-on labs
-   **1 hour:** project work
-   **1 hour:** revision, quiz, and weekly review

Prefer hands-on work over watching tutorials passively.

------------------------------------------------------------------------

# Phase 1 --- Networking, Linux, and computing foundations

## 1.1 Networking

Learn the meaning and practical purpose of each:

-   [ ] **IP** --- Internet Protocol; addresses and routes packets
    between networks.
-   [ ] **IPv4 / IPv6** --- two versions of IP addressing.
-   [ ] **Private vs public IP** --- private addresses are used inside
    private networks; public addresses can be routed over the public
    internet.
-   [ ] **CIDR** --- notation for an IP network range,
    e.g. `192.168.1.0/24`.
-   [ ] **Subnet** --- a smaller network range.
-   [ ] **Router** --- forwards traffic between networks.
-   [ ] **Switch** --- connects devices within a local network.
-   [ ] **DNS** --- Domain Name System; resolves names such as
    `example.com` to records including IP addresses.
-   [ ] **DHCP** --- Dynamic Host Configuration Protocol; automatically
    assigns network configuration.
-   [ ] **TCP / UDP** --- transport protocols; TCP provides ordered
    reliable delivery, while UDP is connectionless.
-   [ ] **HTTP / HTTPS** --- web communication protocols; HTTPS protects
    traffic with TLS.
-   [ ] **TLS** --- Transport Layer Security; encrypts and authenticates
    network connections.
-   [ ] **Ports** --- identify services on a host, e.g. 22 for SSH, 80
    for HTTP, 443 for HTTPS; defaults can be changed.
-   [ ] **NAT** --- Network Address Translation.
-   [ ] **VPN** --- Virtual Private Network.
-   [ ] **Firewall** --- controls traffic according to rules.
-   [ ] **Load balancer** --- distributes traffic among targets.
-   [ ] **Latency / bandwidth** --- delay vs data-transfer capacity.

### Commands and tests

Practise these on your own machine:

``` bash
ping example.com
nslookup example.com
traceroute example.com
# On Windows, use: tracert example.com
curl -I https://example.com
ip addr
ip route
```

Some commands may need installation or administrator privileges. A
failed `ping` does not automatically mean a service is down; ICMP may be
blocked.

### Networking checkpoint

You are ready to continue when you can explain what happens when you
enter a website URL into a browser, including DNS lookup, routing,
TCP/TLS, HTTP, and the server response.

## 1.2 Linux

Learn: - \[ \] Filesystem structure and absolute/relative paths - \[ \]
Files and directories: `ls`, `pwd`, `cd`, `mkdir`, `cp`, `mv`, `rm`,
`touch` - \[ \] Reading files: `cat`, `less`, `head`, `tail` - \[ \]
Searching: `grep`, `find` - \[ \] Permissions and ownership: `chmod`,
`chown`, `sudo` - \[ \] Processes: `ps`, `top`, `kill` - \[ \] Disk and
memory: `df -h`, `du -sh`, `free -h` - \[ \] Networking: `curl`, `ss`,
`ip` - \[ \] Package managers such as `apt` - \[ \] Services and logs:
`systemctl`, `journalctl` - \[ \] Environment variables, pipes,
redirection, exit codes - \[ \] SSH keys and remote access - \[ \] Basic
Bash scripting

### Mini-labs

-   [ ] Create folders and organise a project directory.
-   [ ] Find a word inside multiple log files with `grep`.
-   [ ] Identify a running process and inspect its resource use.
-   [ ] Start a simple web server and test its port.
-   [ ] Create a script that checks disk usage and prints a warning.
-   [ ] Connect to a Linux machine using SSH in a safe lab environment.

## 1.3 Virtualization and operating systems

-   [ ] Understand physical machines vs virtual machines (VMs).
-   [ ] Learn CPU, RAM, storage, processes, and filesystems.
-   [ ] Understand a hypervisor and why multiple VMs can share a
    physical host.
-   [ ] Distinguish a VM from a container.
-   [ ] Learn the basics of Windows and Linux server administration.

### Free/low-cost learning starting points

-   [ ] [Cisco Networking Academy](https://www.netacad.com/)
-   [ ] [freeCodeCamp](https://www.freecodecamp.org/)
-   [ ] [Linux Journey](https://linuxjourney.com/)
-   [ ] [OverTheWire: Bandit](https://overthewire.org/wargames/bandit/)
-   [ ] [TryHackMe](https://tryhackme.com/) --- use beginner
    Linux/networking rooms and check current free access.
-   [ ] [Ubuntu documentation](https://documentation.ubuntu.com/)

------------------------------------------------------------------------

# Phase 2 --- Git, scripting, and cloud concepts

## 2.1 Git and GitHub

-   [ ] `git init`, `git clone`, `git status`
-   [ ] `git add`, `git commit`, `git log`
-   [ ] Branches, merges, pull requests, and conflict resolution
-   [ ] `.gitignore`
-   [ ] README files and Markdown
-   [ ] Never commit API keys, passwords, private keys, or cloud
    credentials.

## 2.2 Scripting

Pick one scripting language to start: - **Bash** for Linux automation. -
**Python** for scripts, APIs, and automation.

Practise: - \[ \] Variables, conditions, loops, functions - \[ \]
Reading files and parsing text/JSON - \[ \] Calling an HTTP API - \[ \]
Handling errors and exit codes - \[ \] Logging and command-line
arguments

You do not need to become an advanced software engineer before starting
cloud labs, but you should be comfortable reading and modifying scripts.

## 2.3 Cloud concepts

-   [ ] **Cloud computing** --- on-demand access to computing resources
    over a network.
-   [ ] **IaaS** --- Infrastructure as a Service; virtual machines,
    networks, and storage.
-   [ ] **PaaS** --- Platform as a Service; managed platforms for
    deploying applications.
-   [ ] **SaaS** --- Software as a Service; ready-to-use software
    delivered online.
-   [ ] **Public, private, hybrid cloud**
-   [ ] **Region / Availability Zone (AZ)** --- geographic area vs
    isolated datacenter grouping within a region.
-   [ ] **Scalability / elasticity** --- ability to handle growth vs
    adjust resources as demand changes.
-   [ ] **High availability (HA)** --- designing to minimise downtime.
-   [ ] **Fault tolerance** --- continuing to operate despite certain
    failures.
-   [ ] **Shared responsibility model** --- provider and customer have
    different security responsibilities.
-   [ ] **CapEx / OpEx** --- capital expenditure vs operating
    expenditure.
-   [ ] **Pay-as-you-go** --- usage-based billing.
-   [ ] **RTO / RPO** --- recovery time objective and recovery point
    objective.

### Checkpoint

Explain the difference between a region and an AZ, IaaS and SaaS,
scalability and elasticity, and what the cloud provider does versus what
the customer must secure.

------------------------------------------------------------------------

# Phase 3 --- AWS fundamentals and core services

AWS means **Amazon Web Services**. Start with one cloud provider and
build transferable skills before exploring multiple clouds.

## 3.1 Account safety before launching resources

-   [ ] Enable MFA on the root user.
-   [ ] Avoid using the root account for everyday work.
-   [ ] Use IAM roles and least-privilege permissions where appropriate.
-   [ ] Configure billing alerts/budgets and review the current
    free-tier terms.
-   [ ] Learn how to find resources in every region you use.
-   [ ] Delete lab resources after each exercise.
-   [ ] Never publish access keys or credentials in GitHub.
-   [ ] Do not assume a service is free because a tutorial calls it
    "free tier."

**Cost rule:** Set a small monthly budget and check the billing
dashboard frequently. Budgets and alerts can notify you; they do not
necessarily stop every charge. Public IPv4 addresses, storage,
snapshots, logs, data transfer, NAT gateways, load balancers, and other
resources may incur costs. Check current prices before deploying.

## 3.2 Core AWS services

  --------------------------------------------------------------------------
  Service /         Full name         What it is for    Practical goal
  abbreviation                                          
  ----------------- ----------------- ----------------- --------------------
  EC2               Elastic Compute   Virtual servers   Launch and secure a
                    Cloud                               Linux VM

  S3                Simple Storage    Object/file       Host files and
                    Service           storage           understand bucket
                                                        permissions

  IAM               Identity and      Users, roles,     Apply least
                    Access Management policies,         privilege
                                      permissions       

  VPC               Virtual Private   Isolated virtual  Understand subnets
                    Cloud             network           and routing

  AZ                Availability Zone Isolated location Explain availability
                                      within a region   design

  EBS               Elastic Block     Block storage for Attach and manage a
                    Store             EC2               volume

  EFS               Elastic File      Managed shared    Understand shared
                    System            file storage      filesystem use cases

  RDS               Relational        Managed           Connect an app to a
                    Database Service  relational        database securely
                                      databases         

  DynamoDB          ---               Managed NoSQL     Understand
                                      database          key-value/document
                                                        use cases

  Route 53          ---               DNS and domain    Understand hosted
                                      routing           zones and records

  CloudFront        ---               Content delivery  Cache and deliver
                                      network (CDN)     static content

  ALB               Application Load  HTTP/HTTPS load   Understand health
                    Balancer          balancing         checks and target
                                                        groups

  Auto Scaling      ---               Adjust capacity   Understand scaling
                                      automatically     policies

  CloudWatch        ---               Metrics, logs,    Inspect logs and
                                      alarms            create an alarm

  CloudTrail        ---               API/account       Understand auditing
                                      activity history  

  SSM               Systems Manager   Fleet and         Learn secure
                                      operations        instance management
                                      management        

  KMS               Key Management    Encryption key    Understand
                    Service           management        encryption at rest

  ACM               AWS Certificate   TLS certificates  Understand HTTPS
                    Manager                             certificates

  Lambda            ---               Serverless        Run code without
                                      compute           managing a server

  SQS               Simple Queue      Managed message   Understand
                    Service           queue             asynchronous
                                                        processing

  SNS               Simple            Pub/sub           Understand event
                    Notification      notifications     notifications
                    Service                             

  ECR               Elastic Container Container image   Store Docker images
                    Registry          registry          

  ECS               Elastic Container Container         Run a containerised
                    Service           orchestration     service

  EKS               Elastic           Managed           Advanced container
                    Kubernetes        Kubernetes        orchestration
                    Service                             

  CloudFormation    ---               Infrastructure as Understand
                                      code (AWS-native) declarative
                                                        infrastructure
  --------------------------------------------------------------------------

## 3.3 Hands-on labs in order

-   [ ] Create an IAM identity/role safely and explain its permissions.
-   [ ] Launch a small EC2 Linux instance using a safe access method.
-   [ ] Connect to it and install a simple web server.
-   [ ] Configure inbound rules narrowly; do not expose unnecessary
    ports.
-   [ ] Create an S3 bucket, upload a file, and understand public access
    blocking.
-   [ ] Host static assets safely or serve them through an appropriate
    managed service.
-   [ ] Create a VPC diagram with public/private subnets and route
    tables.
-   [ ] Learn security groups and network ACLs.
-   [ ] Review CloudWatch metrics/logs and create a basic alarm.
-   [ ] Explain how a domain resolves to a deployed application.
-   [ ] Learn how to terminate/delete the resources after the lab.

### First project: Deploy a web application

Use a small app you already understand.

**Possible architecture:** - Static frontend hosted through an
appropriate static hosting service. - Backend on a small EC2 instance or
a managed compute service. - Database kept private and not exposed
directly to the public internet. - HTTPS for public traffic. - IAM roles
instead of hard-coded keys. - Logs and basic monitoring. - README with
architecture diagram, deployment steps, security notes, and cost cleanup
instructions.

Start with the simplest architecture that teaches the concepts. You do
not need every AWS service in the first project.

------------------------------------------------------------------------

# Phase 4 --- Certification decision and preparation

## Certification strategy

**Recommended first serious technical certification:** AWS Certified
Solutions Architect -- Associate (SAA-C03), after hands-on AWS
fundamentals.\
**Optional beginner credential:** AWS Certified Cloud Practitioner
(CLF-C02) if you need structured fundamentals or want a first exam
experience.

The beginner certificate is not compulsory. If you already understand
basic IT concepts, you may study its syllabus without paying for the
exam and invest the money in the associate exam or hands-on learning
instead.

### Current certification options (verify before paying)

  ------------------------------------------------------------------------
  Certification    Level / focus    When it makes       Published exam fee
                                    sense            
  ---------------- ---------------- ---------------- ---------------------
  AWS Certified    Foundational     Optional          USD \$100; AWS lists
  Cloud            AWS/cloud        beginner                    ₹8,553 for
  Practitioner     knowledge        checkpoint       foundational exams in
  (CLF-C02)                                            its current pricing
                                                         table, before any
                                                                applicable
                                                          taxes/conditions

  AWS Certified    Designing        Recommended       USD \$150; AWS lists
  Solutions        secure,          primary AWS             ₹12,829.50 for
  Architect --     resilient,       certification       associate exams in
  Associate        cost-aware AWS   after practice     its current pricing
  (SAA-C03)        architectures                         table, before any
                                                                applicable
                                                          taxes/conditions

  Microsoft        Azure/cloud      Optional if       Microsoft India page
  Certified: Azure fundamentals     target employers       currently lists
  Fundamentals                      use Azure                       ₹3,691
  (AZ-900)                                           

  Microsoft        Azure            If pursuing       Microsoft page lists
  Certified: Azure administration   Azure              USD \$165; regional
  Administrator                     administrator             price varies
  Associate                         roles            
  (AZ-104)                                           

  Google Cloud     Deploying,       Choose if target        USD \$125 plus
  Associate Cloud  operating, and   roles use GCP           applicable tax
  Engineer         securing GCP                      
                   workloads                         

  Google Cloud     Advanced cloud   Later, after            USD \$200 plus
  Professional     architecture     substantial GCP         applicable tax
  Cloud Architect                   experience       
  ------------------------------------------------------------------------

Official pages: - [AWS Cloud
Practitioner](https://aws.amazon.com/certification/certified-cloud-practitioner/) -
[AWS Solutions Architect --
Associate](https://aws.amazon.com/certification/certified-solutions-architect-associate/) -
[AWS exam
pricing](https://aws.amazon.com/certification/policies/before-testing/) -
[Azure Fundamentals
AZ-900](https://learn.microsoft.com/en-in/credentials/certifications/azure-fundamentals/) -
[Azure Administrator
AZ-104](https://learn.microsoft.com/en-us/credentials/certifications/azure-administrator/) -
[Google Cloud Associate Cloud
Engineer](https://cloud.google.com/learn/certification/cloud-engineer) -
[Google Cloud Professional Cloud
Architect](https://cloud.google.com/learn/certification/cloud-architect)

Fees, exam codes, regional pricing, and exam objectives can change.
Confirm the official page before booking. Avoid relying on an old video
for current prices.

## AWS exam readiness checklist

Do not book the exam just because you finished a playlist.

-   [ ] Read the official exam guide and all domains.
-   [ ] Complete hands-on labs for the major services in the syllabus.
-   [ ] Explain why you would choose one service over another.
-   [ ] Complete several timed practice exams from reputable sources.
-   [ ] Review every incorrect answer and understand why the other
    options are wrong.
-   [ ] Score consistently around 80--85% or better on fresh practice
    sets as a personal readiness target, not an official passing-score
    guarantee.
-   [ ] Check the exam format, policies, language, price, and delivery
    options.
-   [ ] Schedule the exam only when ready.

Use official learning material first. Third-party courses and practice
exams can supplement it; do not treat any practice-question dump as a
substitute for understanding.

------------------------------------------------------------------------

# Phase 5 --- Core DevOps skills

## 5.1 Docker

Docker packages an application and its dependencies into containers.

Learn: - \[ \] Image vs container - \[ \] `Dockerfile` - \[ \] Build,
run, stop, and remove containers - \[ \] Ports and environment
variables - \[ \] Volumes and persistent data - \[ \] Docker networks -
\[ \] Docker Compose - \[ \] Image tags and registries - \[ \] Container
logs and troubleshooting - \[ \] Secrets: do not bake credentials into
images.

### Lab

-   [ ] Containerise a small backend.
-   [ ] Run the app and its database locally using Docker Compose.
-   [ ] Persist database data using a volume.
-   [ ] Write clear build/run instructions in the README.

## 5.2 CI/CD

-   **CI --- Continuous Integration:** frequently merge changes and
    automatically build/test them.
-   **CD --- Continuous Delivery or Continuous Deployment:** automate
    the path from a validated change toward release; the exact meaning
    depends on the team.
-   [ ] Understand build → test → package → deploy.
-   [ ] Learn GitHub Actions first; then explore Jenkins if job listings
    request it.
-   [ ] Store secrets in the CI/CD platform's secret store.
-   [ ] Add linting/tests to a project.
-   [ ] Deploy a test/staging build automatically.
-   [ ] Understand approvals and rollback.

### Lab

Create a GitHub Actions workflow that runs tests on each pull request
and builds a Docker image after a successful merge.

## 5.3 Terraform / Infrastructure as Code

**IaC --- Infrastructure as Code:** define and manage infrastructure
using files instead of manually creating each resource.

Learn: - \[ \] Providers, resources, variables, outputs - \[ \]
`terraform init`, `plan`, `apply`, `destroy` - \[ \] State files and why
state must be protected - \[ \] Remote state and locking concepts - \[
\] Modules and reusable configuration - \[ \] Secrets and sensitive
values - \[ \] Change review before `apply` - \[ \] Clean up test
resources after use

### Lab

Provision a small, safe AWS environment with Terraform. Keep
configuration in Git, exclude secrets/state files where appropriate,
document costs, and demonstrate that the environment can be recreated
and destroyed.

## 5.4 Configuration and scripting

-   [ ] Write small Bash/Python automation scripts.
-   [ ] Learn YAML and JSON.
-   [ ] Understand environment-specific configuration.
-   [ ] Learn Ansible basics if target jobs request configuration
    management.
-   [ ] Practise reading logs and writing repeatable runbooks.

### Project 2: Automated deployment

Build a pipeline that: 1. Takes code from GitHub. 2. Runs tests. 3.
Builds a Docker image. 4. Publishes the image to a registry. 5. Deploys
to a chosen AWS compute target. 6. Runs a health check. 7. Documents
rollback and cleanup.

------------------------------------------------------------------------

# Phase 6 --- Security, monitoring, reliability, and cost

## Security

-   [ ] Least privilege and IAM roles/policies
-   [ ] MFA and credential hygiene
-   [ ] Security groups and network segmentation
-   [ ] Encryption at rest and in transit
-   [ ] Secrets management
-   [ ] Patch management
-   [ ] Backups and restore testing
-   [ ] Audit trails and logging
-   [ ] Basic threat modelling
-   [ ] Shared responsibility model
-   [ ] Avoid publicly exposing databases or administrative ports.

## Monitoring and troubleshooting

-   [ ] Metrics vs logs vs traces
-   [ ] CloudWatch dashboards, alarms, and logs
-   [ ] CPU, memory, disk, latency, error rates, and availability
-   [ ] Health checks
-   [ ] Incident notes and runbooks
-   [ ] Root-cause analysis: what failed, why, impact, fix, and
    prevention

## Reliability and cost

-   [ ] Multi-AZ concepts
-   [ ] Backups and recovery objectives
-   [ ] Load balancing and scaling
-   [ ] Redundancy vs cost trade-offs
-   [ ] Budgets and billing review
-   [ ] Right-sizing resources
-   [ ] Delete unused resources and snapshots
-   [ ] Understand that "high availability" is a design property, not
    just a checkbox.

### Project 3: Operate and improve

Take one deployed project and: - Add logs and an alert. - Test a failure
safely. - Write a short incident report. - Document backup and restore
steps. - Explain what happens if one component becomes unavailable. -
Record the design's limitations and possible improvements. - Estimate
cost using current AWS pricing tools.

------------------------------------------------------------------------

# Phase 7 --- Kubernetes and advanced cloud topics

Kubernetes is useful for many DevOps/platform roles, but learn it after
Linux, networking, Docker, and basic cloud deployments.

Learn: - \[ \] Cluster, node, and control plane - \[ \] Pod, Deployment,
Service - \[ \] ConfigMap and Secret - \[ \] Ingress and load
balancing - \[ \] Namespaces and resource limits - \[ \] Health probes -
\[ \] Persistent volumes - \[ \] RBAC --- Role-Based Access Control - \[
\] Helm basics - \[ \] Troubleshooting with `kubectl` - \[ \] Managed
Kubernetes concepts (e.g. EKS)

Useful resources: - [Kubernetes
documentation](https://kubernetes.io/docs/home/) - [Docker
documentation](https://docs.docker.com/) - [Terraform
documentation](https://developer.hashicorp.com/terraform/docs) - [GitHub
Actions documentation](https://docs.github.com/actions)

### Kubernetes mini-project

Deploy a small stateless application locally with kind or minikube
first. Add a Deployment, Service, configuration, health checks, and
README. Only then consider a managed cloud cluster, because managed
clusters and related networking resources can incur charges.

------------------------------------------------------------------------

# Phase 8 --- Portfolio and job preparation

## Portfolio standard

Each project should have: - \[ \] A clear problem statement and
architecture diagram - \[ \] A list of services/tools used and why - \[
\] Step-by-step deployment instructions - \[ \] Screenshots or a short
demo - \[ \] Security considerations - \[ \] Monitoring and
troubleshooting notes - \[ \] Cost considerations and cleanup
instructions - \[ \] Known limitations and future improvements - \[ \]
No secrets, private keys, or account identifiers

## Resume bullet formula

Use **action + technology + outcome + evidence**. Never invent traffic
numbers, uptime, cost savings, or users.

Example, only if it accurately describes your work: - "Containerised a
web application with Docker and automated its test/build workflow using
GitHub Actions, documenting repeatable deployment and rollback steps."

## Interview preparation checklist

-   [ ] Explain DNS, TCP vs UDP, HTTP vs HTTPS, CIDR, NAT, routing, and
    ports.
-   [ ] Explain Linux permissions, processes, logs, services, and SSH.
-   [ ] Explain EC2, S3, IAM, VPC, security groups, RDS, CloudWatch, and
    load balancing.
-   [ ] Explain Docker images vs containers.
-   [ ] Explain CI vs CD and a pipeline you built.
-   [ ] Explain Terraform state, plan/apply, and infrastructure drift.
-   [ ] Troubleshoot "website is down," "permission denied," "high CPU,"
    and "deployment failed."
-   [ ] Draw your project architecture from memory.
-   [ ] Explain a mistake you made and how you debugged it.
-   [ ] Practise clear, honest explanations rather than memorised
    definitions alone.

## Application routine

-   [ ] Tailor your resume to each role.
-   [ ] Add relevant projects and verified certifications to LinkedIn.
-   [ ] Apply consistently to roles that match your current skills.
-   [ ] Track company, role, date, link, requirements, status, and
    follow-up.
-   [ ] Ask for feedback and revise your plan every two weeks.
-   [ ] Keep building while applying; do not wait for every advanced
    topic to be complete.

------------------------------------------------------------------------

# 3. Abbreviation glossary

  -----------------------------------------------------------------------
  Abbreviation                        Full form / meaning
  ----------------------------------- -----------------------------------
  AWS                                 Amazon Web Services

  Azure                               Microsoft's cloud platform name

  GCP                                 Google Cloud Platform (commonly
                                      used abbreviation; Google Cloud is
                                      the current brand)

  VM                                  Virtual Machine

  OS                                  Operating System

  IP                                  Internet Protocol

  IPv4 / IPv6                         Internet Protocol versions 4 and 6

  CIDR                                Classless Inter-Domain Routing

  DNS                                 Domain Name System

  DHCP                                Dynamic Host Configuration Protocol

  TCP / UDP                           Transmission Control Protocol /
                                      User Datagram Protocol

  HTTP / HTTPS                        Hypertext Transfer Protocol /
                                      secure HTTP using TLS

  TLS                                 Transport Layer Security

  SSH                                 Secure Shell

  VPN                                 Virtual Private Network

  NAT                                 Network Address Translation

  VPC                                 Virtual Private Cloud

  AZ                                  Availability Zone

  IAM                                 Identity and Access Management

  EC2                                 Elastic Compute Cloud

  S3                                  Simple Storage Service

  EBS                                 Elastic Block Store

  EFS                                 Elastic File System

  RDS                                 Relational Database Service

  ALB                                 Application Load Balancer

  CDN                                 Content Delivery Network

  HA                                  High Availability

  DR                                  Disaster Recovery

  RTO                                 Recovery Time Objective

  RPO                                 Recovery Point Objective

  IAM policy                          Rules defining allowed or denied
                                      actions on resources

  MFA                                 Multi-Factor Authentication

  KMS                                 Key Management Service

  ACM                                 AWS Certificate Manager

  SSM                                 AWS Systems Manager

  IaC                                 Infrastructure as Code

  CI                                  Continuous Integration

  CD                                  Continuous Delivery or Continuous
                                      Deployment

  CD pipeline                         Automated workflow for validated
                                      software release/deployment

  CLI                                 Command-Line Interface

  API                                 Application Programming Interface

  SDK                                 Software Development Kit

  YAML                                Human-readable data-serialization
                                      format often used in configuration

  JSON                                JavaScript Object Notation

  Docker image                        Packaged filesystem/configuration
                                      used to create containers

  Container                           Isolated process environment that
                                      shares the host kernel

  Kubernetes / K8s                    Container orchestration platform;
                                      "K8s" abbreviates Kubernetes

  ECR                                 Elastic Container Registry

  ECS                                 Elastic Container Service

  EKS                                 Elastic Kubernetes Service

  RBAC                                Role-Based Access Control

  SQS                                 Simple Queue Service

  SNS                                 Simple Notification Service

  CDN                                 Content Delivery Network

  CLI                                 Command-Line Interface

  CapEx                               Capital Expenditure

  OpEx                                Operating Expenditure

  SAA-C03                             AWS Certified Solutions Architect
                                      -- Associate exam code

  CLF-C02                             AWS Certified Cloud Practitioner
                                      exam code

  AZ-900                              Microsoft Azure Fundamentals exam
                                      code

  AZ-104                              Microsoft Azure Administrator exam
                                      code

  GCP ACE                             Google Cloud Associate Cloud
                                      Engineer (common shorthand)

  SRE                                 Site Reliability Engineering

  SLA                                 Service-Level Agreement

  SLI                                 Service-Level Indicator

  SLO                                 Service-Level Objective

  MTTR                                Mean Time to Recovery/Repair (usage
                                      varies by context)

  WAF                                 Web Application Firewall; also used
                                      for AWS Well-Architected Framework
                                      in a different context
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# 4. Certification decision tree

``` text
Start
  |
  +-- Need cloud concepts and a beginner credential?
  |      +-- Yes -> Study Cloud Practitioner (CLF-C02); exam optional
  |
  +-- Want an AWS cloud engineering path?
  |      +-- Learn Linux + networking + AWS labs
  |      +-- Build and document a project
  |      +-- Prepare for Solutions Architect Associate (SAA-C03)
  |      +-- Add Docker + Terraform + CI/CD + monitoring
  |
  +-- Target jobs explicitly require Azure?
  |      +-- AZ-900 fundamentals -> AZ-104 administration
  |
  +-- Target jobs explicitly require Google Cloud?
         +-- Google Cloud fundamentals -> Associate Cloud Engineer
```

Do not try to earn AWS, Azure, and Google Cloud certificates all at
once. Choose the cloud used by your target roles and revisit the others
later.

------------------------------------------------------------------------

# 5. Monthly milestone tracker

Copy this into your task tracker and check off only what you have
actually completed.

## Month 1 --- Foundations

-   [ ] Networking basics and URL request flow
-   [ ] Linux command-line basics
-   [ ] Git/GitHub basics
-   [ ] One small Bash or Python script
-   [ ] Explain key concepts without notes

## Month 2 --- Cloud fundamentals

-   [ ] Cloud models and shared responsibility
-   [ ] AWS account safety and billing basics
-   [ ] IAM, EC2, S3, VPC, security groups
-   [ ] Deploy a simple test page
-   [ ] Document resource cleanup

## Month 3 --- AWS application deployment

-   [ ] Networking and access control lab
-   [ ] Logs and monitoring
-   [ ] Domain/HTTPS concepts
-   [ ] First project deployed and documented
-   [ ] Decide whether Cloud Practitioner exam adds value

## Month 4 --- Certification preparation and project polish

-   [ ] Review official exam objectives
-   [ ] Practice exams and error log
-   [ ] Complete weak-topic labs
-   [ ] Take an exam only if ready and within budget
-   [ ] Improve project README and architecture diagram

## Months 5--6 --- Docker and CI/CD

-   [ ] Containerise application
-   [ ] Docker Compose lab
-   [ ] GitHub Actions pipeline
-   [ ] Automated tests/build
-   [ ] Publish deployment instructions

## Months 7--8 --- Terraform, security, and reliability

-   [ ] Terraform basics and safe provisioning
-   [ ] Least privilege and secrets handling
-   [ ] Monitoring and alerting
-   [ ] Backup/restore exercise
-   [ ] Second project completed

## Months 9--10 --- Kubernetes and advanced practice

-   [ ] Local Kubernetes deployment
-   [ ] Troubleshooting exercises
-   [ ] Cloud architecture review
-   [ ] Certification decision based on job requirements
-   [ ] Third project or meaningful improvement to an existing project

## Months 11--12 --- Job search and revision

-   [ ] Resume and LinkedIn updated
-   [ ] GitHub pinned projects polished
-   [ ] 10--15 interview questions revised per week
-   [ ] Regular applications and follow-ups
-   [ ] Review feedback and close skill gaps

If your schedule is limited, stretch the timeline instead of skipping
hands-on work.

------------------------------------------------------------------------

# 6. Weekly progress template

Copy for each week:

``` markdown
## Week __: [Date range]

### Learning goals
- [ ] Goal 1
- [ ] Goal 2
- [ ] Goal 3

### Labs completed
- [ ] Lab:
- [ ] Lab:

### Evidence
- GitHub commit / PR:
- Screenshot / diagram:
- Notes:

### What I can explain without notes
- 
- 

### Problems I encountered
- Problem:
- Root cause:
- Fix:

### Next week
- [ ] 
- [ ] 

### Review
- Study hours:
- Hands-on hours:
- Biggest improvement:
- Topic to revise:
```

------------------------------------------------------------------------

# 7. First 7 days --- start here

## Day 1

-   [ ] Create the roadmap repository and tracker.
-   [ ] Review 10 job listings and note recurring skills.
-   [ ] Install Git and a Linux environment.

## Day 2

-   [ ] Learn IP addresses, DNS, ports, HTTP, and HTTPS.
-   [ ] Run `nslookup`, `curl -I`, and `ip addr` (or platform
    equivalents).
-   [ ] Write a short explanation of a browser request.

## Day 3

-   [ ] Practise Linux navigation and file commands.
-   [ ] Learn `grep`, `find`, `tail`, and permissions.
-   [ ] Commit your notes to GitHub.

## Day 4

-   [ ] Learn processes, services, logs, disk usage, and SSH.
-   [ ] Write a simple Bash or Python script.

## Day 5

-   [ ] Learn cloud computing, IaaS/PaaS/SaaS, regions, AZs, and shared
    responsibility.
-   [ ] Draw a simple cloud architecture diagram.

## Day 6

-   [ ] Read AWS account security and current billing/free-tier
    guidance.
-   [ ] Learn IAM, EC2, S3, and VPC at a high level.
-   [ ] Do not launch resources until you understand the likely charges.

## Day 7

-   [ ] Review all notes without watching the lessons again.
-   [ ] Explain five concepts aloud.
-   [ ] Record what was difficult and plan the next week.

------------------------------------------------------------------------

# 8. Reliable resources

Start with official documentation for accuracy, then use videos/courses
for explanations.

-   **AWS training and certification:** https://aws.amazon.com/training/
-   **AWS certification overview:**
    https://aws.amazon.com/certification/
-   **AWS Skill Builder:** https://skillbuilder.aws/
-   **AWS pricing calculator:** https://calculator.aws/
-   **AWS Free Tier information:** https://aws.amazon.com/free/
-   **AWS Well-Architected Framework:**
    https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html
-   **Microsoft Learn:** https://learn.microsoft.com/training/
-   **Google Cloud training:** https://cloud.google.com/learn/training
-   **Linux Journey:** https://linuxjourney.com/
-   **Docker documentation:** https://docs.docker.com/
-   **Terraform documentation:**
    https://developer.hashicorp.com/terraform/docs
-   **Kubernetes documentation:** https://kubernetes.io/docs/home/
-   **GitHub Actions:** https://docs.github.com/actions

## Final rule

**Learn → practise → build → document → explain → revise.**

Your goal is not to finish a playlist. Your goal is to be able to
deploy, secure, monitor, troubleshoot, and explain a real system.
