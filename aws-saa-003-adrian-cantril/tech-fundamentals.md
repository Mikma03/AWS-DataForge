
<!-- TOC -->

- [Cloud Computing Fundamentals](#cloud-computing-fundamentals)
  - [Cloud Computing - what is it...really](#cloud-computing---what-is-itreally)
  - [Public vs Private vs Multi vs Hybrid Cloud](#public-vs-private-vs-multi-vs-hybrid-cloud)
  - [Cloud Service Models](#cloud-service-models)
- [Tech Fundamentals](#tech-fundamentals)
  - [YAML101 - YAML AINT MARKUP LANGUAGE](#yaml101---yaml-aint-markup-language)
  - [JSON101 - JavaScript Object Notation](#json101---javascript-object-notation)
  - [Encryption 101 - PART1 \& PART2](#encryption-101---part1--part2)
  - [Network Starter Pack](#network-starter-pack)
  - [Network Starter Pack - EXTRA - Distributed Denial of Service (DDOS)](#network-starter-pack---extra---distributed-denial-of-service-ddos)
  - [Secure Sockets Layer (SSL) and Transport Layer Security (TLS)](#secure-sockets-layer-ssl-and-transport-layer-security-tls)
  - [Hash Functions \& Hashing](#hash-functions--hashing)
  - [Digital Signatures](#digital-signatures)
  - [DNS 101 Miniseries](#dns-101-miniseries)
  - [Recovery Point Objective (RPO) and Recovery Time Objective (RTO)](#recovery-point-objective-rpo-and-recovery-time-objective-rto)

<!-- /TOC -->

# Cloud Computing Fundamentals

---

## Cloud Computing - what is it...really

Cloud Computing isn't a buzzword - it's a unique type of computing which has a formal set of definitions.

This lesson aims to dispel the jargon, and step through what makes cloud ... cloud.

NIST Special Publication 800-145 : https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-145.pdf

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14040936

---

## Public vs Private vs Multi vs Hybrid Cloud

Understanding what Public Cloud, Private Cloud, Hybrid Cloud and Muti Cloud are is a hugely under rated skill.

More and more larger AWS deployments are requiring a level of bespoke deployment and locational efficiency that only Hybrid cloud can provide, or a level of cloud vendor resilience only achievable with Multi Cloud.

As an AWS solutions architect understanding what IS, and what ISN'T Public, Private, Hybrid and Multi cloud will help in the Exam and in real-world usage.

This lesson steps through the key points of all four types of cloud.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14040943

---

## Cloud Service Models

Cloud Service models define what service you receive from a product.

It defines which parts of the infrastructure stack you are responsible for and which the vendor manages.

They define your unit of consumption - which is the thing you pay for.

As a Service Model Examples : https://en.wikipedia.org/wiki/As_a_service

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/14040947

---

# Tech Fundamentals

---

## YAML101 - YAML AINT MARKUP LANGUAGE

YAML (a recursive acronym for "YAML Ain't Markup Language") is a human-readable data-serialization language. It is commonly used for configuration files and in applications where data is being stored or transmitted.

It's used within AWS as one of two supported CloudFormation Template formats

This lesson is an introduction to YAML

https://en.wikipedia.org/wiki/Recursive_acronym

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/27415250

---

## JSON101 - JavaScript Object Notation

JavaScript Object Notation is an open standard file format, and data interchange format, that uses human-readable text to store and transmit data objects consisting of attribute–value pairs and array data types

It's used within AWS as one of two CloudFormation template formats and for identity and resource policies.

This lesson is a high level introduction to JSON.

**Link to video:**

- https://learn.cantrill.io/courses/730712/lectures/27415253

---

## Encryption 101 - PART1 & PART2

In part 1 of this lesson I step through the difference between encryption at rest, and encryption in transit.

I discuss the high level components of encryption and provide definitions

We look at Symmetric encryption - how it works, and what its limitations are

and we finish by evaluation Asymmetric encryption and how it addresses these problems.

**Link to video:**

- https://learn.cantrill.io/courses/1820301/lectures/42241184

In Part 2 of this lesson I step through the process of signing - and how it can help to prove identity using Asymmetric keys

and we finish up talking about steganography the processing of hiding data inside of something else.

**Link to video:**

https://learn.cantrill.io/courses/1820301/lectures/42241187

---

## Network Starter Pack

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

---

## Network Starter Pack - EXTRA - Distributed Denial of Service (DDOS)

Distributed Denial of Service (DDOS) attacks are effective at disrupting web applications no matter their size.

They are generally initiated from networks of compromised machines known as Botnets.

They come in 3 common types...

Application Layer
Protocol Attacks
Volumetric Attacks
This lesson steps through the architecture of all 3 ... the attack method and the components used.

**Link to video:**

https://learn.cantrill.io/courses/730712/lectures/26952882

---

## Secure Sockets Layer (SSL) and Transport Layer Security (TLS)

Secure Sockets Layer (SSL) and Transport Layer Security (TLS) are what provides the encrypted communications for HTTPS and other encrypted connection oriented protocols. This lesson steps through how the handshake process works for TLS and some of the key components.

**Link to video:**

https://learn.cantrill.io/courses/1820301/lectures/41301663

---

## Hash Functions & Hashing

This video steps through how hashing works , what it's used for and why it's really important as a supporting process for many other areas of tech. It also explains a critical MD5 vulnerability vs something more secure like SHA2-256.

https://marc-stevens.nl/research/papers/MTh%20Marc%20Stevens%20-%20On%20Collisions%20for%20MD5.pdf

https://natmchugh.blogspot.com/2015/02/create-your-own-md5-collisions.html

https://www.sentinelone.com/cybersecurity-101/hashing/

**Link to video:**

https://learn.cantrill.io/courses/730712/lectures/41817977

---

## Digital Signatures

This video explores how public key cryptography, signing and hashing can be used to provide authenticity and integrity checks on data of all kinds. Digital signatures support many of the other tech used day to day within AWS and beyond.

**Link to video:**

https://learn.cantrill.io/courses/730712/lectures/41818183

---

## DNS 101 Miniseries

The Domain Name System (DNS) is a core part of most applications and IT systems. If you work as a developer, engineer, solutions architect, devops engineer, security engineer or in any other IT role - you HAVE to understand DNS. DNS uses a fairly complex hierarchical structure to allow scaling and delegation. In this series of videos I will step you through the functionality of DNS from what it does, why it's needed, how it works and elaborate on many of the core pieces of functionality.

In this video I will start by explaining what DNS does ... in super simple terms.

**Link to video:**

https://learn.cantrill.io/courses/1820301/lectures/43290509
https://learn.cantrill.io/courses/1820301/lectures/43290510
https://learn.cantrill.io/courses/1820301/lectures/43290514
https://learn.cantrill.io/courses/1820301/lectures/43290516
https://learn.cantrill.io/courses/1820301/lectures/43390310

DNSSEC strengthens authentication in DNS using digital signatures based on public key cryptography. With DNSSEC, it's not DNS queries and responses themselves that are cryptographically signed, but rather DNS data itself is signed by the owner of the data.

This video steps through what benefits DNSSEC provides and one of the common attacks which can be conducted against DNS.

**Link to video:**

https://learn.cantrill.io/courses/1820301/lectures/43390310
https://learn.cantrill.io/courses/1820301/lectures/43390325
https://learn.cantrill.io/courses/1820301/lectures/43390327

---

## Recovery Point Objective (RPO) and Recovery Time Objective (RTO)

Recovery Point Objective (RPO) and Recovery Time Objective (RTO) are essential concepts to understand in almost all areas of IT, Cloud and AWS. They inform much of the design choices relating to backups, restore and resilience within systems.

**Link to video:**

https://learn.cantrill.io/courses/1820301/lectures/43601660

---