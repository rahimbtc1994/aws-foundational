# aws-foundational

## 1. Requirements

## 2. Compute

1. What is computing?
The brain that make IT operations work.
It collect, analyze, process and distribute data.
2. Components?
CPU: run instructions
RAM: store the data needed by the app (instructions)
Disk: long term storage
Network: bandwidth and latency
OS: manage computer software and hardware (linux ...)
-> Cloud computing : Save on cost, Scalable, Reliable
3. Methods?
Instance: a VM (hosting env, develop env, backup)
Container: a container (microservices)
Servless: run a code (PaaS) without provisioning servers ...
Hybrid: local and cloud ...
4. Services?
EC2:
ECS/EKS: Containers
Lambda: Servelss
Fargate: Servless for containers
Beanstalk: Deploy and scale web app

## 3. AWS EC2
1. def
2. Types (CPU, RAM, Disk, Network)
- Compute optimized: webapp, Videotranscoding
- Memory optimized: big data and caches
- Storage optimized: large db
- Graphic : ML
3. Scaling
4. High availability: because many AZ
5. Cost effectivness: pay only for what you use
6. Purchasing options:
- On-demand instance:  pay as you go
- Saving plans: low prices for 1 to 3 years commitment
- Dedicated hot: reserve physical 
- Spot instance: low price for flexible app
7. Provisioninig
- OS
- Networking details
- Storage options
- Security settings
8. Problems solved : cost, ..
9. Overview: #TODO
10. Benefits: #TODO
11. Architeccture: you need to define 
- Region
- VPC
- Subnet
- Security group
12. Use Cases:
13. Instance Costs:
- IPO: 
    - On-demand instance:  pay for compute per sec MS or Linux/hour others
    - Saving plans:
      1. compute saving plan: 66% reduce
      2. EC2 instance: specific instance family & specific regions
    - Dedicated hot: up t0 72% discount, 1 to 3 yc, with 3 upfornt payment methods
    - Spot instance: up to 90%
- Tenancy:
- define how EC2 instances are distributed accross the hardware
  - Shared instance
  - Dedicated instance
  - Dedicated host

## 4. Using AWS EC2
1. Launching EC2 instance:
- Name & tag: recommanded
- AMI: Template (OS, System Servers, APPs), Launch permissions, Block device mapping
- Type: Hardware (CPU, RAM, Disk, Network)
  - families: (T, M, C, P, R) with ... (t2.micro, t3.large, ...)
  - Example t3.large: family, genration, size
  - categories: General purpose, Compute optimized, Memory optimized, Acclerated computing, Storage optimized
  - Scalable (vertically)
- Key pair: creds to connect to the aws EC2 instance
- Network settings: VPC, Subnet, Security Group + public ip address
  - Region
  - VPC
  - Subnet
  - Public ip address
  - Security group
- Storage: EBS
  - types: (SSD: general purpose, Provisioned IOPS, HDD: Throughput optimized, Cold)
  - configs:
    - type
    - size
    - delete or termination
    - Encryption
  - AWS EFS
  - EC2 storage store
- Advanced details

## 5. Manage AWS Compute