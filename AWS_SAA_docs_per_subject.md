

<!-- TOC -->

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

<!-- /TOC -->



<!-- 

#########################################

temlpate:

___

## 



**Link to video:**

- 

**AWS docs:** 

- []()

######################################### 

-->

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