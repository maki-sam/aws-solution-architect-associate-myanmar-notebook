# AWS SAA-C03 Study Guide — မာတိကာ (Architect's Journey Framework)

---

## Toto HtwarHtwar
- 0.1 Preface.md
- 0.2 thankyou_note.md

---

## STAGE I — FOUNDATION

### Part 1: Exam Overview & AWS Global Infrastructure
- 1.1 Exam Format, Domain Weights, Scoring
- 1.2 In-Scope vs Out-of-Scope Services

### Part 2: IAM Fundamentals
- 2.1 Users,Groups,Roles,Policies
- 🧪 Lab 1: IAM Policy Basics

---

## STAGE II — BUILD
*Server, Storage, Database — "App တစ်ခု run ဖို့ ဘာတွေလိုလဲ"*

### Part 3: Compute
- 3.1 EC2 Fundamentals — Instance Types, AMIs
- 3.2 EBS-backed vs Instance Store
- 3.3 Purchasing Options — On-Demand, Reserved, Spot, Savings Plans
- 3.4 EC2 Auto Scaling
- 3.5 Elastic Load Balancing — ALB vs NLB vs GWLB
- 🧪 Lab 2: Launch Template + Auto Scaling Policy
- 🧪 Lab 3: ALB + Target Groups

### Part 4: Storage
- 4.1 S3 Fundamentals — Storage Classes, Versioning, Lifecycle
- 4.2 S3 Advanced — Replication, Glacier
- 4.3 S3 Security Basics — Bucket Policy, SSE-S3
- 4.4 EFS, FSx Family
- 4.5 Storage Gateway, DataSync, Transfer Family, AWS Backup
- 🧪 Lab 4: S3 Lifecycle + Versioning
- 🧪 Lab 5: EBS Snapshot + EFS Mount

### Part 5: Database
- 5.1 RDS — Multi-AZ, Read Replicas, RDS Proxy
- 5.2 Aurora & Aurora Serverless
- 5.3 DynamoDB — Capacity Modes, GSI/LSI, DAX
- 5.4 ElastiCache (Redis vs Memcached)
- 5.5 DMS, DocumentDB, Neptune, Keyspaces, Redshift
- 🧪 Lab 6: RDS Multi-AZ + Read Replica
- 🧪 Lab 7: DynamoDB + Auto Scaling
- 🧪 Lab 8: ElastiCache Setup

---

## STAGE III — CONNECT
*Server တွေချင်း၊ User တွေနဲ့ ချိတ်ဆက်တဲ့ အဆင့်*

### Part 6: Networking & Content Delivery
- 6.1 VPC Basics — Subnets, IGW, NAT Gateway
- 6.2 Route 53 — DNS, Routing Policies
- 6.3 CloudFront & Global Accelerator
- 🧪 Lab 9: Multi-tier VPC + NAT Gateway
- 🧪 Lab 10: Route 53 Routing Policies
- 🧪 Lab 11: CloudFront + S3 Static Website

### Part 7: Application Integration
- 7.1 SQS — Standard vs FIFO
- 7.2 SNS — Pub/Sub & Fan-out
- 7.3 EventBridge
- 7.4 Amazon MQ, AppFlow
- 🧪 Lab 12: SQS + Lambda Decoupled Architecture
- 🧪 Lab 13: SNS Fan-out Pattern

---

## STAGE IV — MODERNIZE
*Server-based ကနေ Container/Serverless ကို ပြောင်းတဲ့ အဆင့်*

### Part 8: Containers
- 8.1 ECS — Fargate vs EC2 Launch Type
- 8.2 EKS Fundamentals, ECR
- 🧪 Lab 14: ECS Fargate Deployment

### Part 9: Serverless
- 9.1 Lambda — Triggers, Memory, Concurrency
- 9.2 Step Functions, API Gateway
- 🧪 Lab 15: Lambda + API Gateway Serverless App

---

## STAGE V — PROTECT & GOVERN
*Production-ready ဖြစ်ဖို့ Security/Compliance/Multi-account အဆင့် (Beginner topic အကုန်ပြီးမှ ဒီကို ရောက်တာ)*

### Part 10: Advanced Identity & Governance
- 10.1 IAM Advanced — Cross-account Access, AWS STS
- 10.2 AWS Organizations, SCPs, Control Tower
- 10.3 IAM Identity Center & Directory Federation
- 10.4 Identity-based vs Resource-based Policies
- 🧪 Lab 16: Cross-account Role Setup

### Part 11: Security & Encryption
- 11.1 KMS, ACM, CloudHSM
- 11.2 Secrets Manager vs Parameter Store
- 11.3 Amazon Cognito
- 11.4 Shield, WAF, Firewall Manager, Network Firewall
- 11.5 GuardDuty, Macie, Inspector, Detective, Security Hub
- 11.6 CloudTrail, Config, Artifact, Audit Manager
- 🧪 Lab 17: KMS Encryption + Secrets Manager
- 🧪 Lab 18: GuardDuty + CloudTrail Setup

### Part 12: Advanced Networking
- 12.1 VPC Security Deep Dive — Security Groups vs NACLs
- 12.2 VPC Peering, Transit Gateway, PrivateLink
- 12.3 Direct Connect, Site-to-Site VPN, Client VPN
- 🧪 Lab 19: VPC Peering + Transit Gateway

### Part 13: Monitoring & Operations
- 13.1 CloudWatch — Metrics, Alarms, Logs
- 13.2 CloudFormation — IaC Basics
- 13.3 Systems Manager
- 13.4 Trusted Advisor, Compute Optimizer, Well-Architected Tool
- 13.5 Service Catalog, License Manager
- 🧪 Lab 20: CloudWatch Alarms + Dashboard
- 🧪 Lab 21: CloudFormation Stack Deploy

---

## STAGE VI — OPTIMIZE & SPECIALIZE
*Cost လျှော့၊ Data/ML/Migration — niche ဒါပေမယ့် exam ပါတဲ့ အပိုင်း*

### Part 14: Cost Management
- 14.1 Cost Explorer, Budgets, Cost & Usage Report
- 14.2 Savings Plans vs Reserved Instances
- 14.3 Cost Allocation Tags, Multi-account Billing
- 🧪 Lab 22: Budget Alert + Cost Explorer Analysis

### Part 15: Migration
- 15.1 Snow Family
- 15.2 AWS Application Migration Service (MGN)

### Part 16: Analytics & Machine Learning
- 16.1 Kinesis, Glue, Lake Formation
- 16.2 Athena, Redshift, OpenSearch, MSK
- 16.3 ML use-cases — Rekognition, Comprehend, Textract

### Part 17: Other Exam-relevant Services
- 17.1 X-Ray
- 17.2 Amplify, API Gateway, Device Farm

---

## STAGE VII — MASTER
*Exam day ပြင်ဆင်တဲ့ နောက်ဆုံးအဆင့်*

### Part 18: Practice & Final Review
- 18.1 Domain-wise Practice Questions
- 18.2 Exam Traps
- 18.3 Quick Reference Cheat Sheet
- 18.4 Exam Day Tips