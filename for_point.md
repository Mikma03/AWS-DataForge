

# SERVERLESS AND APPLICATION SERVICES

## 1

- Architecture Deep Dive - PART1
  - https://learn.cantrill.io/courses/730712/lectures/15190436

- Architecture Deep Dive - PART2
  - https://learn.cantrill.io/courses/730712/lectures/15190450

Kom, obecna architektura. To nas czym mozna pomyslec ->

W Point72 jest architektura zbudowana pod microservices (Process, Upload, Store and Manage), ale to bardziej pod wyzwalanie kolejncyh krokow w pipeline. Dlaczego decyzja zeby stawiac processing na Sparku a nie na zasobach AWS?

Event Driven Architekture - to jest podejscie w Point72. Mikroserwisy sa gotowe na kolejne kroki, widza wydarzenie i podejmuja akcje.

**Event Router **- constant flow of events. Event driven architekture - no concstant running. W ta strone idziemy pod serverless architekture.

Oraz EC2 pod computig.

Wtedy pod Lambde podlaczamy VPCE (gateway) zeby podlaczyc sie do zewnatrz poza VPC. lub jezeli chcemy sie podlaczyc pod publiczny internet to mozemy skonfigurowac NATGW (nat gateway) plus zlaczyc ja z IGW (public internet IPv6).

- https://learn.cantrill.io/courses/730712/lectures/36049039


Dodatkowo sa zastsosowane Lambdy, dlaczego nie zostalo to ubrane w Step Functions od implementacji AWS?

https://learn.cantrill.io/courses/730712/lectures/15267923

## 2

Pod przyszle projekty real-time streaming - Kinesis + Lambda.


## 3

Pod monitoring Lambdy - X-Ray for distributed tracing

Dodatkowo jest potencjal pod automation using CloudFroamtion - CNF.


## 4

Pod computing Bootstraping EC2

- https://learn.cantrill.io/courses/730712/lectures/14679949


## 5

Elastic File System

- https://learn.cantrill.io/courses/730712/lectures/14990550


## 6

Elastic Load Balancer
- https://learn.cantrill.io/courses/730712/lectures/36048303
- https://learn.cantrill.io/courses/730712/lectures/36048304


## 7 to dobre

Auto Scaling Groups
- https://learn.cantrill.io/courses/730712/lectures/36048316


## 8 

AWS Fargate
- https://tutorialsdojo.com/aws-fargate/
- https://tutorialsdojo.com/aws-parallelcluster/
- https://tutorialsdojo.com/aws-serverless-application-model-sam/

##

Big Data
Amazon EMR
https://aws.amazon.com/emr/?c=a&sec=srv

Amazon Athena
https://aws.amazon.com/athena/?c=a&sec=srv&whats-new-cards.sort-by=item.additionalFields.postDateTime&whats-new-cards.sort-order=desc
