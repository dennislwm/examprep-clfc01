# Domain 3: Technology

<!-- TOC depthfrom:2 depthto:4 -->

- [Domain 3: Technology](#domain-3-technology)
  - [Define methods of deploying and operating in the AWS Cloud](#define-methods-of-deploying-and-operating-in-the-aws-cloud)
    - [Identify at a high level different ways of provisioning and operating in the AWS cloud](#identify-at-a-high-level-different-ways-of-provisioning-and-operating-in-the-aws-cloud)
      - [Programmatic access, APIs, SDKs, AWS Management Console, CLI, Infrastructure as Code](#programmatic-access-apis-sdks-aws-management-console-cli-infrastructure-as-code)
    - [Identify different types of cloud deployment models](#identify-different-types-of-cloud-deployment-models)
      - [All in with cloud/cloud native](#all-in-with-cloudcloud-native)
      - [Hybrid](#hybrid)
      - [On-premises](#on-premises)
      - [Benefits of cloud computing](#benefits-of-cloud-computing)
    - [Identify connectivity options](#identify-connectivity-options)
      - [VPN](#vpn)
      - [AWS Direct Connect](#aws-direct-connect)
      - [Public internet](#public-internet)
  - [Define the AWS global infrastructure](#define-the-aws-global-infrastructure)
    - [Describe the relationships among Regions, Availability Zones, and Edge Locations](#describe-the-relationships-among-regions-availability-zones-and-edge-locations)
    - [Describe how to achieve high availability through the use of multiple Availability Zones](#describe-how-to-achieve-high-availability-through-the-use-of-multiple-availability-zones)
      - [Recall that high availability is achieved by using multiple Availability Zones](#recall-that-high-availability-is-achieved-by-using-multiple-availability-zones)
      - [Recognize that Availability Zones do not share single points of failure](#recognize-that-availability-zones-do-not-share-single-points-of-failure)
    - [Describe when to consider the use of multiple AWS Regions](#describe-when-to-consider-the-use-of-multiple-aws-regions)
      - [Disaster recovery/business continuity](#disaster-recoverybusiness-continuity)
      - [Low latency for end-users](#low-latency-for-end-users)
      - [Data sovereignty](#data-sovereignty)
    - [Describe at a high level the benefits of Edge Locations](#describe-at-a-high-level-the-benefits-of-edge-locations)
      - [Amazon CloudFront](#amazon-cloudfront)
      - [AWS Global Accelerator](#aws-global-accelerator)
  - [Identify the core AWS services](#identify-the-core-aws-services)
    - [Describe the categories of services on AWS (compute, storage, network, database)](#describe-the-categories-of-services-on-aws-compute-storage-network-database)
    - [Identify AWS compute services](#identify-aws-compute-services)
      - [Recognize there are different compute families](#recognize-there-are-different-compute-families)
      - [Recognize the different services that provide compute (for example, AWS Lambda compared to Amazon Elastic Container Service (Amazon ECS), or Amazon EC2, etc.)](#recognize-the-different-services-that-provide-compute-for-example-aws-lambda-compared-to-amazon-elastic-container-service-amazon-ecs-or-amazon-ec2-etc)
      - [Recognize that elasticity is achieved through Auto Scaling](#recognize-that-elasticity-is-achieved-through-auto-scaling)
      - [Identify the purpose of load balancers](#identify-the-purpose-of-load-balancers)
    - [Identify different AWS storage services](#identify-different-aws-storage-services)
      - [Describe Amazon S3](#describe-amazon-s3)
      - [Describe Amazon Elastic Book Store (Amazon EBS)](#describe-amazon-elastic-book-store-amazon-ebs)
      - [Describe Amazon S3 Glacier](#describe-amazon-s3-glacier)
      - [Describe AWS Snowball](#describe-aws-snowball)
      - [Describe Amazon Elastic File System (Amazon EFS)](#describe-amazon-elastic-file-system-amazon-efs)
      - [Describe AWS Storage Gateway](#describe-aws-storage-gateway)
    - [Identify AWS networking services](#identify-aws-networking-services)
      - [Identify VPC](#identify-vpc)
      - [Identify security groups](#identify-security-groups)
      - [Identify the purpose of Amazon Route 53](#identify-the-purpose-of-amazon-route-53)
      - [Identify VPN, AWS Direct Connect](#identify-vpn-aws-direct-connect)
    - [Idenfify different AWS database services](#idenfify-different-aws-database-services)
      - [Install databases on Amazon EC2 compared to AWS managed databases](#install-databases-on-amazon-ec2-compared-to-aws-managed-databases)
      - [Identify Amazon RDS](#identify-amazon-rds)
      - [Identify Amazon DynamoDB](#identify-amazon-dynamodb)
      - [Identify Amazon Redshift](#identify-amazon-redshift)
  - [Idenfify resources for technology support](#idenfify-resources-for-technology-support)
    - [Recognize there is documentation (best practices, whitepapers, AWS Knowledge Center, forums, blogs)](#recognize-there-is-documentation-best-practices-whitepapers-aws-knowledge-center-forums-blogs)
    - [Identify the various levels and scope of AWS support](#identify-the-various-levels-and-scope-of-aws-support)
      - [AWS Abuse](#aws-abuse)
      - [AWS support cases](#aws-support-cases)
      - [Premium support](#premium-support)
      - [Technical Account Managers](#technical-account-managers)
    - [Recognize there is a partner network (marketplace, third-party) including independent Software Vendors and System Integrators](#recognize-there-is-a-partner-network-marketplace-third-party-including-independent-software-vendors-and-system-integrators)
    - [Identify sources of AWS technical assistance and knowledge including professional services, solution architects, training and certification, and the Amazon Partner Network](#identify-sources-of-aws-technical-assistance-and-knowledge-including-professional-services-solution-architects-training-and-certification-and-the-amazon-partner-network)
    - [Identify the benefits of using AWS Trusted Advisor](#identify-the-benefits-of-using-aws-trusted-advisor)

<!-- /TOC -->

## Define methods of deploying and operating in the AWS Cloud

### Identify at a high level different ways of provisioning and operating in the AWS cloud

#### Programmatic access, APIs, SDKs, AWS Management Console, CLI, Infrastructure as Code

### Identify different types of cloud deployment models

The three cloud computing deployment models are cloud-based, on-premises, and hybrid.

#### All in with cloud/cloud native

In a **cloud-based deployment** model, you can migrate existing applications to the cloud, or you can design and build new applications in the cloud. You can build those applications on low-level infrastructure that requires your IT staff to manage them. Alternatively, you can build them using higher-level services that reduce the management, architecting, and scaling requirements of the core infrastructure.

* Run all parts of the application in the cloud.
* Migrate existing applications to the cloud.
* Design and build new applications in the cloud.

#### Hybrid

In a **hybrid deployment**, cloud-based resources are connected to on-premises infrastructure. For example, you have legacy applications that are better maintained on premises, or government regulations require your business to keep certain records on premises.

* Connect cloud-based resources to on-premises infrastructure.
* Integrate cloud-based resources with legacy IT applications.

#### On-premises

**On-premises deployment** is also known as a private cloud deployment. Though this model is much like legacy IT infrastructure, its incorporation of application management and virtualization technologies helps to increase resource utilization.

* Deploy resources by using virtualization and resource management tools.
* Increase resource utilization by using application management and virtualization technologies.

#### Benefits of cloud computing

* Trade upfront expense for variable expense
* Stop spending money to run and maintain data centers
* Stop guessing capacity
* Benefit from massive economies of scale
* Increase speed and agility
* Go global in minutes

### Identify connectivity options

#### VPN

#### AWS Direct Connect

#### Public internet

## Define the AWS global infrastructure

### Describe the relationships among Regions, Availability Zones, and Edge Locations

### Describe how to achieve high availability through the use of multiple Availability Zones

#### Recall that high availability is achieved by using multiple Availability Zones

#### Recognize that Availability Zones do not share single points of failure

### Describe when to consider the use of multiple AWS Regions

#### Disaster recovery/business continuity

#### Low latency for end-users

#### Data sovereignty

### Describe at a high level the benefits of Edge Locations

#### Amazon CloudFront

#### AWS Global Accelerator

## Identify the core AWS services

### Describe the categories of services on AWS (compute, storage, network, database)

### Identify AWS compute services

#### Recognize there are different compute families

#### Recognize the different services that provide compute (for example, AWS Lambda compared to Amazon Elastic Container Service (Amazon ECS), or Amazon EC2, etc.)

#### Recognize that elasticity is achieved through Auto Scaling

#### Identify the purpose of load balancers

### Identify different AWS storage services

#### Describe Amazon S3

#### Describe Amazon Elastic Book Store (Amazon EBS)

#### Describe Amazon S3 Glacier

#### Describe AWS Snowball

#### Describe Amazon Elastic File System (Amazon EFS)

#### Describe AWS Storage Gateway

### Identify AWS networking services

#### Identify VPC

#### Identify security groups

#### Identify the purpose of Amazon Route 53

#### Identify VPN, AWS Direct Connect

### Idenfify different AWS database services

#### Install databases on Amazon EC2 compared to AWS managed databases

#### Identify Amazon RDS

#### Identify Amazon DynamoDB

#### Identify Amazon Redshift

## Idenfify resources for technology support

### Recognize there is documentation (best practices, whitepapers, AWS Knowledge Center, forums, blogs)

### Identify the various levels and scope of AWS support

#### AWS Abuse

#### AWS support cases

#### Premium support

#### Technical Account Managers

### Recognize there is a partner network (marketplace, third-party) including independent Software Vendors and System Integrators

### Identify sources of AWS technical assistance and knowledge including professional services, solution architects, training and certification, and the Amazon Partner Network

### Identify the benefits of using AWS Trusted Advisor
