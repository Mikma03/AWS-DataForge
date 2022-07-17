

<!-- TOC -->

- [Theory and AWS docs](#theory-and-aws-docs)
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

<!-- /TOC -->

# Theory and AWS docs

x
x
x
x
x
x

<!-- #########################################

temlpate:

___

## 



**Link to video:**

- 

**AWS docs:** 

- []()

######################################### -->

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


