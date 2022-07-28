

<!-- TOC -->

- [Cloud Computing Fundamentals](#cloud-computing-fundamentals)
  - [Cloud Computing - what is it...really](#cloud-computing---what-is-itreally)
  - [Public vs Private vs Multi vs Hybrid Cloud](#public-vs-private-vs-multi-vs-hybrid-cloud)
  - [Cloud Service Models](#cloud-service-models)
- [Tech Fundamentals](#tech-fundamentals)
  - [YAML101 - YAML AINT MARKUP LANGUAGE](#yaml101---yaml-aint-markup-language)
  - [JSON101 - JavaScript Object Notation](#json101---javascript-object-notation)
  - [Network Starter Pack - 0 - INTRO](#network-starter-pack---0---intro)
- [AWS Fundamentals](#aws-fundamentals)
  - [AWS Public vs Private Services](#aws-public-vs-private-services)
  - [AWS Global Infrastructure](#aws-global-infrastructure)
  - [AWS Default Virtual Private Cloud (VPC)](#aws-default-virtual-private-cloud-vpc)
  - [Elastic Compute Cloud (EC2) Basics](#elastic-compute-cloud-ec2-basics)
  - [Simple Storage Service (S3) Basics](#simple-storage-service-s3-basics)
  - [CloudFormation (CFN) Basics](#cloudformation-cfn-basics)
  - [CloudWatch (CW) Basics](#cloudwatch-cw-basics)
  - [Shared Responsibility Model](#shared-responsibility-model)
  - [High-Availability vs Fault-Tolerance vs Disaster Recovery](#high-availability-vs-fault-tolerance-vs-disaster-recovery)
  - [Domain Name System (DNS) Fundamentals](#domain-name-system-dns-fundamentals)
  - [High-Availability vs Fault-Tolerance vs Disaster Recovery](#high-availability-vs-fault-tolerance-vs-disaster-recovery-1)
  - [Route53 (R53) Fundamentals](#route53-r53-fundamentals)
  - [DNS Record Types](#dns-record-types)
- [IAM, ACCOUNTS AND AWS ORGANISATIONS](#iam-accounts-and-aws-organisations)
  - [IAM Identity Policies](#iam-identity-policies)
  - [IAM Users and ARNs](#iam-users-and-arns)
  - [IAM Users and ARNs](#iam-users-and-arns-1)
  - [IAM Groups](#iam-groups)
  - [IAM Roles - The Tech](#iam-roles---the-tech)
  - [When to use IAM Roles](#when-to-use-iam-roles)
  - [Service-linked Roles & PassRole](#service-linked-roles--passrole)
  - [AWS Organizations](#aws-organizations)
  - [Service Control Policies (SCPs)](#service-control-policies-scps)
  - [CloudWatch Logs](#cloudwatch-logs)
  - [CloudTrail](#cloudtrail)
- [SIMPLE STORAGE SERVICE (S3)](#simple-storage-service-s3)
  - [S3 Security (Resource Policies & ACLs)](#s3-security-resource-policies--acls)
  - [S3 Security (Resource Policies & ACLs)](#s3-security-resource-policies--acls-1)
  - [S3 Static Hosting](#s3-static-hosting)
  - [S3 Object Versioning & MFA Delete](#s3-object-versioning--mfa-delete)
  - [S3 Performance Optimization](#s3-performance-optimization)
  - [S3 Performance Optimization](#s3-performance-optimization-1)
  - [Encryption 101 - Part 1](#encryption-101---part-1)
  - [Encryption 101 - Part 1 & 2](#encryption-101---part-1--2)
  - [Key Management Service (KMS)](#key-management-service-kms)
  - [Object Encryption](#object-encryption)
  - [Key Management Service (KMS)](#key-management-service-kms-1)
  - [S3 Object Storage Classes](#s3-object-storage-classes)
  - [S3 Lifecycle Configuration](#s3-lifecycle-configuration)
  - [S3 Replication](#s3-replication)
  - [S3 PreSigned URLs](#s3-presigned-urls)
  - [S3 Select and Glacier Select](#s3-select-and-glacier-select)
  - [S3 Events](#s3-events)
  - [S3 Access Logs](#s3-access-logs)
- [VIRTUAL PRIVATE CLOUD (VPC) BASICS](#virtual-private-cloud-vpc-basics)
  - [VPC Sizing and Structure](#vpc-sizing-and-structure)
  - [Custom VPCs](#custom-vpcs)
  - [VPC Subnets](#vpc-subnets)
  - [VPC Routing, Internet Gateway & Bastion Hosts](#vpc-routing-internet-gateway--bastion-hosts)
  - [VPC Routing, Internet Gateway & Bastion Hosts](#vpc-routing-internet-gateway--bastion-hosts-1)
  - [Stateful vs Stateless Firewalls](#stateful-vs-stateless-firewalls)
  - [Network Access Control Lists (NACLs)](#network-access-control-lists-nacls)
  - [Security Groups (SG)](#security-groups-sg)
  - [Network Address Translation (NAT) & NAT Gateway](#network-address-translation-nat--nat-gateway)
  - [Network Address Translation (NAT) & NAT Gateway](#network-address-translation-nat--nat-gateway-1)
- [ELASTIC COMPUTE CLOUD (EC2) BASICS](#elastic-compute-cloud-ec2-basics-1)
  - [Virtualization](#virtualization)
  - [EC2 Architecture and Resilience](#ec2-architecture-and-resilience)
  - [EC2 Instance Types](#ec2-instance-types)
  - [Storage Refresher](#storage-refresher)
  - [Elastic Block Store (EBS) Service Architecture](#elastic-block-store-ebs-service-architecture)
  - [EBS Volume Types - General Purpose](#ebs-volume-types---general-purpose)
  - [EBS Volume Types - Provisioned IOPS](#ebs-volume-types---provisioned-iops)
  - [EBS Volume Types - HDD-Based](#ebs-volume-types---hdd-based)
  - [Instance Store Volumes - Architecture](#instance-store-volumes---architecture)
  - [Choosing between the EC2 Instance Store and EBS](#choosing-between-the-ec2-instance-store-and-ebs)
  - [Snapshots, Restore & Fast Snapshot Restore (FSR)](#snapshots-restore--fast-snapshot-restore-fsr)
  - [EBS Encryption](#ebs-encryption)
  - [EBS Encryption](#ebs-encryption-1)
  - [EC2 Purchase Options](#ec2-purchase-options)
  - [EC2 Purchase Options](#ec2-purchase-options-1)
  - [Instance Status Checks & Auto Recovery](#instance-status-checks--auto-recovery)
  - [Horizontal & Vertical Scaling](#horizontal--vertical-scaling)
- [CONTAINERS & ECS](#containers--ecs)
  - [Introduction to Containers](#introduction-to-containers)
  - [ECS - Concepts](#ecs---concepts)
  - [ECS - Cluster Mode](#ecs---cluster-mode)
- [ADVANCED EC2](#advanced-ec2)
  - [Bootstrapping EC2 using User Data](#bootstrapping-ec2-using-user-data)
  - [Enhanced Bootstrapping with CFN-INIT](#enhanced-bootstrapping-with-cfn-init)
  - [EC2 Instance Roles & Profile](#ec2-instance-roles--profile)
  - [SSM Parameter Store](#ssm-parameter-store)
  - [System and Application Logging on EC2](#system-and-application-logging-on-ec2)
  - [EC2 Placement Groups](#ec2-placement-groups)
  - [Dedicated Hosts](#dedicated-hosts)
  - [Enhanced Networking & EBS Optimized](#enhanced-networking--ebs-optimized)
- [Route 53 - Global DNS](#route-53---global-dns)
  - [R53 Public Hosted Zones](#r53-public-hosted-zones)
  - [R53 Private Hosted Zones](#r53-private-hosted-zones)
  - [CNAME vs R53 Alias](#cname-vs-r53-alias)
  - [Simple Routing](#simple-routing)
  - [R53 Health Checks](#r53-health-checks)
  - [Failover Routing](#failover-routing)
  - [Multi Value Routing](#multi-value-routing)
  - [Weighted Routing](#weighted-routing)
  - [Latency Routing](#latency-routing)
  - [Geolocation Routing](#geolocation-routing)
  - [Geoproximity](#geoproximity)
  - [R53 Interoperability](#r53-interoperability)
- [Relational Database Service (RDS)](#relational-database-service-rds)
  - [Database Refresher & MODELS - PART1 - SQL](#database-refresher--models---part1---sql)
  - [Database Refresher & MODELS - PART2 - NoSQL](#database-refresher--models---part2---nosql)
  - [ACID vs BASE](#acid-vs-base)
  - [Databases on EC2](#databases-on-ec2)
  - [Relational Database Service (RDS) Architecture](#relational-database-service-rds-architecture)
  - [RDS High-Availability (Multi AZ)](#rds-high-availability-multi-az)
  - [RDS Automatic Backup, RDS Snapshots and Restore](#rds-automatic-backup-rds-snapshots-and-restore)
  - [RDS Read-Replicas](#rds-read-replicas)
  - [RDS Data Security](#rds-data-security)
  - [Aurora Architecture](#aurora-architecture)
  - [Aurora Serverless](#aurora-serverless)
  - [Aurora Global Database](#aurora-global-database)
  - [Aurora Multi-master writes](#aurora-multi-master-writes)
  - [Database Migration Service (DMS)](#database-migration-service-dms)
- [NETWORK STORAGE & DATA LIFECYCLE](#network-storage--data-lifecycle)
  - [EFS Architecture](#efs-architecture)
- [HA & SCALING](#ha--scaling)
  - [Regional and Global AWS Architecture](#regional-and-global-aws-architecture)
  - [Elastic Load Balancer](#elastic-load-balancer)
  - [Application Load balancing (ALB) vs Network Load Balancing (NLB)](#application-load-balancing-alb-vs-network-load-balancing-nlb)
  - [Launch Configuration and Templates](#launch-configuration-and-templates)
  - [Auto-Scaling Groups](#auto-scaling-groups)
  - [ASG Scaling Policies](#asg-scaling-policies)
  - [ASG Lifecycle Hooks](#asg-lifecycle-hooks)
  - [ASG HealthCheck Comparison - EC2 vs ELB](#asg-healthcheck-comparison---ec2-vs-elb)
  - [SSL Offload & Session Stickiness](#ssl-offload--session-stickiness)
  - [Gateway Load Balancer](#gateway-load-balancer)
- [SERVERLESS AND APPLICATION SERVICES](#serverless-and-application-services)
  - [Architecture Deep Dive - PART1 and PART2](#architecture-deep-dive---part1-and-part2)
  - [AWS Lambda](#aws-lambda)
  - [CloudWatchEvents and EventBridge](#cloudwatchevents-and-eventbridge)
  - [Serverless Architecture](#serverless-architecture)
  - [Simple Notification Service](#simple-notification-service)
  - [Step Functions](#step-functions)
  - [API Gateway](#api-gateway)
  - [Simple Queue Service](#simple-queue-service)
  - [Kinesis Data Streams](#kinesis-data-streams)
  - [Kinesis Data Firehose](#kinesis-data-firehose)
  - [Kinesis Data Analytics](#kinesis-data-analytics)
  - [Amazon Cognito - User and Identity Pools](#amazon-cognito---user-and-identity-pools)
- [GLOBAL CONTENT DELIVERY AND OPTIMIZATION](#global-content-delivery-and-optimization)
  - [Cloudfront Architecture](#cloudfront-architecture)
  - [Cloudfront Behaviours](#cloudfront-behaviours)
  - [CF TTL and Invalidations](#cf-ttl-and-invalidations)
  - [ACM](#acm)
  - [Cloudfront and SSL/TLS](#cloudfront-and-ssltls)
  - [Origin Types & Origin Architecture](#origin-types--origin-architecture)
  - [Securing CF and S3 using OAI](#securing-cf-and-s3-using-oai)
  - [Lambda@Edge](#lambdaedge)
  - [Global Accelerator](#global-accelerator)
- [VPC Flow Logs](#vpc-flow-logs)
  - [VPC Flow Logs](#vpc-flow-logs-1)
  - [Egress-Only Internet gateway](#egress-only-internet-gateway)
  - [VPC Endpoints (Gateway)](#vpc-endpoints-gateway)
  - [VPC Endpoints (Interface)](#vpc-endpoints-interface)
  - [VPC Peering](#vpc-peering)
- [HYBRID ENVIRONMENTS AND MIGRATION](#hybrid-environments-and-migration)
  - [Border Gateway Protocol 101](#border-gateway-protocol-101)
  - [AWS Site-to-Site VPN](#aws-site-to-site-vpn)
  - [Direct Connect](#direct-connect)
  - [Direct Connect Resilience](#direct-connect-resilience)
  - [Transit Gateway](#transit-gateway)
  - [Storage gateway](#storage-gateway)
  - [Snowball / Edge / Snowmobile](#snowball--edge--snowmobile)
  - [Directory Service](#directory-service)
  - [DataSync](#datasync)
  - [FSx for Windows Servers](#fsx-for-windows-servers)
  - [FSx For Lustre](#fsx-for-lustre)
- [SECURITY, DEPLOYMENT & OPERATIONS](#security-deployment--operations)
  - [AWS Secrets Manager](#aws-secrets-manager)
  - [AWS WAF & Shield](#aws-waf--shield)
  - [CloudHSM](#cloudhsm)
  - [AWS Config](#aws-config)
  - [Amazon Macie](#amazon-macie)
  - [Amazon Inspector](#amazon-inspector)
  - [Amazon Guardduty](#amazon-guardduty)
- [Infrastructure as Code (CloudFormation)](#infrastructure-as-code-cloudformation)
  - [CloudFormation Physical & Logical Resources](#cloudformation-physical--logical-resources)
  - [CloudFormation Template and Pseudo Parameters](#cloudformation-template-and-pseudo-parameters)
  - [CloudFormation Intrinsic Functions](#cloudformation-intrinsic-functions)
  - [CloudFormation Mappings](#cloudformation-mappings)
  - [CloudFormation Outputs](#cloudformation-outputs)
  - [CloudFormation Conditions](#cloudformation-conditions)
  - [CloudFormation DependsOn](#cloudformation-dependson)
  - [CloudFormation Wait Conditions & cfn-signal](#cloudformation-wait-conditions--cfn-signal)
  - [CloudFormation Wait Conditions & cfn-signal](#cloudformation-wait-conditions--cfn-signal-1)
  - [CloudFormation Nested Stacks](#cloudformation-nested-stacks)
  - [CloudFormation Cross-Stack References](#cloudformation-cross-stack-references)
  - [CloudFormation Stack Sets](#cloudformation-stack-sets)
  - [CloudFormation Deletion Policy](#cloudformation-deletion-policy)
  - [CloudFormation Deletion Policy](#cloudformation-deletion-policy-1)
  - [CloudFormation Init (CFN-INIT)](#cloudformation-init-cfn-init)
  - [CloudFormation cfn-hup](#cloudformation-cfn-hup)
  - [CloudFormation ChangeSets](#cloudformation-changesets)
  - [CloudFormation Custom Resources](#cloudformation-custom-resources)
- [NOSQL Databases & DynamoDB](#nosql-databases--dynamodb)
  - [DynamoDB - Architecture](#dynamodb---architecture)
  - [DynamoDB - Operations, Consistency and Performance-PART1](#dynamodb---operations-consistency-and-performance-part1)
  - [DynamoDB - Operations, Consistency and Performance-PART2](#dynamodb---operations-consistency-and-performance-part2)
  - [DynamoDB Local and Global Secondary Indexes](#dynamodb-local-and-global-secondary-indexes)
  - [DynamoDB - Streams & Lambda Triggers](#dynamodb---streams--lambda-triggers)
  - [DynamoDB - Global Tables](#dynamodb---global-tables)
  - [DynamoDB - Accelerator (DAX)](#dynamodb---accelerator-dax)
  - [Amazon Athena](#amazon-athena)
  - [Elasticache](#elasticache)
  - [Redshift Architecture](#redshift-architecture)
  - [Redshift DR and Resilience](#redshift-dr-and-resilience)

<!-- /TOC -->

# Cloud Computing Fundamentals
___

## Cloud Computing - what is it...really

Cloud Computing isn't a buzzword - it's a unique type of computing which has a formal set of definitions.

This lesson aims to dispel the jargon, and step through what makes cloud ... cloud.

NIST Special Publication 800-145 : https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-145.pdf

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14040936

___

## Public vs Private vs Multi vs Hybrid Cloud

Understanding what Public Cloud, Private Cloud, Hybrid Cloud and Muti Cloud are is a hugely under rated skill.

More and more larger AWS deployments are requiring a level of bespoke deployment and locational efficiency that only Hybrid cloud can provide, or a level of cloud vendor resilience only achievable with Multi Cloud.

As an AWS solutions architect understanding what IS, and what ISN'T Public, Private, Hybrid and Multi cloud will help in the Exam and in real-world usage.

This lesson steps through the key points of all four types of cloud.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14040943

___

## Cloud Service Models

Cloud Service models define what service you receive from a product.

It defines which parts of the infrastructure stack you are responsible for and which the vendor manages.

They define your unit of consumption - which is the thing you pay for.


As a Service Model Examples : https://en.wikipedia.org/wiki/As_a_service

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14040947

___

# Tech Fundamentals
___

## YAML101 - YAML AINT MARKUP LANGUAGE

YAML (a recursive acronym for "YAML Ain't Markup Language") is a human-readable data-serialization language. It is commonly used for configuration files and in applications where data is being stored or transmitted. 

It's used within AWS as one of two supported CloudFormation Template formats

This lesson is an introduction to YAML

https://en.wikipedia.org/wiki/Recursive_acronym

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/27415250

___

## JSON101 - JavaScript Object Notation

JavaScript Object Notation  is an open standard file format, and data interchange format, that uses human-readable text to store and transmit data objects consisting of attribute–value pairs and array data types 

It's used within AWS as one of two CloudFormation template formats and for identity and resource policies.

This lesson is a high level introduction to JSON.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/27415253

___

## Network Starter Pack - 0 - INTRO

This lesson series will step through the OSI 7-Layer Networking Model

Physical
Data Link
Network
Transport
Session
Presentation
Application

https://en.wikipedia.org/wiki/OSI_model

**Link to videos:**

- Network Starter Pack - 0 - INTRO
  - https://learn.cantrill.io/courses/730712/lectures/25094903

- Network Starter Pack - 1 - PHYSICAL
  - https://learn.cantrill.io/courses/730712/lectures/25094904

- Network Starter Pack - 2 - Data Link - Part 1
  - https://learn.cantrill.io/courses/730712/lectures/25094906

- Network Starter Pack - 2 - Data Link - Part 2
  - https://learn.cantrill.io/courses/730712/lectures/25094908

- Decimal to Binary Conversion (IP Addressing)
  - https://learn.cantrill.io/courses/730712/lectures/32357244

- Network Starter Pack - 3 - Network - Part 1
  - https://learn.cantrill.io/courses/730712/lectures/25141550

- Network Starter Pack - 3 - Network - Part 2
  - https://learn.cantrill.io/courses/730712/lectures/25141552

- Network Starter Pack - 3 - Network - Part 3
  - https://learn.cantrill.io/courses/730712/lectures/25141553

- Network Starter Pack - 4 - Transport - Part 1
  - https://learn.cantrill.io/courses/730712/lectures/25171215

- Network Starter Pack - 4 - Transport - Part 2
  - https://learn.cantrill.io/courses/730712/lectures/25171216

- Network Starter Pack - EXTRA - Network Address Translation - PART1
  - https://learn.cantrill.io/courses/730712/lectures/25279341

- Network Starter Pack - EXTRA - Network Address Translation - PART2
  - https://learn.cantrill.io/courses/730712/lectures/25279345

- Network Starter Pack - EXTRA - Subnetting - PART1
  - https://learn.cantrill.io/courses/730712/lectures/26984983

- Network Starter Pack - EXTRA - Subnetting - PART2
  - https://learn.cantrill.io/courses/730712/lectures/26984984

- Network Starter Pack - EXTRA - Distributed Denial of Service (DDOS)
  - https://learn.cantrill.io/courses/730712/lectures/26952882

- Secure Sockets Layer (SSL) and Transport Layer Security (TLS)
  - https://learn.cantrill.io/courses/730712/lectures/27799870

- Hash Functions & Hashing
  - https://learn.cantrill.io/courses/730712/lectures/41817977

- Digital Signatures
  - https://learn.cantrill.io/courses/730712/lectures/41818183


# AWS Fundamentals
___

## AWS Public vs Private Services

AWS Services can be divided into public and private AWS services

In this lesson I explain the difference between the two - focussing on the network zones these services are hosted in.

https://github.com/acantril/aws-sa-associate-saac02/blob/master/04-AWS-Fundamentals/00_LearningAids/Public%26PrivateServices.pdf


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14040998

___

## AWS Global Infrastructure

AWS have created a global public cloud platform which consists of isolated 'regions' connected together by high speed global networking.

This lesson reviews the main architectural components of AWS, Regions, Edge Locations and Availability Zones.

It also discusses what it means to be Globally Resilient, Regional Resilient and AZ resilient.


**Lesson Links**

AWS Website used in this lesson https://www.infrastructure.aws/


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14041000


___

## AWS Default Virtual Private Cloud (VPC)

A default VPC is created once per region when an AWS account is first created.

There can only be one default VPC per region, and they can be deleted and recreated from the console UI .

They always have the same IP range and same '1 subnet per AZ' architecture.

This lesson details and demos the functionality of a default VPC.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14041001

___

## Elastic Compute Cloud (EC2) Basics

The Elastic Compute Cloud or EC2 is AWS's implement of IAAS - Infrastructure as a service.

It allows you to provision virtual machines known as instances with resources you select and an operating system of your choosing.

This lesson provides an initial overview of what an instance is, instance states, what an Amazon Machine Image does and talks about how to connect to instances.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14041048

___

## Simple Storage Service (S3) Basics

Simple Storage Service (S3) is a core AWS service.

It provides a near infinitely scalable object storage platform - accessible from anywhere with a public internet connection.

It tends to be the default storage location for data ingestion and output for many AWS services.

This lesson introduces S3, Objects and Buckets


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14041055

___

## CloudFormation (CFN) Basics

CloudFormation is an Infrastructure as Code (IaC) product in AWS which allows automation infrastructure creation, update and deletion.

Templates created in YAML or JSON can be used to automate infrastructure operations

Templates are used to create stacks, which are used to interact with resources in an AWS account.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14041060

___

## CloudWatch (CW) Basics

CloudWatch is a core supporting service within AWS which provides metric, log and event management services.

It's used through other AWS services for health and performance monitoring, log management and nerveless architectures.

This lesson steps through the basics.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14041064


___

## Shared Responsibility Model

The Shared Responsibility Model - is how AWS provide clarity around which areas of systems security are theirs, and which are owned by the customer.

The model is useful as you learn about AWS and so this lesson provides a brief introduction


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14041065

___

## High-Availability vs Fault-Tolerance vs Disaster Recovery

High Availability (HA), Fault-Tolerance (FT) and Disaster Recover (DR) are three essential concepts to understand for every Solutions Architect.

Whats more important is understanding the differences between the three - specifically HA and FT.

Most technical people don't have a correct grasp .. this lesson aims to ensure that you do, before starting the main course content.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14041073

___

## Domain Name System (DNS) Fundamentals

In this lesson I step through the fairly complex architecture of DNS - the domain name system.

DNS is probably one of the most important distributed databases which exist today.

It is used for service discovery, configuration and the operation of most consumer web browsing and other internet activities.

While not strictly required in detail for the exam - understanding DNS will help you answer DNS related questions and help make sense of other AWS lessons throughout the course.

**Lesson Links**

IANA : https://www.iana.org

Root hints : https://www.internic.net/domain/named.root

Root Servers : https://www.iana.org/domains/root/servers

Root Zone Database : https://www.iana.org/domains/root/db

Root Zone File : https://www.internic.net/domain/root.zone

Delegation Record for .com : https://www.iana.org/domains/root/db/com.html


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14041088
- https://learn.cantrill.io/courses/730712/lectures/14225527

___

## High-Availability vs Fault-Tolerance vs Disaster Recovery

High Availability (HA), Fault-Tolerance (FT) and Disaster Recover (DR) are three essential concepts to understand for every Solutions Architect.

Whats more important is understanding the differences between the three - specifically HA and FT.

Most technical people don't have a correct grasp .. this lesson aims to ensure that you do, before starting the main course content.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14041073

___

## Route53 (R53) Fundamentals

In this lesson I step through how r53 is architectures and some of its benefits and features.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14041089

___

## DNS Record Types

DNS is capable of handling a number of different record types - which perform different tasks.

This lesson steps through :-

A & AAAA
CNAME
TXT
MX
NS

as well as introducing TTL values on records.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14041093


# IAM, ACCOUNTS AND AWS ORGANISATIONS
___

## IAM Identity Policies

Identity Policies are attached to AWS identities and either ALLOW or DENY access to AWS resources.

In this lesson I step through the main components of an IAM policy .. and discuss in some detail about the priority order or ALLOW and DENY.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14274988

**AWS docs:** 

- [Policies and permissions in IAM](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html)


___

## IAM Users and ARNs

IAM Users are one of the identity types available inside AWS.

They are type you pick when you can identity a single individual or 'thing' which will use that identity - a person, an application or a service account.

In this lesson I detail the architecture of an IAM user ... how it authenticates, and talk about ARNs which are how resources in AWS are identified.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14275269

**AWS docs:** 

- [Amazon Resource Names (ARNs)](https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html)

___

## IAM Users and ARNs

IAM Users are one of the identity types available inside AWS.

They are type you pick when you can identity a single individual or 'thing' which will use that identity - a person, an application or a service account.

In this lesson I detail the architecture of an IAM user ... how it authenticates, and talk about ARNs which are how resources in AWS are identified.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14275269

**AWS docs:** 

- [Amazon Resource Names (ARNs)](https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html)

___

## IAM Groups

IAM Groups are a feature of IAM which you need to know about for the exam.

They are an admin or container feature.

You can add IAM users to groups, and add permissions to Groups

Groups are NOT real identities ... can't be used from resource policies and have no credentials to login with.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14275293

**AWS docs:** 

- [IAM user groups](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_groups.html)


___

## IAM Roles - The Tech

IAM Roles are one of the more difficult AWS identity types of fully understand.

In this lesson I step through the basic technical and architecture points of AWS IAM Roles.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14293449

**AWS docs:** 

- [IAM roles](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html)

___

## When to use IAM Roles

In this lesson I try to step through the type of situations where IAM roles might be used.

By giving examples - I hope to make you more comfortable when to select and when NOT to select roles.

It's an important set of skills to have for the exam and real-world AWS usage.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14293450

**AWS docs:** 

- [Using IAM roles](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_use.html)

___

## Service-linked Roles & PassRole

A service-linked role is a unique type of IAM role that is linked directly to an AWS service. Service-linked roles are predefined by the service and include all the permissions that the service requires to call other AWS services on your behalf. The linked service also defines how you create, modify, and delete a service-linked role. A service might automatically create or delete the role. It might allow you to create, modify, or delete the role as part of a wizard or process in the service. Or it might require that you use IAM to create or delete the role.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/40570800

**AWS docs:** 

- [Using service-linked roles](https://docs.aws.amazon.com/IAM/latest/UserGuide/using-service-linked-roles.html)


___

## AWS Organizations

In this lesson I explain AWS Organizations - It's architecture and some of the benefits for businesses managing larger numbers of AWS Accounts.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14293487

**AWS docs:** 

- [AWS Organizations](https://aws.amazon.com/organizations/)

___

## Service Control Policies (SCPs)

In this lesson I introduce service control policies - a feature of AWS Organizations which allow restrictions to be placed on MEMBER accounts in the form of boundaries.

SCPs can be applied to the organization, to OU's or to individual accounts.

Member accounts can be effected, the MANAGEMENT account cannot.

SCPs DON'T GIVE permission - they just control what an account CAN and CANNOT grant via identity policies.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14293489

**AWS docs:** 

- [Service control policies (SCPs)](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scps.html)

___


## CloudWatch Logs

CloudWatch Logs is a service which can accept logging data, store it and monitor it.

It is often the default place where AWS Services can output their logging too.

CloudWatch Logs is a public service and can also be utilised in an on-premises environment and even from other public cloud platforms.

This lesson introduces the main concepts of CloudWatch Logs and its architecture.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14293489

**AWS docs:** 

- [What is Amazon CloudWatch Logs?](https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/WhatIsCloudWatchLogs.html)

___

## CloudTrail

CloudTrail Is a product which logs API calls and account events.

It's very often used to diagnose security or performance issues, or to provide quality account level traceability.

It is enabled by default in AWS accounts and logs free information with a 90 day retention.

It can be configured to store data indefinitely in S3 or CloudWatch Logs.

In this lesson I detail the theory and architecture of the product.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14304051

**AWS docs:** 

- [What Is AWS CloudTrail?](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-user-guide.html)


# SIMPLE STORAGE SERVICE (S3)

___

## S3 Security (Resource Policies & ACLs)

S3 Security is controlled via a combination of Identity Policies, Bucket Policies (Resource Policies) and Legacy Bucket and Object ACLs

This lesson introduces bucket policies and warns you off using ACLs

Bucket Policy Examples : https://docs.aws.amazon.com/AmazonS3/latest/dev/example-bucket-policies.html


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14305158

**AWS docs:** 

- [What is Amazon S3?](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html)

___

## S3 Security (Resource Policies & ACLs)

S3 Security is controlled via a combination of Identity Policies, Bucket Policies (Resource Policies) and Legacy Bucket and Object ACLs

This lesson introduces bucket policies and warns you off using ACLs

Bucket Policy Examples : https://docs.aws.amazon.com/AmazonS3/latest/dev/example-bucket-policies.html


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14305158

**AWS docs:** 

- [What is Amazon S3?](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html)

___


## S3 Static Hosting

Accessing S3 is generally done via APIs

Static Website Hosting is a feature of the product which lets you define a HTTP endpoint, set index and error documents and use S3 like a website.

This lesson exposures the functionality and some common usages.

S3 Pricing : https://aws.amazon.com/s3/pricing/

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14305160

**AWS docs:**

[Hosting a static website using Amazon S3](https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html)

___

## S3 Object Versioning & MFA Delete

Object versioning is a feature which can be enabled on an S3 bucket - allowing the bucket to store multi versions of objects

These objects can be referenced by their version ID to interact directly - or omit this to reference the latest version of an object

Objects aren't deleted - object deletion markers are put in place to hide objects.

Versioning is an essential feature to understand for the exam.

MFADelete is a related feature which is also discussed.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14305171

**AWS docs:**

[Deleting object versions from a versioning-enabled bucket](https://docs.aws.amazon.com/AmazonS3/latest/userguide/DeletingObjectVersions.html)

___

## S3 Performance Optimization

This lesson reviews how S3 Uploads (PutObject) works

Single PUT Upload

Multipart Upload

Finishing up by reviewing how S3 Transfer Acceleration works and how it could benefit Animals4life remote workers when uploading large data sets.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14305180

**AWS docs:**

[Best practices design patterns: optimizing Amazon S3 performance](https://docs.aws.amazon.com/AmazonS3/latest/userguide/optimizing-performance.html)

___

## S3 Performance Optimization

This lesson reviews how S3 Uploads (PutObject) works

Single PUT Upload

Multipart Upload

Finishing up by reviewing how S3 Transfer Acceleration works and how it could benefit Animals4life remote workers when uploading large data sets.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14305180

**AWS docs:**

[Best practices design patterns: optimizing Amazon S3 performance](https://docs.aws.amazon.com/AmazonS3/latest/userguide/optimizing-performance.html)

___

## Encryption 101 - Part 1

In part 1 of this lesson I step through the difference between encryption at rest, and encryption in transit.

I discuss the high level components of encryption and provide definitions

We look at Symmetric encryption - how it works, and what its limitations are

and we finish by evaluation Asymmetric encryption and how it addresses these problems.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14368208

**AWS docs:**

[Protecting data using encryption](https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingEncryption.html)

___

## Encryption 101 - Part 1 & 2

In part 1 of this lesson I step through the difference between encryption at rest, and encryption in transit.

I discuss the high level components of encryption and provide definitions

We look at Symmetric encryption - how it works, and what its limitations are

and we finish by evaluation Asymmetric encryption and how it addresses these problems.


In Part 2 of this lesson I step through the process of signing - and how it can help to prove identity using Asymmetric keys

and we finish up talking about steganography the processing of hiding data inside of something else.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14368208
- https://learn.cantrill.io/courses/730712/lectures/14368213

**AWS docs:**

[Protecting data using encryption](https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingEncryption.html)

___

## Key Management Service (KMS)

AWS Key Management Service (AWS KMS) makes it easy for you to create and manage cryptographic keys and control their use across a wide range of AWS services and in your applications. AWS KMS is a secure and resilient service that uses hardware security modules that have been validated under FIPS 140-2, or are in the process of being validated, to protect your keys.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14305193

**AWS docs:**

[AWS Key Management Service](https://docs.aws.amazon.com/kms/latest/developerguide/overview.html)

___

## Object Encryption

This lesson steps through the various encryption options available within S3 and finishes by looking at default bucket encryption settings

Client-Side Encryption
SSE-C
SSE-S3
SSE-KMS
As part of the lesson we review how SSE-KMS impacts permissions and how it can achieve role separation.



https://docs.aws.amazon.com/AmazonS3/latest/user-guide/default-bucket-encryption.html

https://docs.aws.amazon.com/kms/latest/developerguide/services-s3.html

https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingKMSEncryption.html

https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingServerSideEncryption.html

https://docs.aws.amazon.com/AmazonS3/latest/dev/ServerSideEncryptionCustomerKeys.html

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14305204
- https://learn.cantrill.io/courses/730712/lectures/14391330


___

## Key Management Service (KMS)

AWS Key Management Service (AWS KMS) makes it easy for you to create and manage cryptographic keys and control their use across a wide range of AWS services and in your applications. AWS KMS is a secure and resilient service that uses hardware security modules that have been validated under FIPS 140-2, or are in the process of being validated, to protect your keys.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14305193

**AWS docs:**

[AWS Key Management Service](https://docs.aws.amazon.com/kms/latest/developerguide/overview.html)


___

## S3 Object Storage Classes

This lesson steps through the S3 storage classes

PART 1 - covers S3 Standard, S3 Standard-IA and S3 One Zone-IA

PART 2 - covers S3 Glacier, S3 Glacier Deep Archive and Intelligent-Tiering

https://aws.amazon.com/s3/pricing/

https://aws.amazon.com/s3/storage-classes/


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/24266000
- https://learn.cantrill.io/courses/730712/lectures/24266028


___

## S3 Lifecycle Configuration

This lesson steps through S3 lifecycle management/configuration/rules both in theory and via an S3 console example.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/24266078

**AWS docs:**

[Examples of S3 Lifecycle configuration](https://docs.aws.amazon.com/AmazonS3/latest/userguide/lifecycle-configuration-examples.html)

___

## S3 Replication

S3 has to replication features which allow objects to be replicated between a SOURCE and DESTINATION buckets in the same or different AWS accounts

Cross-Region Replication (CRR) is the process used when Source and Destination are in different AWS regions

Same-Region Replication (SRR) is used when the buckets are in the same region.

This lesson introduces the theory, features and limitations of both of these methods.

https://docs.aws.amazon.com/AmazonS3/latest/dev/replication-what-is-isnot-replicated.html

Lesson Links

https://docs.aws.amazon.com/AmazonS3/latest/dev/replication.html

https://aws.amazon.com/about-aws/whats-new/2019/11/amazon-s3-replication-time-control-for-predictable-replication-time-backed-by-sla/

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14305189

___

## S3 PreSigned URLs

Presigned URL's are a feature of S3 which allows the system to generate a URL with access permissions encoded into it, for a specific bucket and object, valid for a certain time period.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14305206

**AWS docs:**

[Using presigned URLs](https://docs.aws.amazon.com/AmazonS3/latest/userguide/using-presigned-url.html)

___

## S3 Select and Glacier Select

S3 and Glacier Select allow you to use a SQL-Like statement to retrieve partial objects from S3 and Glacier.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15828869

**AWS docs:**

[Querying Archives with S3 Glacier Select](https://docs.aws.amazon.com/amazonglacier/latest/dev/glacier-select.html)

___

## S3 Events

The Amazon S3 notification feature enables you to receive notifications when certain events happen in your bucket. To enable notifications, you must first add a notification configuration that identifies the events you want Amazon S3 to publish and the destinations where you want Amazon S3 to send the notifications. You store this configuration in the notification subresource that is associated with a bucket

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/30151243

**AWS docs:**

[Amazon S3 Event Notifications](https://docs.aws.amazon.com/AmazonS3/latest/userguide/NotificationHowTo.html)

___

## S3 Access Logs

Server access logging provides detailed records for the requests that are made to a bucket. Server access logs are useful for many applications. For example, access log information can be useful in security and access audits. It can also help you learn about your customer base and understand your Amazon S3 bill.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/30151271

**AWS docs:**

[Enabling Amazon S3 server access logging](https://docs.aws.amazon.com/AmazonS3/latest/userguide/enable-server-access-logging.html)


# VIRTUAL PRIVATE CLOUD (VPC) BASICS
___

## VPC Sizing and Structure


This lesson steps through the design choices around VPC design and IP planning.


Lesson Links

https://aws.amazon.com/answers/networking/aws-single-vpc-design/

https://cloud.google.com/vpc/docs/vpc

https://github.com/acantril/aws-sa-associate-saac02/tree/master/07-VPC-Basics/01_vpc_sizing_and_structure

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14419885
- https://learn.cantrill.io/courses/730712/lectures/14441636

___

## Custom VPCs

This video steps through the architecture and features of Custom VPCs including the main issues which are raised in the exam.

In the second half .. a [DEMO] portion - we implement the VPC shell for the Animals4life (A4L) organization in our accounts.



Lesson Links

VPC Limits https://docs.aws.amazon.com/vpc/latest/userguide/amazon-vpc-limits.html

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14419886

___

## VPC Subnets

In this lesson I explain the architecture of VPC subnets - their features and some of the configuration options they provide.

We also cover the IPs which are reserved and unavailable for use in every VPC and the IP auto assignment options configurable on a per Subnet basis.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14419888

**AWS docs:**

[Subnets for your VPC](https://docs.aws.amazon.com/vpc/latest/userguide/configure-subnets.html)

___

## VPC Routing, Internet Gateway & Bastion Hosts

In this lesson we step through the architecture and functionality of Route Tables, Routes, Associations, the internet gateway and public IP v4 functionality within a VPC

The lesson finishes by briefly discussing what a Bastion or Jumpbox does.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14419889

**AWS docs:**

- [Configure route tables](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Route_Tables.html)
- [Connect to the internet using an internet gateway](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Internet_Gateway.html)

___

## VPC Routing, Internet Gateway & Bastion Hosts

In this lesson we step through the architecture and functionality of Route Tables, Routes, Associations, the internet gateway and public IP v4 functionality within a VPC

The lesson finishes by briefly discussing what a Bastion or Jumpbox does.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14419889

**AWS docs:**

- [Configure route tables](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Route_Tables.html)

___

## Stateful vs Stateless Firewalls

Firewalls can either be stateless or stateful - this lesson explains the difference between the two.

Developing an understanding, is essential to be able to implement these networking security features in AWS.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36039663

**AWS docs:**

- [Network Firewall stateless and stateful rules engines](https://docs.aws.amazon.com/network-firewall/latest/developerguide/firewall-rules-engines.html)

___

## Network Access Control Lists (NACLs)

A network access control list (ACL) is an optional layer of security for your VPC that acts as a firewall for controlling traffic in and out of one or more subnets. You might set up network ACLs with rules similar to your security groups in order to add an additional layer of security to your VPC. This lesson steps through the features of a NACL, the impact of their stateless nature and some of the key points to be aware of for the exam.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14419892

**AWS docs:**

- [Control traffic to subnets using Network ACLs](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html)
- [Access control list (ACL) overview](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html)

___

## Security Groups (SG)

Security Groups (SGs) are another security feature of AWS VPC ... only unlike NACLs they are attached to AWS resources, not VPC subnets.

SGs offer a few advantages vs NACLs in that they can recognize AWS resources and filter based on them, they can reference other SGs and also themselves.

But.. SGs are not capable of explicitly blocking traffic - so often require assistance from NACLs

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14480041

**AWS docs:**

- [Control traffic to resources using security groups](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html)

___

## Network Address Translation (NAT) & NAT Gateway

In this 2-part lesson we step through the architecture of Network Address Translation or (NAT) - what it does, and why it's required within AWS.

and we look at the NAT Gateway service - AWS NAT-as-a-service Gateway Product.

**Link to video:**
- https://learn.cantrill.io/courses/730712/lectures/14419891
- https://learn.cantrill.io/courses/730712/lectures/14499321

**AWS docs:**

- [Architecture with an internet gateway and a NAT gateway](https://docs.aws.amazon.com/network-firewall/latest/developerguide/arch-igw-ngw.html)

___

## Network Address Translation (NAT) & NAT Gateway

In this 2-part lesson we step through the architecture of Network Address Translation or (NAT) - what it does, and why it's required within AWS.

and we look at the NAT Gateway service - AWS NAT-as-a-service Gateway Product.

**Link to video:**
- https://learn.cantrill.io/courses/730712/lectures/14419891
- https://learn.cantrill.io/courses/730712/lectures/14499321

**AWS docs:**

- [Architecture with an internet gateway and a NAT gateway](https://docs.aws.amazon.com/network-firewall/latest/developerguide/arch-igw-ngw.html)



# ELASTIC COMPUTE CLOUD (EC2) BASICS
___

## Virtualization

In this lesson, I discussion a few different historical methods of performing virtualisation

Emulated Virtualization
Paravirtualization
Hardware Assisted Virtualization
SR-IOV

Lesson Links

http://www.brendangregg.com/blog/2017-11-29/aws-ec2-virtualization-2017.html


**Link to video:**
- https://learn.cantrill.io/courses/730712/lectures/14549314

**AWS docs:**

- [Linux AMI virtualization types](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/virtualization_types.html)
- [What is Amazon EC2?](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html)
___

## EC2 Architecture and Resilience

This lesson reviews the architecture of EC2

Looking specifically at EC2 Hosts, how they are physically architected, why they are AZ resilient, and how the resilience of the Elastic Block Store (EBS) factors into our decisions as Solutions Architects.

**Link to video:**
- https://learn.cantrill.io/courses/730712/lectures/14549494

**AWS docs:**

- [Resilience in Amazon EC2](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/disaster-recovery-resiliency.html)

___

## EC2 Instance Types

In this lesson I step through the considerations required when a Solutions Architect is picking EC2 instances for a given workload.

I explain EC2 instance Categories, talk about how to decode the instance type names (family, generation, features & size)

and I provide some hints and tips on remembering the Instance type differences.

https://aws.amazon.com/ec2/instance-types/

https://ec2instances.info/


**Link to video:**
- https://learn.cantrill.io/courses/730712/lectures/14550449
- https://learn.cantrill.io/courses/730712/lectures/14550451

___

## Storage Refresher

In this lesson I provide a quick refresher on a few key storage related facts, including:-

Block storage
File storage
Object Storage
IO Block Size
IOPS
Throughput

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14550556

**AWS docs:**

- [Using Amazon S3 storage classes](https://docs.aws.amazon.com/AmazonS3/latest/userguide/storage-class-intro.html)

___

## Elastic Block Store (EBS) Service Architecture

In this lesson I provide a quick refresher on a few key storage related facts, including:-

Block storage
File storage
Object Storage
IO Block Size
IOPS
Throughput

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/29774521

**AWS docs:**

- [Amazon Elastic Block Store (Amazon EBS)](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AmazonEBS.html)
- [Category: Amazon Elastic Block Store (Amazon EBS)](https://aws.amazon.com/blogs/architecture/category/storage/amazon-elastic-block-storage-ebs/)

___

## EBS Volume Types - General Purpose

EBS Provides a number of different volume types, this lesson will be covering :-

General Purpose SSD — Provides a balance of price and performance. We recommend these volumes for most workloads.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/29774522

**AWS docs:**

- [Amazon Elastic Block Store (Amazon EBS)](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AmazonEBS.html)
- [Category: Amazon Elastic Block Store (Amazon EBS)](https://aws.amazon.com/blogs/architecture/category/storage/amazon-elastic-block-storage-ebs/)

___

## EBS Volume Types - Provisioned IOPS

EBS Provides a number of different volume types, this lesson will be covering :-

Provisioned IOPS SSD — Provides high performance for mission-critical, low-latency, or high-throughput workloads.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/29774523

**AWS docs:**

- [Amazon Elastic Block Store (Amazon EBS)](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AmazonEBS.html)
- [Category: Amazon Elastic Block Store (Amazon EBS)](https://aws.amazon.com/blogs/architecture/category/storage/amazon-elastic-block-storage-ebs/)


___

## EBS Volume Types - HDD-Based

EBS Provides a number of different volume types, this lesson will be covering :-

Throughput Optimized HDD — A low-cost HDD designed for frequently accessed, throughput-intensive workloads.
Cold HDD — The lowest-cost HDD design for less frequently accessed workloads.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/29774524

**AWS docs:**

- [Amazon Elastic Block Store (Amazon EBS)](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AmazonEBS.html)
- [Category: Amazon Elastic Block Store (Amazon EBS)](https://aws.amazon.com/blogs/architecture/category/storage/amazon-elastic-block-storage-ebs/)

___

## Instance Store Volumes - Architecture

An instance store provides temporary block-level storage for your instance. This storage is located on disks that are physically attached to the host computer. Instance store is ideal for temporary storage of information that changes frequently, such as buffers, caches, scratch data, and other temporary content, or for data that is replicated across a fleet of instances, such as a load-balanced pool of web servers.

An instance store consists of one or more instance store volumes exposed as block devices. The size of an instance store as well as the number of devices available varies by instance type.

The virtual devices for instance store volumes are `ephemeral[0-23]`. Instance types that support one instance store volume have `ephemeral0`. Instance types that support two instance store volumes have `ephemeral0` and `ephemeral1`, and so on.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/29774525

**AWS docs:**

- [Amazon EC2 instance store](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html)

___

## Choosing between the EC2 Instance Store and EBS

In this exam focused lesson I provide some suggestions on when to pick EBS over EC2 Instance Store and vice-versa.

Exam questions regularly test the ability to pick between the two so understanding the criteria is important to do well

https://aws.amazon.com/ec2/instance-types/

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14561544

___

## Snapshots, Restore & Fast Snapshot Restore (FSR)

EBS Snapshots are backups of data consumed within EBS Volumes - Stored on S3.

Snapshots are incremental, the first being a full backup - and any future snapshots being incremental.

Snapshots can be used to migrate data to different availability zones in a region, or to different regions of AWS.

This lesson steps through the theory and architecture of EBS Snapshots.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14576025

**AWS docs:**

- [Amazon EBS fast snapshot restore](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-fast-snapshot-restore.html)

___

## EBS Encryption

In this lesson I talk about EBS Volume encryption. We look at the architecture, the flow of the encryption process and security of the data encryption keys.

In the second part of the lesson, i demonstrate how to interact with EBS from an encryption perspective in the console UI.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14576061

**AWS docs:**

- [Amazon EBS encryption](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSEncryption.html)

___

## EBS Encryption

In this lesson I talk about EBS Volume encryption. We look at the architecture, the flow of the encryption process and security of the data encryption keys.

In the second part of the lesson, i demonstrate how to interact with EBS from an encryption perspective in the console UI.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14576061

**AWS docs:**

- [Amazon EBS encryption](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSEncryption.html)

___

## EC2 Purchase Options

This two-part lesson steps through a number of different EC2 purchase options, explaining their mechanics and the type of situations they should be used in

On-Demand
Spot
Reserved
Dedicated Instance
Dedicated host

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36046909
- https://learn.cantrill.io/courses/730712/lectures/36046913

**AWS docs:**

- [Instance purchasing options](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instance-purchasing-options.html)

___

## EC2 Purchase Options

This lesson looks at Scheduled Reserved Instances, the differences between zonal and regional reservations and on-demand capacity Reservations.

Each of these are essential cost control and capacity control features you need to understand at the pro level.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36046914

**AWS docs:** 

- [Reserved Instances](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-reserved-instances.html)
- [Reserved Instances (RIs)](https://aws.amazon.com/aws-cost-management/aws-cost-optimization/reserved-instances/)

___

## Instance Status Checks & Auto Recovery

With instance status monitoring, you can quickly determine whether Amazon EC2 has detected any problems that might prevent your instances from running applications. Amazon EC2 performs automated checks on every running EC2 instance to identify hardware and software issues. You can view the results of these status checks to identify specific and detectable problems.

You can create an Amazon CloudWatch alarm that monitors an Amazon EC2 instance and automatically recovers the instance if it becomes impaired due to an underlying hardware failure or a problem that requires AWS involvement to repair. Terminated instances cannot be recovered. A recovered instance is identical to the original instance, including the instance ID, private IP addresses, Elastic IP addresses, and all instance metadata

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-recover.html

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14616991

**AWS docs:** 

- [Status checks for your instances](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/monitoring-system-instance-status-check.html)
- [Recover your instance](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-recover.html)

___

## Horizontal & Vertical Scaling

Within AWS Horizontal and Vertical scaling are two ways which systems have to deal with increasing or decreasing user-side load.

Each has pros and cons but handles the act of scaling radically differently.

This lesson provides a high level overview of the differences, pros and cons of each.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14617207

**AWS docs:** 

- [Dynamic scaling for Amazon EC2 Auto Scaling](https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-scale-based-on-demand.html)


# CONTAINERS & ECS
___

## Introduction to Containers

To understand the AWS container products requires an appreciation of containerization in general.

In this lesson I step through container computing, container images, fs layers, containers, and container registries.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14639197

**AWS docs:** 

- [Containers](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/containers.html)

___

## ECS - Concepts

In this video I step through the key ECS concepts.

I talk briefly about clusters, container definitions, task definitions and service definitions.

https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_ContainerDefinition.html

https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_TaskDefinition.html

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14640456

**AWS docs:** 

- [What is Amazon Elastic Container Service?](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/Welcome.html)

___

## ECS - Cluster Mode

ECS is capable of running in EC2 mode or Fargate mode.

EC2 mode deploys EC2 instances into your AWS account which can be used to deploy tasks and services.

With EC2 mode you pay for the EC2 instances regardless of container usage

Fargate mode uses shared AWS infrastructure, and ENI's which are injected into your VPC

You pay only for container resources used while they are running.

This lesson steps through the key architectures of both.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14640457

**AWS docs:**

[Amazon ECS clusters](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/clusters.html)


# ADVANCED EC2
___

## Bootstrapping EC2 using User Data

EC2 Bootstrapping is the process of configuring an EC2 instance to perform automated install & configuration steps 'post launch' before an instance is brought into service.

With EC2 this is accomplished by passing a script via the User Data part of the Meta-data service - which is then executed by the EC2 Instance OS

In this lesson I step through the architecture and some key concepts

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14679949

**AWS docs:**

[Bootstrapping container instances with Amazon EC2 user data](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/bootstrap_container_instance.html)

___

## Enhanced Bootstrapping with CFN-INIT

CFN-INIT is a powerful desired-state-like configuration engine which is part of the CFN suite of products.

It allows you to set a state for things like packages, users, groups, sources and files within resources inside a template - and it will make that change happen on the instance, performing whatever actions are required.

Creation policies create a 'WAIT STATE' on resources .. not allowing the resource to move to CREATE_COMPLETE until signalled using the cfn-signal tool.

This lesson covers the CFN-INIT and CFN-SIGNAL architectures.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14679968

**AWS docs:**

[Bootstrapping AWS CloudFormation Windows stacks](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/cfn-windows-stacks-bootstrapping.html)

___

## EC2 Instance Roles & Profile

EC2 Instance roles and Instance Profiles are how applications running on an EC2 instance can be given permissions to access AWS resources on your behalf.

Short Term Temporary credentials are available via the EC2 Instance Metadata and are renewed automatically by the EC2 and STS Services.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14679977

**AWS docs:**

[Bootstrapping AWS CloudFormation Windows stacks](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/cfn-windows-stacks-bootstrapping.html)

___

## SSM Parameter Store

The SSM Parameter store is a service which is part of Systems Manager which allows the storage and retrieval of parameters - string, stringlist or secure string.

The service supports encryption which integrates with KMS, versioning and can be secured using IAM.

The service integrates natively with many AWS services - and can be accessed using the CLI/APIs from anywhere with access to the AWS Public Spare Endpoints.

**Link to video:**

https://learn.cantrill.io/courses/730712/lectures/14726329

**AWS docs:**

- [AWS Systems Manager Parameter Store](https://docs.aws.amazon.com/systems-manager/latest/userguide/systems-manager-parameter-store.html)

___

## System and Application Logging on EC2

In this lesson we learn about the CloudWatch agent - which is capable of adding internal instance metrics and logging collection and injection.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14727078

**AWS docs:**

[Amazon Elastic Compute Cloud (Amazon EC2) - system level logs](https://docs.aws.amazon.com/managedservices/latest/userguide/access-to-logs-ec2.html)

___

## EC2 Placement Groups

In this lesson we step through the architecture, benefits and limitations of the three placement groups available within AWS :

Cluster Placement Groups (PERFORMANCE)
Spread Placement Groups (Resilience)
Partition Placement Groups (Topology Awareness)

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/placement-groups.html

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36047393

**AWS docs:**

[Placement groups](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/placement-groups.html)

___

## Dedicated Hosts

Dedicated hosts are EC2 Hosts which support a certain type of instance which are dedicated to your account.

You can pay an on-demand or reserved price for the hosts and then you have no EC2 instance pricing to pay for instances running on these dedicated hosts.

Generally dedicated hosts are used for applications which use physical core/socket licensing

https://aws.amazon.com/ec2/dedicated-hosts/pricing/


**Link to video:**

https://learn.cantrill.io/courses/730712/lectures/14727083

___

## Enhanced Networking & EBS Optimized

Enhanced networking is the AWS implementation of SR-IOV, a standard allowing a physical host network card to present many logical devices which can be directly utilized by instances.

This means lower host CPU usage, better throughput, lower and consistent latency

EBS optimisation on instances means dedicated bandwidth for storage networking - separate from data networking.

https://docs.aws.amazon.com/AWSEC2/latest/WindowsGuide/enhanced-networking.html

**Link to video:**

https://learn.cantrill.io/courses/730712/lectures/14760364


# Route 53 - Global DNS

___

## R53 Public Hosted Zones

A public hosted zone is a container that holds information about how you want to route traffic on the internet for a specific domain which is accessible from the public internet

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/28015249

**AWS docs:** 

- [Working with public hosted zones](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/AboutHZWorkingWith.html)

___

## R53 Private Hosted Zones

A private hosted zone is a container that holds information about how you want Amazon Route 53 to respond to DNS queries for a domain and its subdomains within one or more VPCs that you create with the Amazon VPC service

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/28015250

**AWS docs:** 

- [Working with private hosted zones](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/hosted-zones-private.html)

___

## CNAME vs R53 Alias

The differences between CNAME and ALIAS and when to use one v's the other.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/28015254

**AWS docs:** 

- [Using custom URLs by adding alternate domain names (CNAMEs)](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/CNAMEs.html)
- [Choosing between alias and non-alias records](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/resource-record-sets-choosing-alias-non-alias.html)

___

## Simple Routing

Simple routing lets you configure standard DNS records, with no special Route 53 routing such as weighted or latency. With simple routing, you typically route traffic to a single resource, for example, to a web server for your website.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/28015256

**AWS docs:** 

- [Simple routing](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy-simple.html)

___

## R53 Health Checks

Amazon Route 53 health checks monitor the health and performance of your web applications, web servers, and other resources. Each health check that you create can monitor one of the following:

- The health of a specified resource, such as a web server
- The status of other health checks
- The status of an Amazon CloudWatch alarm

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/28015257

**AWS docs:** 

- [Creating Amazon Route 53 health checks and configuring DNS failover](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/dns-failover.html)

___

## Failover Routing

Failover routing lets you route traffic to a resource when the resource is healthy or to a different resource when the first resource is unhealthy

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/28015259

**AWS docs:** 

- [Configuring DNS failover](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/dns-failover-configuring.html)

___

## Multi Value Routing

Multivalue answer routing lets you configure Amazon Route 53 to return multiple values, such as IP addresses for your web servers, in response to DNS queries. You can specify multiple values for almost any record, but multivalue answer routing also lets you check the health of each resource, so Route 53 returns only values for healthy resources

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/28015261

**AWS docs:** 

- [Multivalue answer routing](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy-multivalue.html)

___

## Weighted Routing

Weighted routing lets you associate multiple resources with a single domain name (catagram.io) and choose how much traffic is routed to each resource. This can be useful for a variety of purposes, including load balancing and testing new versions of software.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/28015261

**AWS docs:** 

- [Weighted routing](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy-weighted.html)

___

## Latency Routing

If your application is hosted in multiple AWS Regions, you can improve performance for your users by serving their requests from the AWS Region that provides the lowest latency.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/28015264

**AWS docs:** 

- [Latency-based routing](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy-latency.html)

___

## Geolocation Routing

Geolocation routing lets you choose the resources that serve your traffic based on the geographic location of your users, meaning the location that DNS queries originate from. 

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/28015269

**AWS docs:** 

- [Geolocation Routing](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy-geo.html)

___

## Geoproximity

Geoproximity routing lets Amazon Route 53 route traffic to your resources based on the geographic location of your users and your resources. You can also optionally choose to route more traffic or less to a given resource by specifying a value, known as a bias. A bias expands or shrinks the size of the geographic region from which traffic is routed to a resource.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/28015271

**AWS docs:** 

- [Geoproximity routing (traffic flow only)](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy-geoproximity.html)

___

## R53 Interoperability

This lesson details how Route53 provides Registrar and DNS Hosting features and steps through architectures where it is used for BOTH, or only one of those functions - and how it integrates with other registrars or DNS hosting.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/28015272

**AWS docs:** 

- [Supported DNS record types](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/ResourceRecordTypes.html)



# Relational Database Service (RDS)


___

## Database Refresher & MODELS - PART1 - SQL

This 2-part lesson steps through some DB fundamentals with Part 1 focussing on the architectural fundamentals of Relational Database systems - looking at tables and how data is structured.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14831877

**AWS docs:** 

- [Amazon Relational Database Service](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html)

___

## Database Refresher & MODELS - PART2 - NoSQL

Part 2 steps through some alternative database models - and some potential scenarios where they might be used

- Key-Value
- Wide Column
- Document
- Column Databases
- Graph

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14831884

**AWS docs:** 

- [What is NoSQL?](https://aws.amazon.com/nosql/)

___

## ACID vs BASE

This lesson steps through the ACID and BASE Database transaction models and introduces the CAP Theorem

- https://en.wikipedia.org/wiki/CAP_theorem

- https://en.wikipedia.org/wiki/ACID#Consistency

- https://en.wikipedia.org/wiki/Eventual_consistency

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/30062911

**AWS docs:** 

- [Managing complex workflows with DynamoDB transactions](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/transactions.html)
- [Using Athena ACID transactions](https://docs.aws.amazon.com/athena/latest/ug/acid-transactions.html)

___

## Databases on EC2

This lesson steps through the architecture of running DB's on EC2. The lesson reviews the reasons FOR and AGAINST running DBMS systems directly on EC2.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14835740

**AWS docs:** 

- [Choosing between Amazon EC2 and Amazon RDS](https://docs.aws.amazon.com/prescriptive-guidance/latest/migration-sql-server/comparison.html)

___

## Relational Database Service (RDS) Architecture

The Relational Database Service (RDS) is a Database(server) as a service product from AWS which allows the creation of managed databases instances.

This lesson steps through the high level architecture of the product and details what engines are supported, the access methods and some other key concepts.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14899227

**AWS docs:** 

- [What is Amazon Relational Database Service (Amazon RDS)?](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html)

___

## RDS High-Availability (Multi AZ)

MultiAZ is a feature of RDS which provisions a standby replica which is kept in sync Synchronously with the primary instance.

The standby replica cannot be used for any performance scaling ... only availability.

Backups, software updates and restarts can take advantage of MultiAZ to reduce user disruption.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14923950

**AWS docs:** 

- [Multi-AZ deployments for high availability](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.MultiAZ.html)
- [Amazon RDS Multi-AZ](https://aws.amazon.com/rds/features/multi-az/)

___

## RDS Automatic Backup, RDS Snapshots and Restore

RDS is capable of performing Manual Snapshots and Automatic backups

Manual snapshots are performed manually and live past the termination of an RDS instance

Automatic backups can be taken of an RDS instance with a 0 (Disabled) to 35 Day retention.

Automatic backups also use S3 for storing transaction logs every 5 minutes - allowing for point in time recovery.

Snapshots can be restored .. but create a new RDS instance.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14923952

**AWS docs:** 

- [Backing up and restoring an Amazon RDS DB instance](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_CommonTasks.BackupRestore.html)

___

## RDS Read-Replicas

RDS Read Replicas can be added to an RDS Instance - 5 direct per primary instance.

They can be in the same region, or cross-region replicas.

They provide read performance scaling for the instance, but also offer low RTO recovery for any instance failure issues

N.B they don't help with data corruption as the corruption will be replicated to the RR.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14923953

**AWS docs:** 

- [Amazon RDS Read Replicas](https://aws.amazon.com/rds/features/read-replicas/)
- [Working with read replicas](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_ReadRepl.html)

___

## RDS Data Security

This lesson steps through RDS Encryption at rest and RDS IAM authentication

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/27570953

**AWS docs:** 

- [Security in Amazon RDS](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/UsingWithRDS.html)

___

## Aurora Architecture

Aurora is a AWS designed database engine officially part of RDS

Aurora implements a number of radical design changes which offer significant performance and feature improvements over other RDS database engines.

This lesson steps through the changes introduced with the Aurora architecture.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14923964

**AWS docs:** 

- [What is Amazon Aurora?](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/CHAP_AuroraOverview.html)

___

## Aurora Serverless

This lesson reviews the architecture of Aurora Serverless and compares it against Aurora Provisioned.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14954142

**AWS docs:** 

- [Using Aurora Serverless v2](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/aurora-serverless-v2.html)

___

## Aurora Global Database

Aurora global databases are a feature of Aurora Provisioned clusters which allow data to be replicated globally providing significant RPO and RTO improvements for BC and DR planning. Additionally global databases can provide performance improvements for customers .. with data being located closer to them, in a read-only form.

Replication occurs at the storage layer and is generally ~1second between all AWS regions

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14954149

**AWS docs:** 

- [Using Amazon Aurora global databases](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/aurora-global-database.html)

___

## Aurora Multi-master writes

Multi-master write is a mode of Aurora Provisioned Clusters which allows multiple instances to perform reads and writes at the same time - rather than only one primary instance having write capability in a single-master cluster. This lesson steps through the architecture and explains how the conflict resolution works.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14954151

**AWS docs:** 

- [Working with Aurora multi-master clusters](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/aurora-multi-master.html)

___

## Database Migration Service (DMS)

The Database Migration Service (DMS) is a managed service which allows for 0 data loss, low or 0 downtime migrations between 2 database endpoints.

The service is capable of moving databases INTO or OUT of AWS.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15747976

**AWS docs:** 

- [What is AWS Database Migration Service?](https://docs.aws.amazon.com/dms/latest/userguide/Welcome.html)



# NETWORK STORAGE & DATA LIFECYCLE


___

## EFS Architecture

The Elastic File System (EFS) is an AWS managed implementation of NFS which allows for the creation of shared 'filesystems' which can be mounted within multi EC2 instances.

EFS can play an essential part in building scalable and resilient syste

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14990550

**AWS docs:** 

- https://en.wikipedia.org/wiki/File_system_permissions

- https://docs.aws.amazon.com/efs/latest/ug/performance.html

- https://docs.aws.amazon.com/efs/latest/ug/storage-classes.html

- https://docs.aws.amazon.com/efs/latest/ug/lifecycle-management-efs.html



# HA & SCALING

___

## Regional and Global AWS Architecture

This lesson steps through the high level components and considerations of AWS architecture.

It introduces global and regional perspectives and the tiers or components which make up most applications.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36048264

**AWS docs:** 

- [Regions and Availability Zones](https://aws.amazon.com/about-aws/global-infrastructure/regions_az/)


___

## Elastic Load Balancer

The Elastic Load Balancer (ELB) was introduced in 2009 with the 'now called' Classic Load Balancer

Two new versions the v2 Application and v2 Network load balancers are now the recommended solutions.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36048303
- https://learn.cantrill.io/courses/730712/lectures/36048304
- https://learn.cantrill.io/courses/730712/lectures/36048305

**AWS docs:** 

- [What is an Application Load Balancer?](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/introduction.html)

___

## Application Load balancing (ALB) vs Network Load Balancing (NLB)

This lesson steps through the main features and some important considerations when using Application Load Balancers and Network Load Balancers

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36048307

**AWS docs:** 

- [Network Load Balancers](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html)

___

## Launch Configuration and Templates

Launch Configurations and Launch Templates provide the WHAT to Auto scaling groups.

They define WHAT gets provisioned

The AMI, the Instance Type, the networking & security, the key pair to use, the userdata to inject and IAM Role to attach.

This lesson steps through briefly how they both work.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36048308

**AWS docs:** 

- [Launch configurations](https://docs.aws.amazon.com/autoscaling/ec2/userguide/launch-configurations.html)
- [Launch templates](https://docs.aws.amazon.com/autoscaling/ec2/userguide/launch-templates.html)

___

## Auto-Scaling Groups

An Auto Scaling group contains a collection of Amazon EC2 instances that are treated as a logical grouping for the purposes of automatic scaling and management. An Auto Scaling group also enables you to use Amazon EC2 Auto Scaling features such as health check replacements and scaling policies. Both maintaining the number of instances in an Auto Scaling group and automatic scaling are the core functionality of the Amazon EC2 Auto Scaling service.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36048316

**AWS docs:** 

- [Auto Scaling groups](https://docs.aws.amazon.com/autoscaling/ec2/userguide/auto-scaling-groups.html)

___

## ASG Scaling Policies

With step scaling and simple scaling, you choose scaling metrics and threshold values for the CloudWatch alarms that trigger the scaling process. You also define how your Auto Scaling group should be scaled when a threshold is in breach for a specified number of evaluation periods.

Step scaling policies and simple scaling policies are two of the dynamic scaling options available for you to use. Both require you to create CloudWatch alarms for the scaling policies. Both require you to specify the high and low thresholds for the alarms. Both require you to define whether to add or remove instances, and how many, or set the group to an exact size. 

The main difference between the policy types is the step adjustments that you get with step scaling policies. When step adjustments are applied, and they increase or decrease the current capacity of your Auto Scaling group, the adjustments vary based on the size of the alarm breach.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36048317

**AWS docs:** 

- [Step and simple scaling policies for Amazon EC2 Auto Scaling](https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-scaling-simple-step.html)

___

## ASG Lifecycle Hooks

Lifecycle hooks enable you to perform custom actions by pausing instances as an Auto Scaling group launches or terminates them. When an instance is paused, it remains in a wait state either until you complete the lifecycle action using the complete-lifecycle-action command or the ```CompleteLifecycleAction``` operation, or until the timeout period ends (one hour by default).

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36048319

**AWS docs:** 

- [Amazon EC2 Auto Scaling lifecycle hooks](https://docs.aws.amazon.com/autoscaling/ec2/userguide/lifecycle-hooks.html)

___

## ASG HealthCheck Comparison - EC2 vs ELB

Amazon EC2 Auto Scaling can determine the health status of an instance using one or more of the following:

- Status checks provided by Amazon EC2 to identify hardware and software issues that may impair an instance. The default health checks for an Auto Scaling group are EC2 status checks only.

- Health checks provided by Elastic Load Balancing (ELB). These health checks are disabled by default but can be enabled.

- Your custom health checks.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36048320

**AWS docs:** 

- [Add Elastic Load Balancing health checks to an Auto Scaling group](https://docs.aws.amazon.com/autoscaling/ec2/userguide/as-add-elb-healthcheck.html)
- [Health checks for Auto Scaling instances](https://docs.aws.amazon.com/autoscaling/ec2/userguide/ec2-auto-scaling-health-checks.html)

__

## SSL Offload & Session Stickiness

This lesson steps through 3 different ways that ELB's can handle SSL

SSL Bridging
SSL Pass Through
SSL Offloading
Additionally the lesson steps through what session stickiness means, and why it matters to the solutions we design as solutions architects.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15828867

**AWS docs:** 

- [Configure sticky sessions for your Classic Load Balancer](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/sticky-sessions.html)
- [Sticky sessions for your Application Load Balancer](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/sticky-sessions.html)
  

___

## Gateway Load Balancer

Gateway Load Balancers enable you to deploy, scale, and manage virtual appliances, such as firewalls, intrusion detection and prevention systems, and deep packet inspection systems. It combines a transparent network gateway (that is, a single entry and exit point for all traffic) and distributes traffic while scaling your virtual appliances with the demand.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/34350240

**AWS docs:** 

- [What is a Gateway Load Balancer?](https://docs.aws.amazon.com/elasticloadbalancing/latest/gateway/introduction.html)



# SERVERLESS AND APPLICATION SERVICES

___

## Architecture Deep Dive - PART1 and PART2

In PART1 of this lesson I step through how a video uploading architecture 'CatTube' can be evolved from monolithic to tiered.

Part 2 continues by looking at evolutions using a queue based design, to achieve improved asynchronous communications and scaling and finishes by looking at microservices and event driven architectures.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15190436
- https://learn.cantrill.io/courses/730712/lectures/15190450

**AWS docs:** 

- [AWS Well-Architected Framework](https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html)

___

## AWS Lambda

This 3-part series steps through Lambdas architecture and features in depth.

Part 1 is a refresher of the topics covered at an associate level with some additional detail

Part 2 looks at public & VPC networking, security and logging

Part 3 looks at invocation modes, versions & aliases, Latency, destinations and execution context

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36049038
- https://learn.cantrill.io/courses/730712/lectures/36049039
- https://learn.cantrill.io/courses/730712/lectures/36049040

**AWS docs:** 

- [Lambda instruction set architectures](https://docs.aws.amazon.com/lambda/latest/dg/foundation-arch.html)

___

## CloudWatchEvents and EventBridge

CloudWatch Events and EventBridge have visibility over events generated by supported AWS services within an account.

They can monitor the default account event bus - and pattern match events flowing through and deliver these events to multiple targets.

They are also the source of scheduled events which can perform certain actions at certain times of day, days of the week, or multiple combinations of both - using the Unix CRON time expression format.

Both services are one way how event driven architectures can be implemented within AWS.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15191500

**AWS docs:** 

- [What Is Amazon CloudWatch Events?](https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/WhatIsCloudWatchEvents.html)

- [What Is Amazon EventBridge?](https://docs.aws.amazon.com/eventbridge/latest/userguide/eb-what-is.html)


___
 
## Serverless Architecture

The Serverless architecture is a evolution/combination of other popular architectures such as event-driven and microservices.

It aims to use 3rd party services where possible and FAAS products for any on-demand computing needs.

Using a serverless architecture means little to no base costs for an environment - and any cost incurred during operations scale in a way with matches the incoming load.

Serverless starts to feature more and more on the AWS exams - so its a critical architecture to understand.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15267917

**AWS docs:** 

- [AWS Serverless Multi-Tier Architectures with Amazon API Gateway and AWS Lambda](https://docs.aws.amazon.com/whitepapers/latest/serverless-multi-tier-architectures-api-gateway-lambda/welcome.html)

___
 
## Simple Notification Service

The Simple Notification Service or SNS .. is a PUB SUB style notification system which is used within AWS products and services but can also form an essential part of serverless, event-driven and traditional application architectures.

Publishers send messages to TOPICS

Subscribers receive messages SENT to TOPICS.

SNS supports a wide variety of subscriber types including other AWS services such as LAMBDA and SQS

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15267920

**AWS docs:** 

- [What is Amazon SNS?](https://docs.aws.amazon.com/sns/latest/dg/welcome.html)

___
 
## Step Functions

Step functions is a product which lets you build long running serverless workflow based applications within AWS which integrate with many AWS services.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15267923

**AWS docs:** 

- [What is AWS Step Functions?](https://docs.aws.amazon.com/step-functions/latest/dg/welcome.html)

___
 
## API Gateway

API Gateway is a managed service from AWS which allows the creation of API Endpoints, Resources & Methods.

The API gateway integrates with other AWS services - and can even access some without the need for dedicated compute.

It serves as a core component of many serverless architectures using Lambda as event-driven and on-demand backing for methods.

It can also connect to legacy monolithic applications and act as a stable API endpoint during an evolution from a monolith to microservices and potentially through to serverless.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15267912

**AWS docs:** 

- [What is Amazon API Gateway?](https://docs.aws.amazon.com/apigateway/latest/developerguide/welcome.html)

___
 
## Simple Queue Service

SQS queues are a managed message queue service in AWS which help to decouple application components, allow Asynchronous messaging or the implementation of worker pools.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15267945

**AWS docs:** 

- [What is Amazon Simple Queue Service?](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/welcome.html)

___
 
## Kinesis Data Streams

Kinesis data streams are a streaming service within AWS designed to ingest large quantities of data and allow access to that data for consumers.

Kinesis is ideal for dashboards and large scale real time analytics needs.

Kinesis data firehose allows the long term persistent storage of kinesis data onto services like S3

This lesson ends by evaluating the differences between SQS and Kinesis, and identifying key factors in exam questions which suggest picking one vs the other.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36049059

**AWS docs:** 

- [What Is Amazon Kinesis Data Streams?](https://docs.aws.amazon.com/streams/latest/dev/introduction.html)

___
 
## Kinesis Data Firehose

Kinesis Data Firehose is a stream based delivery service capable of delivering high throughput streaming data to supported destinations in near realtime.

Its a member of the kinesis family and for the PRO level exam it's critical to have a good understanding of how it functions in isolation and how it integrates with AWS products and services.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36049060

**AWS docs:** 

- [What Is Amazon Kinesis Data Firehose?](https://docs.aws.amazon.com/firehose/latest/dev/what-is-this-service.html)

___
 
## Kinesis Data Analytics

Amazon Kinesis Data Analytics is the easiest way to analyze streaming data, gain actionable insights, and respond to your business and customer needs in real time.

it is part of the kinesis family of products and is capable of operating in realtime on high throughput streaming data.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36049063

**AWS docs:** 

- [What Is Amazon Kinesis Data Analytics for SQL Applications?](https://docs.aws.amazon.com/kinesisanalytics/latest/dev/what-is.html)

___
 
## Amazon Cognito - User and Identity Pools

A user pool is a user directory in Amazon Cognito. With a user pool, your users can sign in to your web or mobile app through Amazon Cognito. Your users can also sign in through social identity providers like Google, Facebook, Amazon, or Apple, and through SAML identity providers. Whether your users sign in directly or through a third party, all members of the user pool have a directory profile that you can access through a Software Development Kit (SDK).

Amazon Cognito identity pools (federated identities) enable you to create unique identities for your users and federate them with identity providers. With an identity pool, you can obtain temporary, limited-privilege AWS credentials to access other AWS services. 

This lesson reviews the features of the product and talks through some example architectures.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/32121076

**AWS docs:** 

- [What is Amazon Cognito?](https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html)



# GLOBAL CONTENT DELIVERY AND OPTIMIZATION


___
 
## Cloudfront Architecture

CloudFront is a Content Delivery network (CDN) within AWS.

This lesson steps through the basic architecture

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36049951

**AWS docs:** 

- [What is Amazon CloudFront?](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html)


___
 
## Cloudfront Behaviours

CloudFront Behaviours control much of the TTL, protocol and privacy settings within CloudFront

This lesson steps through settings configured at a distribution level and those settings which apply to a distribution

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36049952

**AWS docs:** 

- [What is Amazon CloudFront?](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html)

___
 
## CF TTL and Invalidations

This lesson steps through how CloudFront handles object expiry and invalidation

Covering

Default TTL, Minimum TTL, Maximum TTL

And Cache Invalidation


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36049953

**AWS docs:** 

- [How CloudFront processes and caches HTTP 4xx and 5xx status codes from your origin](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/HTTPStatusCodes.html)

___
 
## ACM

The AWS certificate Manage is a service which allows the creation, management and renewal of certificates. It allows deployment of certificates onto supported AWS services such as CloudFront and ALB.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15356375

**AWS docs:** 

- [What Is AWS Certificate Manager?](https://docs.aws.amazon.com/acm/latest/userguide/acm-overview.html)

___
 
## Cloudfront and SSL/TLS

Understanding CloudFront and SSL is essential for the exam

This lesson steps through the certificate requirements for the viewer and origin side and steps through the reasons for SNI, and how it works.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36049954

**AWS docs:** 

- [Requirements for using SSL/TLS certificates with CloudFront](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/cnames-and-https-requirements.html)

___
 
## Origin Types & Origin Architecture

CloudFront origins store content distributed via edge locations.

The features available differ based on using S3 origins vs Custom origins

Supported SSL/TLS protocols and ciphers for communication between viewers and CloudFront


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36049955

**AWS docs:** 

- [Origin](https://docs.aws.amazon.com/cloudfront/latest/APIReference/API_Origin.html)
- [Supported protocols and ciphers between viewers and CloudFront](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/secure-connections-supported-viewer-protocols-ciphers.html#secure-connections-supported-ciphers)

___
 
## Securing CF and S3 using OAI

Origin Access Identities are a feature where virtual identities can be created, associated with a CloudFront Distribution and deployed to edge locations.

Access to an s3 bucket can be controlled by using these OAI's - allowing access from an OAI, and using an implicit DENY for everything else.

They are generally used to ensure no direct access to S3 objects is allowed when using private CF Distributions.

This lesson covers the main ways to secure origins from direct access (bypassing CloudFront)

- Origin Access identities (OAI) - for S3 Origins
- Custom Headers - For Custom Origins
- IP Based FW Blocks - For Custom Origins.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15356377

**AWS docs:** 

- [Restricting access to Amazon S3 content by using an origin access identity (OAI)](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/private-content-restricting-access-to-s3.html)

___
 
## Lambda@Edge

Lambda@Edge allows cloudfront to run lambda function at CloudFront edge locations to modify traffic between the viewer and edge location and edge locations and origins.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/22696404

**AWS docs:** 

- [Personalize content by country or device type headers - examples](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/lambda-examples.html#lambda-examples-redirecting-examples)


___

## Global Accelerator

AWS Global Accelerator is designed to improve global network performance by offering entry point onto the global AWS transit network as close to customers as possible using ANycast IP addresses

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15790988

**AWS docs:** 

- [What is AWS Global Accelerator?](https://docs.aws.amazon.com/global-accelerator/latest/dg/what-is-global-accelerator.html)


# VPC Flow Logs

___

## VPC Flow Logs

VPC Flow logs is a feature allowing the monitoring of traffic flow to and from interfaces within a VPC

VPC Flow logs can be added at a VPC, Subnet or Interface level.

Flow Logs DON'T monitor packet contents ... that requires a packet sniffer.

Flow Logs can be stored on S3 or CloudWatch Logs

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15443338

**AWS docs:** 

- [Publish flow logs to Amazon S3](https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs-s3.html)
- [Publish flow logs to CloudWatch Logs](https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs-cwl.html)

___

## Egress-Only Internet gateway

Egress-Only internet gateways allow outbound (and response) only access to the public AWS services and Public Internet for IPv6 enabled instances or other VPC based services.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15443339

**AWS docs:** 

- [Enable outbound IPv6 traffic using an egress-only internet gateway](https://docs.aws.amazon.com/vpc/latest/userguide/egress-only-internet-gateway.html)

___

## VPC Endpoints (Gateway)

Gateway endpoints are a type of VPC endpoint which allow access to S3 and DynamoDB without using public addressing.

Gateway endpoints add 'prefix lists' to route table, allowing the VPC router to direct traffic flow to the public services via the gateway endpoint.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15443340

**AWS docs:** 

- [Enable outbound IPv6 traffic using an egress-only internet gateway](https://docs.aws.amazon.com/vpc/latest/userguide/egress-only-internet-gateway.html)

__

## VPC Endpoints (Interface)

Interface endpoints are used to allow private IP addressing to access public AWS services.

S3 and DynamoDB are handled by gateway endpoints - other supported services are handled by interface endpoints.

Unlike gateway endpoints - interface endpoints are not highly available by default - they are normal VPC network interfaces and should be placed 1 per AZ to ensure full HA.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15443340

**AWS docs:** 

- [Enable outbound IPv6 traffic using an egress-only internet gateway](https://docs.aws.amazon.com/vpc/latest/userguide/egress-only-internet-gateway.html)

___

## VPC Peering

VPC peering is a software define and logical networking connection between two VPC's

They can be created between VPCs in the same or different accounts and the same or different regions.

In this lesson I step through the architectural key points which you'll need to understand for the exam and real world usage.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15443346

**AWS docs:** 

- [What is VPC peering?](https://docs.aws.amazon.com/vpc/latest/peering/what-is-vpc-peering.html)


# HYBRID ENVIRONMENTS AND MIGRATION

___

## Border Gateway Protocol 101

This lesson provides a high level introduction to the Border Gateway Protocol (BGP) which is used by some AWS services such as Direct Connect and Dynamic Site to Site VPNs.

N.B this lesson has been added as an OPTIONAL ADVANCED lesson for any students who want to understand what BGP is - its more toward the PROFESSIONAL level, so if you don't understand it fully ... 

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/20129430

**AWS docs:** 

- [Routing policies and BGP communities](https://docs.aws.amazon.com/directconnect/latest/UserGuide/routing-and-bgp.html)

___

## AWS Site-to-Site VPN

AWS Site-to-Site VPN is a hardware VPN solution which creates a highly available IPSEC VPN between an AWS VPN and external network such as on-premises traditional networks. VPNs are quick to setup vs direct connect, don't offer the same high performance, but do encrypt data in transit. This lesson details the architecture and key concepts you need to be aware of for the exam.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15532724

**AWS docs:** 

- [What is AWS Site-to-Site VPN?](https://docs.aws.amazon.com/vpn/latest/s2svpn/VPC_VPN.html)

___

## Direct Connect

Direct Connect is AWS's physical private link connecting your business premises to its public and private services.

It has many pros and cons vs Site-to-Site VPN and its one of those products which is impossible to DEMO without using.

This lesson attempts to teach you all of the theory and architecture you will need for the exam.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15532730

**AWS docs:** 

- [What is AWS Direct Connect?](https://docs.aws.amazon.com/directconnect/latest/UserGuide/Welcome.html)


___

## Direct Connect Resilience

This lesson steps through the architecture of a few resilient implementations of direct connect, starting with an overview of why the default implementation architecture of direct connect provides no resiience.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/24660629

**AWS docs:** 

- [Resilience in AWS Direct Connect](https://docs.aws.amazon.com/directconnect/latest/UserGuide/disaster-recovery-resiliency.html)

___

## Transit Gateway

The AWS Transit gateway is a network gateway which can be used to significantly simplify networking between VPC's, VPN and Direct Connect.

It can be used to peer VPCs in the same account, different account, same or different region and supports transitive routing between networks.

In this lesson I step through the features which allow for a significant reduction in network complexity.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15532731

**AWS docs:** 

- [What is a transit gateway?](https://docs.aws.amazon.com/vpc/latest/tgw/what-is-transit-gateway.html)

___

## Storage gateway

Storage Gateway is a super flexible hybrid storage appliance.

Its capable of running in 3 modes

FILE

TAPE

VOLUME (Stored or Cached).

Understanding the features of each, and when to use those features is a key part of any hybrid infrastructure questions in the exam

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15532734

**AWS docs:** 

- [What is Amazon S3 File Gateway](https://docs.aws.amazon.com/filegateway/latest/files3/what-is-file-s3.html)

___

## Snowball / Edge / Snowmobile

Snowball, Snowball Edge and Snowmobile are three parts of the same product family designed to allow the physical transfer of data between business locations and AWS.

Knowing which to pick and why is essential for the solutions architect exam .. in this lesson I step through all of the key product family features.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15532735

**AWS docs:** 

- [What Is AWS Snowball Edge?](https://docs.aws.amazon.com/snowball/latest/developer-guide/whatisedge.html)

___

## Directory Service

The Directory service is a product which provides managed directory service instances within AWS

it functions in three modes

- Simple AD - An implementation of Samba 4 (compatibility with basics AD functions)
- AWS Managed Microsoft AD - An actual Microsoft AD DS Implementation
- AD Connector which proxies requests back to an on-premises directory.

This lesson steps through the architecture of the service and explains scenarios where each might be used.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15690951

**AWS docs:** 

- [What is AWS Directory Service?](https://docs.aws.amazon.com/directoryservice/latest/admin-guide/what_is.html)

___

## DataSync

AWS DataSync is a product which can orchestrate the movement of large scale data (amounts or files) from on-premises NAS/SAN into AWS or vice-versa

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15690952

**AWS docs:** 

- [What is AWS DataSync?](https://docs.aws.amazon.com/datasync/latest/userguide/what-is-datasync.html)

___

## FSx for Windows Servers

FSx for Windows Servers provides a native windows file system as a service which can be used within AWS, or from on-premises environments via VPN or Direct Connect

FSx is an advanced shared file system accessible over SMB, and integrates with Active Directory (either managed, or self-hosted).

It provides advanced features such as VSS, Data de-duplication, backups, encryption at rest and forced encryption in transit.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15749267

**AWS docs:** 

- [What is FSx for Windows File Server?](https://docs.aws.amazon.com/fsx/latest/WindowsGuide/what-is.html)

___

## FSx For Lustre

FSx for Lustre is a managed file system which uses the FSx product designed for high performance computing

It delivers extreme performance for scenarios such as Big Data, Machine Learning and Financial Modeling

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/22586267

**AWS docs:** 

- [Aggregate file system performance](https://docs.aws.amazon.com/fsx/latest/LustreGuide/performance.html#fsx-aggregate-perf)



# SECURITY, DEPLOYMENT & OPERATIONS

___

## AWS Secrets Manager

AWS Secrets manager is a product which can manage secrets within AWS. There is some overlap between it and the SSM Parameter Store - but Secrets manager is specialised for secrets.

Additionally Secrets managed is capable of automatic credential rotation using Lambda.

For supported services it can even adjust the credentials of the service itself.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15793908

**AWS docs:** 

- [What is AWS Secrets Manager?](https://docs.aws.amazon.com/secretsmanager/latest/userguide/intro.html)


___

## AWS WAF & Shield

AWS WAF is a web application firewall that helps protect your web applications or APIs against common web exploits that may affect availability, compromise security, or consume excessive resources. AWS WAF gives you control over how traffic reaches your applications by enabling you to create security rules that block common attack patterns, such as SQL injection or cross-site scripting, and rules that filter out specific traffic patterns you define. 

https://aws.amazon.com/waf/pricing/

AWS Shield is a managed Distributed Denial of Service (DDoS) protection service that safeguards applications running on AWS. AWS Shield provides always-on detection and automatic inline mitigations that minimize application downtime and latency, so there is no need to engage AWS Support to benefit from DDoS protection. There are two tiers of AWS Shield - Standard and Advanced.

https://www.cloudflare.com/en-au/learning/ddos/what-is-a-ddos-attack/

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15792890

**AWS docs:** 

- [What are AWS WAF, AWS Shield, and AWS Firewall Manager?](https://docs.aws.amazon.com/waf/latest/developerguide/what-is-aws-waf.html)


___

## CloudHSM

In this lesson I step through the architecture and features of CloudHSM - an AWS provided Hardware Security Module products.

CloudHSM is required to achieve compliance with certain security standards such as FIPS 140-2 Level 3

https://en.wikipedia.org/wiki/FIPS_140-2

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15828633

**AWS docs:** 

- [What is AWS CloudHSM?](https://docs.aws.amazon.com/cloudhsm/latest/userguide/introduction.html)


___

## AWS Config

AWS Config is a service which records the configuration of resources over time (configuration items) into configuration histories.

All the information is stored regionally in an S3 config bucket.

AWS Config is capable of checking for compliance .. and generating notifications and events based on compliance.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/30035588

**AWS docs:** 

- [What Is AWS Config?](https://docs.aws.amazon.com/config/latest/developerguide/WhatIsConfig.html)

___

## Amazon Macie

Amazon Macie is a fully managed data security and data privacy service that uses machine learning and pattern matching to discover and protect your sensitive data in AWS.

This lesson steps through the theory and architecture of the product.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/30036454

**AWS docs:** 

- [Using managed data identifiers in Amazon Macie](https://docs.aws.amazon.com/macie/latest/user/managed-data-identifiers.html)

- [Building custom data identifiers in Amazon Macie](https://docs.aws.amazon.com/macie/latest/user/custom-data-identifiers.html)

- [Types of Amazon Macie findings](https://docs.aws.amazon.com/macie/latest/user/findings-types.html)


___

## Amazon Inspector

Amazon Inspector is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS. Amazon Inspector automatically assesses applications for exposure, vulnerabilities, and deviations from best practices

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36408324

**AWS docs:** 

- [Using managed data identifiers in Amazon Macie](https://docs.aws.amazon.com/macie/latest/user/managed-data-identifiers.html)

___

## Amazon Guardduty

Guard Duty is an automatic threat detection service which reviews data from supported services and attempts to identify any events outside of the 'norm' for a given AWS account or Accounts.

This lesson steps through its capabilities and supported datasources.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36408326

**AWS docs:** 

- [What is Amazon GuardDuty?](https://docs.aws.amazon.com/guardduty/latest/ug/what-is-guardduty.html)


# Infrastructure as Code (CloudFormation)

___

## CloudFormation Physical & Logical Resources 

CloudFormation defines logical resources within templates (using YAML or JSON). The logical resource defines the WHAT, and leaves the HOW up to the CFN product. A CFN stack creates a physical resource for every logical resource - updating or deleting them as a template changes.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204848

**AWS docs:** 

- [What is AWS CloudFormation?](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html)

- [AWS resource and property types reference](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-template-resource-type-ref.html)

___

## CloudFormation Template and Pseudo Parameters

Template and Pseudo Parameters are two methods to provide input to a template, which can influence what resources are provisioned, and the configuration of those resources.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204864

**AWS docs:** 

- [Pseudo parameters reference](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/pseudo-parameter-reference.html)

___

## CloudFormation Intrinsic Functions

AWS CloudFormation provides several built-in functions that help you manage your stacks. Use intrinsic functions in your templates to assign values to properties that are not available until runtime.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204866

**AWS docs:** 

- [ntrinsic function reference](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-reference.html)


___

## CloudFormation Mappings

The optional Mappings section matches a key to a corresponding set of named values. For example, if you want to set values based on a region, you can create a mapping that uses the region name as a key and contains the values you want to specify for each specific region. You use the Fn::FindInMap intrinsic function to retrieve values in a map.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204867

**AWS docs:** 

- [Mapping](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/mappings-section-structure.html)

___

## CloudFormation Outputs

The optional Outputs section declares output values that you can import into other stacks (to create cross-stack references), return in response (to describe stack calls), or view on the AWS CloudFormation console. For example, you can output the S3 bucket name for a stack to make the bucket easier to find

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204867

**AWS docs:** 

- [Outputs](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/outputs-section-structure.html)


___

## CloudFormation Conditions

The optional Conditions section contains statements that define the circumstances under which entities are created or configured. You might use conditions when you want to reuse a template that can create resources in different contexts, such as a test environment versus a production environment. In your template, you can add an EnvironmentType input parameter, which accepts either prod or test as inputs. Conditions are evaluated based on predefined pseudo parameters or input parameter values that you specify when you create or update a stack. Within each condition, you can reference another condition, a parameter value, or a mapping. After you define all your conditions, you can associate them with resources and resource properties in the Resources and Outputs sections of a template

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204873

**AWS docs:**

- [Conditions](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/conditions-section-structure.html)

___

## CloudFormation DependsOn

With the DependsOn attribute you can specify that the creation of a specific resource follows another. When you add a DependsOn attribute to a resource, that resource is created only after the creation of the resource specified in theDependsOn attribute.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204875

**AWS docs:**

- [DependsOn attribute](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-attribute-dependson.html)

___

## CloudFormation Wait Conditions & cfn-signal

CreationPolicy, WaitConditions and cfn-signal can all be used together to prevent the status if a resource from reaching create complete until AWS CloudFormation receives a specified number of success signals or the timeout period is exceeded.The cfn-signal helper script signals AWS CloudFormation to indicate whether Amazon EC2 instances have been successfully created or updated.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204877

**AWS docs:**

- [cfn-signal](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/cfn-signal.html)

- [Creating wait conditions in a template](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-waitcondition.html)

___

## CloudFormation Wait Conditions & cfn-signal

CreationPolicy, WaitConditions and cfn-signal can all be used together to prevent the status if a resource from reaching create complete until AWS CloudFormation receives a specified number of success signals or the timeout period is exceeded.The cfn-signal helper script signals AWS CloudFormation to indicate whether Amazon EC2 instances have been successfully created or updated.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204877

**AWS docs:**

- [cfn-signal](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/cfn-signal.html)

- [Creating wait conditions in a template](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-waitcondition.html)


___

## CloudFormation Nested Stacks

Nested stacks allow for a hierarchy of related templates to be combined to form a single product

A root stack can contain and create nested stacks .. each of which can be passed parameters and provide back outputs.

Nested stacks should be used when the resources being provisioned share a lifecycle and are related.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204881

**AWS docs:**

- [Working with nested stacks](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-nested-stacks.html)

___

## CloudFormation Cross-Stack References

Cross stack references allow one stack to reference another

Outputs in one stack reference logical resources or attributes in that stack

They can be exported, and then using the !ImportValue intrinsic function, referenced from another stack.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204883

**AWS docs:**

- [Walkthrough: Refer to resource outputs in another AWS CloudFormation stack](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/walkthrough-crossstackref.html)

___

## CloudFormation Stack Sets

StackSets are a feature of CloudFormation allowing infrastructure to be deployed and managed across multiple regions and multiple accounts from a single location.

Additionally it adds a dynamic architecture - allowing automatic operations based on accounts being added or removed from the scope of a StackSet.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204885

**AWS docs:**

- [StackSets concepts](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/stacksets-concepts.html)

___

## CloudFormation Deletion Policy

With the DeletionPolicy attribute you can preserve or (in some cases) backup a resource when its stack is deleted. You specify a DeletionPolicy attribute for each resource that you want to control. If a resource has no DeletionPolicy attribute, AWS CloudFormation deletes the resource by default.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204886

**AWS docs:**

- [DeletionPolicy attribute](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-attribute-deletionpolicy.html)

___

## CloudFormation Deletion Policy

Stack roles allow an IAM role to be passed into the stack via PassRole

A stack uses this role, rather than the identity interacting with the stack to create, update and delete AWS resources.

It allows role separation and is a powerful security feature.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204888

**AWS docs:**

- [AWS::CloudFormation::Stack](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-properties-stack.html)

___

## CloudFormation Init (CFN-INIT)

CloudFormationInit and cfn-init are tools which allow a desired state configuration management system to be implemented within CloudFormation

Use the AWS::CloudFormation::Init type to include metadata on an Amazon EC2 instance for the cfn-init helper script. If your template calls the cfn-init script, the script looks for resource metadata rooted in the AWS::CloudFormation::Init metadata key. cfn-init supports all metadata types for Linux systems & It supports some metadata types for Windows

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204888

**AWS docs:**

- [cfn-init](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/cfn-init.html)

___

## CloudFormation cfn-hup

The cfn-hup helper is a daemon that detects changes in resource metadata and runs user-specified actions when a change is detected. This allows you to make configuration updates on your running Amazon EC2 instances through the UpdateStack API action.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204895

**AWS docs:**

- [cfn-hup](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/cfn-hup.html)

- https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html

___

## CloudFormation ChangeSets

When you need to update a stack, understanding how your changes will affect running resources before you implement them can help you update stacks with confidence. Change sets allow you to preview how proposed changes to a stack might impact your running resources, for example, whether your changes will delete or replace any critical resources, AWS CloudFormation makes the changes to your stack only when you decide to execute the change set, allowing you to decide whether to proceed with your proposed changes or explore other changes by creating another change set.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204900

**AWS docs:**

- [Updating stacks using change sets](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-changesets.html)

___

## CloudFormation Custom Resources

Custom resources enable you to write custom provisioning logic in templates that AWS CloudFormation runs anytime you create, update (if you changed the custom resource), or delete stacks

This lesson steps through the theory and architecture of Custom Resources

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/36204902

**AWS docs:**

- [Custom resources](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/template-custom-resources.html)



# NOSQL Databases & DynamoDB


___

## DynamoDB - Architecture

DynamoDB is a NoSQL fully managed Database-as-a-Service (DBaaS) product available within AWS.

In this lesson I step through the key architectural components and features you will need to understand for the exam.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15601347

**AWS docs:**

- [Amazon DynamoDB Architecture Overview](https://docs.aws.amazon.com/whitepapers/latest/comparing-dynamodb-and-hbase-for-nosql/amazon-dynamodb-architecture-overview.html)


___

## DynamoDB - Operations, Consistency and Performance-PART1

IN PART1 of this lesson series I step through some key elements of READS and WRITES to DynamoDB and step through how the QUERY AND SCAN operations work.


**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15601351

**AWS docs:**

- [Amazon DynamoDB: How it works](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.html)


___

## DynamoDB - Operations, Consistency and Performance-PART2

In PART 2 of this lesson series we will step through the Consistency model in DynamoDB and them look at two RCU and WCU calculation examples.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15603829

**AWS docs:**

- [Read consistency](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadConsistency.html)

___

## DynamoDB Local and Global Secondary Indexes

Local Secondary Indexes (LSI) and Global Secondary Indexes (GSI) allow for an alternative presentation of data stored in a base table.

LSI allow for alternative SK's whereas with GSIs you can use alternative PK and SK.

This lesson details the difference between them - and steps through an example way they can help improve database query performance.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15662767

**AWS docs:**

- [Using Global Secondary Indexes in DynamoDB](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/GSI.html)

- [Local Secondary Indexes](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/LSI.html)

___

## DynamoDB - Streams & Lambda Triggers

DynamoDB Streams are a 24 hour rolling window of time ordered changes to ITEMS in a DynamoDB table

Streams have to be enabled on a per table basis , and have 4 view types

KEYS_ONLY

NEW_IMAGE

OLD_IMAGE

NEW_AND_OLD_IMAGES

Lambda can be integrated to provide trigger functionality - invoking when new entries are added on the stream.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15601352

**AWS docs:**

- [DynamoDB Streams and AWS Lambda triggers](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Streams.Lambda.html)

___

## DynamoDB - Global Tables

DynamoDB Global Tables provides multi-master global replication of DynamoDB tables which can be used for performance, HA or DR/BC reasons.

This lesson introduces the architecture and features you will need to understand for the exam.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15662768

**AWS docs:**

- [Amazon DynamoDB global tables](https://aws.amazon.com/dynamodb/global-tables/)

___

## DynamoDB - Accelerator (DAX)

DynamoDB Accelerator (DAX) is an in-memory cache designed specifically for DynamoDB. It should be your default choice for any DynamoDB caching related questions.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15662769

**AWS docs:**

- [Amazon DynamoDB Accelerator (DAX)](https://aws.amazon.com/dynamodb/dax/)
- [In-memory acceleration with DynamoDB Accelerator (DAX)](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DAX.html)

___

## Amazon Athena

Amazon Athena is serverless querying service which allows for ad-hoc questions where billing is based on the amount of data consumed.

Athena is an underrated service capable of working with unstructured, semi-structured or structured data.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/15662776

**AWS docs:**

- [What is Amazon Athena?](https://docs.aws.amazon.com/athena/latest/ug/what-is.html)

___

## Elasticache

Elasticache is a managed in-memory cache which provides a managed implementation of the redis or memcached engines.

its useful for read heavy workloads, scaling reads in a cost effective way and allowing for externally hosted user session state.

https://aws.amazon.com/elasticache/pricing/

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/22586311

**AWS docs:**

- [Comparing Memcached and Redis](https://docs.aws.amazon.com/AmazonElastiCache/latest/red-ug/SelectEngine.html)

___

## Redshift Architecture

Redshift is a column based, petabyte scale, data warehousing product within AWS

Its designed for OLAP products within AWS/on-premises to add data to for long term processing, aggregation and trending

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/24160433

**AWS docs:**

- [Getting started with Amazon Redshift](https://docs.aws.amazon.com/redshift/latest/gsg/getting-started.html)

__

## Redshift DR and Resilience

This lesson steps through in detail the backup options for redshift to overcome the single AZ risk.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/24160434

**AWS docs:**

- [Resilience in Amazon Redshift](https://docs.aws.amazon.com/redshift/latest/mgmt/security-disaster-recovery-resiliency.html)
