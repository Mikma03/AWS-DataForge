<!-- TOC -->

- [SAA-course-range: IAM](#saa-course-range-iam)
  - [IAM Identity Policies](#iam-identity-policies)
  - [IAM Users and ARNs](#iam-users-and-arns)
  - [\[DEMO\] Simple Identity Permissions in AWS](#demo-simple-identity-permissions-in-aws)
  - [IAM Groups](#iam-groups)
  - [\[DEMO\] Permissions control using IAM Groups](#demo-permissions-control-using-iam-groups)
  - [IAM Roles - The Tech](#iam-roles---the-tech)
  - [When to use IAM Roles](#when-to-use-iam-roles)
  - [Service-linked Roles \& PassRole](#service-linked-roles--passrole)
  - [AWS Organizations](#aws-organizations)
  - [\[DEMO\] AWS Organizations - PART1 \& 2](#demo-aws-organizations---part1--2)
  - [Service Control Policies (SCPs)](#service-control-policies-scps)
  - [\[DEMO\] Using Service Control Policies](#demo-using-service-control-policies)
  - [CloudWatch Logs](#cloudwatch-logs)
  - [CloudTrail](#cloudtrail)
  - [\[DEMO\] Implementing an Organizational Trail](#demo-implementing-an-organizational-trail)
- [More about AWS Control Tower 101](#more-about-aws-control-tower-101)
- [AWS IAM Identity Center](#aws-iam-identity-center)
- [Okta](#okta)

<!-- /TOC -->

# SAA-course-range: IAM

## IAM Identity Policies

Identity Policies are attached to AWS identities and either ALLOW or DENY access to AWS resources.

In this lesson I step through the main components of an IAM policy .. and discuss in some detail about the priority order or ALLOW and DENY.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14274988

**AWS docs:**

- [Policies and permissions in IAM](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html)

---

## IAM Users and ARNs

IAM Users are one of the identity types available inside AWS.

They are type you pick when you can identity a single individual or 'thing' which will use that identity - a person, an application or a service account.

In this lesson I detail the architecture of an IAM user ... how it authenticates, and talk about ARNs which are how resources in AWS are identified.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14275269

**AWS docs:**

- [Amazon Resource Names (ARNs)](https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html)

---

## [DEMO] Simple Identity Permissions in AWS

In this [DEMO] lesson we create an IAM user, and experiment with assigning permissions on two S3 buckets via inline policies and managed policies.

The DEMO lesson will require two browsers

the 1st will login to the IAMADMIN user of the general account

the 2nd will login to an IAM user called 'sally' for testing.

This lesson guest stars Thor and Merlin - two animal friends... enjoy :)

**Link to video:**

- https://learn.cantrill.io/courses/1820301/lectures/41301364

---

## IAM Groups

IAM Groups are a feature of IAM which you need to know about for the exam.

They are an admin or container feature.

You can add IAM users to groups, and add permissions to Groups

Groups are NOT real identities ... can't be used from resource policies and have no credentials to login with.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14275293

**AWS docs:**

- [IAM user groups](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_groups.html)

---

## [DEMO] Permissions control using IAM Groups

In this [DEMO] we investigate how groups can be used to hold permissions for group members.

Permissions which were assigned to the IAM user 'Sally' are migrated to a new development group we create in the demo.

**Link to video:**

- https://learn.cantrill.io/courses/1820301/lectures/41301366

---

## IAM Roles - The Tech

IAM Roles are one of the more difficult AWS identity types of fully understand.

In this lesson I step through the basic technical and architecture points of AWS IAM Roles.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14293449

**AWS docs:**

- [IAM roles](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html)

---

## When to use IAM Roles

In this lesson I try to step through the type of situations where IAM roles might be used.

By giving examples - I hope to make you more comfortable when to select and when NOT to select roles.

It's an important set of skills to have for the exam and real-world AWS usage.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14293450

**AWS docs:**

- [Using IAM roles](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_use.html)

---

## Service-linked Roles & PassRole

A service-linked role is a unique type of IAM role that is linked directly to an AWS service. Service-linked roles are predefined by the service and include all the permissions that the service requires to call other AWS services on your behalf. The linked service also defines how you create, modify, and delete a service-linked role.

A service might automatically create or delete the role. It might allow you to create, modify, or delete the role as part of a wizard or process in the service. Or it might require that you use IAM to create or delete the role.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/40570800

**AWS docs:**

- [Using service-linked roles](https://docs.aws.amazon.com/IAM/latest/UserGuide/using-service-linked-roles.html)

---

## AWS Organizations

In this lesson I explain AWS Organizations - It's architecture and some of the benefits for businesses managing larger numbers of AWS Accounts.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14293487

**AWS docs:**

- [AWS Organizations](https://aws.amazon.com/organizations/)

---

## [DEMO] AWS Organizations - PART1 & 2

In this [DEMO] Lesson we will create an organisation for the Animals4life business.

The GENERAL account will become the MASTER account for the organisation

We will invite the PRODUCTION account as a MEMBER account and create the DEVELOPMENT account as a MEMBER account.

Finally - we will create an OrganizationAccountAccessRole in the production account, and use this role to switch between accounts.

WARNING : If you get an error "You have exceeded the allowed number of AWS Accounts" then you can go here https://console.aws.amazon.com/servicequotas/home?region=us-east-1#!/services/organizations/quotas/L-29A0C5DF and request a quote increase for the number of member accounts in an ORG

**Link to video:**

https://learn.cantrill.io/courses/1820301/lectures/41301371
https://learn.cantrill.io/courses/1820301/lectures/41301372

---

## Service Control Policies (SCPs)

In this lesson I introduce service control policies - a feature of AWS Organizations which allow restrictions to be placed on MEMBER accounts in the form of boundaries.

SCPs can be applied to the organization, to OU's or to individual accounts.

Member accounts can be effected, the MANAGEMENT account cannot.

SCPs DON'T GIVE permission - they just control what an account CAN and CANNOT grant via identity policies.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14293489

**AWS docs:**

- [Service control policies (SCPs)](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scps.html)

---

## [DEMO] Using Service Control Policies

In this [DEMO] lesson we update the structure within the organization - and apply an SCP to the PRODUCTION account to test their capabilities.

**Link to video:**

https://learn.cantrill.io/courses/1820301/lectures/41301374

---

## CloudWatch Logs

CloudWatch Logs is a service which can accept logging data, store it and monitor it.

It is often the default place where AWS Services can output their logging too.

CloudWatch Logs is a public service and can also be utilised in an on-premises environment and even from other public cloud platforms.

This lesson introduces the main concepts of CloudWatch Logs and its architecture.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14293489

**AWS docs:**

- [What is Amazon CloudWatch Logs?](https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/WhatIsCloudWatchLogs.html)

---

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

---

## [DEMO] Implementing an Organizational Trail

In this [DEMO] lesson we will implement a Organizational CloudTrail for the Animals4life organisation.

This CloudTrail will be configured for all regions and set to log global services events.

We will set the trail to log to an S3 bucket and then enhance it to inject data into CloudWatch Logs.

CloudTrail Pricing : https://aws.amazon.com/cloudtrail/pricing/

CloudWatch Logs Pricing : https://aws.amazon.com/cloudwatch/pricing/

**Link to video:**

https://learn.cantrill.io/courses/1820301/lectures/41301377

---

# More about AWS Control Tower 101

AWS Control Tower offers a straightforward way to set up and govern an AWS multi-account environment, following prescriptive best practices. AWS Control Tower orchestrates the capabilities of several other AWS services, including AWS Organizations, AWS Service Catalog, and AWS IAM Identity Center (successor to AWS Single Sign-On), to build a landing zone in less than an hour. Resources are set up and managed on your behalf.

AWS Control Tower orchestration extends the capabilities of AWS Organizations. To help keep your organizations and accounts from drift, which is divergence from best practices, AWS Control Tower applies preventive and detective controls (guardrails). For example, you can use guardrails to help ensure that security logs and necessary cross-account access permissions are created, and not altered.

**Link to video:**

https://learn.cantrill.io/courses/1820301/lectures/42087171

**YouTube**

- https://www.youtube.com/watch?v=rBtHe6Qt1Wc&ab_channel=LoiLiangYang

---

# AWS IAM Identity Center

- Identity Center YouTube video by AWS

  - https://www.youtube.com/watch?v=4yJp5-jGGNk&ab_channel=AmazonWebServices

- How to Setup Okta as an Identity Provider in AWS IAM Identity Center

  - https://www.youtube.com/watch?v=V6VrC5gO6oU&ab_channel=JKSTechLab

- Brief intro and demo of AWS IAM Identity Center
  - https://www.youtube.com/watch?v=AnbBztAmP1w&ab_channel=CloudwithJerry

# Okta

- OKTA Tutorial | What Is OKTA

  - https://www.youtube.com/watch?v=UDCgfMoaq5c&ab_channel=MindMajix

- Okta Administration

  - https://learning.oreilly.com/library/view/okta-administration-up/9781800566644/

- Master SAML 2.0 with Okta

  - https://www.udemy.com/course/master-saml-with-okta/

- Getting Started with Okta

  - https://www.udemy.com/course/getting-started-with-okta/

- OKTA Training | OKTA Online Course
  - https://www.youtube.com/watch?v=fIhEG9FUQDQ&ab_channel=MindMajix
