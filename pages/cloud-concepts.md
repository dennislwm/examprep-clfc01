# Domain 1: Cloud Concepts
<!-- TOC -->

- [Domain 1: Cloud Concepts](#domain-1-cloud-concepts)
    - [Define the AWS Cloud and its value proposition](#define-the-aws-cloud-and-its-value-proposition)
        - [Define the benefits of the AWS cloud including:](#define-the-benefits-of-the-aws-cloud-including)
            - [Global Reach](#global-reach)
            - [Economy of scale](#economy-of-scale)
        - [Explain how the AWS cloud allows users to focus on business value](#explain-how-the-aws-cloud-allows-users-to-focus-on-business-value)
            - [Shifting technical resources to revenue-generating activities as opposed to managing infrastructure](#shifting-technical-resources-to-revenue-generating-activities-as-opposed-to-managing-infrastructure)
    - [Identify aspects of AWS Cloud economics](#identify-aspects-of-aws-cloud-economics)
        - [Define items that would be part of a Total Cost of Ownership proposal](#define-items-that-would-be-part-of-a-total-cost-of-ownership-proposal)
            - [Understand the role of operational expenses (OpEx)](#understand-the-role-of-operational-expenses-opex)
            - [Understand the role of capital expenses (CapEx)](#understand-the-role-of-capital-expenses-capex)
            - [Understand the labor costs associated with on-premises operations](#understand-the-labor-costs-associated-with-on-premises-operations)
            - [Understand the impact of software licensing costs when moving to the cloud](#understand-the-impact-of-software-licensing-costs-when-moving-to-the-cloud)
        - [Identify which operations will reduce costs by moving to the cloud](#identify-which-operations-will-reduce-costs-by-moving-to-the-cloud)
            - [Right-sized infrastructure](#right-sized-infrastructure)
            - [Benefits of automation](#benefits-of-automation)
            - [Reduce compliance scope (for example, reporting)](#reduce-compliance-scope-for-example-reporting)
            - [Managed services (for example, RDS, ECS, EKS, DynamoDB)](#managed-services-for-example-rds-ecs-eks-dynamodb)
    - [Explain the different cloud architecture design principles](#explain-the-different-cloud-architecture-design-principles)
        - [Explain the design principles](#explain-the-design-principles)
            - [Design for failure](#design-for-failure)
            - [Decouple components versus monolithic architecture](#decouple-components-versus-monolithic-architecture)
            - [Implement elasticity in the cloud versus on-premises](#implement-elasticity-in-the-cloud-versus-on-premises)
            - [Think parallel](#think-parallel)
        - [AWS Cloud Adoption Framework (AWS CAF)](#aws-cloud-adoption-framework-aws-caf)
            - [Business Pespective](#business-pespective)
            - [People Perspective](#people-perspective)
            - [Governance Perspective](#governance-perspective)
            - [Platform Perspective](#platform-perspective)
            - [Security Perspective](#security-perspective)
            - [Operations Perspective](#operations-perspective)
        - [Migration strategies](#migration-strategies)
        - [AWS Well-Architected Framework](#aws-well-architected-framework)

<!-- /TOC -->

## Define the AWS Cloud and its value proposition

### Define the benefits of the AWS cloud including:

**Ease of Use**

**Flexibility**

Choose as many AWS services as needed. You receive a virtual platform from AWS, and you load the software services you need to support your applications.

**Cost-Effectiveness**

Pay only for the amount of services you need. There are no long term contracts or up-front commitments. Discounts are provided for certain services reserved for a minimum period of time.

**Scalability and Elasticity**

**Scalability**

Scale applications in two ways, while taking advantage of autoscaling:
  * _Vertically_: Increase computing capacity by adding RAM or CPUs to a virtual machine.
  * _Horizontally_: Increase computing capacity by adding more virtual machines.

Scalability gives us the ability to add resources on demand to accommodate growth. Elasticity means it's designed to grow and shrink on demand based on need.

**Elasticity**

Configure application to always have the resources they need, increasing or decreasing resources depending to meet the changing demands without worrying about capacity planning.

Elasticity is the ability to not only grow (scalability) when required but also reduce in size when required.

**High Availability and Fault Tolerance**

**Fault Tolerance**

This goes one step further than HA by guaranteeing zero downtime. The ability to withstand a certain amount of failure and still remain functional (and/or be self-healing and return to full capacity).
When an environment is fault tolerant, it is able to withstand the loss of a component within the infrastructure while remaining functional. 

**High Availability**

Designed to be available 99.999% of the time, or as close to it as possible. The concept of something being accessible when you attempt to access it.

High availability is the ability of a system to remain in an operational state for a long period of time. Highly available systems are able to stay operational during maintenance and system failures.

**Security**

**Reliability**

**Agility**

The flexibility of cloud computing makes it easier for you to develop and deploy applications, hence it provides you more time to experiment and innovate.

**Pay-as-you go pricing**

#### Global Reach

The global footprint of the AWS Cloud enables you to deploy applications to customers around the world quickly, while providing them with low latency. This means that even if you are located in a different part of the world than your customers, customers are able to access your applications with minimal delays. 

#### Economy of scale

By using cloud computing, you can achieve a lower variable cost thatn you can get on your own. The economy of scale translates into lower pay-as-you-go prices.

### Explain how the AWS cloud allows users to focus on business value

The idea of IT resources is actually a big part of the AWS philosophy. If there are IT elements that are common across a number of businesses, then this is not a differentiator.

Take a MySQL database as an example. If your business runs a MySQL database, does your ability to install the MySQL engine make you a better company than your competitors? Well, probably not that. Do you keep backups in a way that makes you superior to other players in your vertical? Again, doubtful. 

The data inside your database, now that's critically different. The way you build your tables and manage the structures, absolutely separates you from the competition. But the engine is just the engine. 

At AWS, we call that the undifferentiated heavy lifting of IT. Tasks that are common, often repetitive and ultimately time-consuming; these are the tasks AWS wants to help you with so you can focus on what makes you unique.

#### Shifting technical resources to revenue-generating activities as opposed to managing infrastructure

## Identify aspects of AWS Cloud economics

### Define items that would be part of a Total Cost of Ownership proposal

#### Understand the role of operational expenses (OpEx)

#### Understand the role of capital expenses (CapEx)

#### Understand the labor costs associated with on-premises operations

#### Understand the impact of software licensing costs when moving to the cloud

### Identify which operations will reduce costs by moving to the cloud

#### Right-sized infrastructure

#### Benefits of automation

#### Reduce compliance scope (for example, reporting)

#### Managed services (for example, RDS, ECS, EKS, DynamoDB)

## Explain the different cloud architecture design principles

### Explain the design principles

#### Design for failure

#### Decouple components versus monolithic architecture

#### Implement elasticity in the cloud versus on-premises

#### Think parallel

### AWS Cloud Adoption Framework (AWS CAF)

At the highest level, the AWS CAF organizes guidance into six area of focus, called **Perspectives**. Each Perspective addresses distinct responsibilities to help the right people across the organization prepare for the changes ahead.

In general, the Business, People, and Governance Perspectives focus on business capabilities, whereas the Platform, Security, and Operations Perspectives focus on technical capabilities.

#### Business Pespective

The **Business Perspective** ensures that IT aligns with business needs and that IT investments link to key business results. Use the Business Perspective to create a strong business case for cloud adoption and prioritize cloud adoption initiatives.

Common roles in the Business Perspective include:
* Business managers
* Finance managers
* Budget owners
* Strategy stakeholders

#### People Perspective

The **People Pespective** supports development of an organization-wide change management strategy for successful cloud adoption. Use the People Perspective to evaluate organizational structures and roles, new skill and process requirements, and identify gaps.

Common roles in the People Perspective include:
* Human resources
* Staffing
* People managers

#### Governance Perspective

The **Governance Perspective** focuses on the skills and processes to align IT strategy with business strategy. Use the Governance Perspective to understand how to update the staff skills and processes necessary to ensure business goverance in the cloud.

Common roles in the Governance Perspective include:
* Chief Information Officer (CIO)
* Program managers
* Enterprise architects
* Business analysts
* Portfolio managers

#### Platform Perspective

The **Platform Perspective** includes principles and patterns for implementing new solutions on the cloud, and migrating on-premises workloads to the cloud. Use a variety of architectural models to understand and communicate the structure of IT systems and their relationships.

Common roles in the Platform Perspective include:
* Chief Technology Officer (CTO)
* IT managers
* Solutions architects

#### Security Perspective

The **Security Perspective** ensures that the organization meets security objectives for visibility, auditability, control, and agility. Use the AWS CAF to structure the selection and implementation of security controls that meet the organization's needs.

Common roles in the Security Perspective include:
* Chief Information Security Officer (CISO)
* IT security managers
* IT security analysts

#### Operations Perspective

The **Operations Perspective** helps you to enable, run, use, operate, and recover IT workloads to the level agreed upon with your business stakeholders. The AWS CAF helps these stakeholders define current operating procedures and identify the process changes and training needed to implement successful cloud adoption.

Common roles in the Operations Perspective include:
* IT operations managers
* IT support managers

### Migration strategies

When migrating applications to the cloud, six of the most common migration strategies that you can implement are:
* Rehosting
* Replatforming
* Refactoring/re-architecting
* Repurchasing
* Retaining
* Retiring

**Rehosting** (also known as _lift-and-shift_) involves moving applications without changes quickly to meet a business case.

**Replatforming** (also known as _lift, tinker, and shift_) involves making a few cloud optimizations to realize a tangible benefit. Optimization is achieved without changing the core architecture of the application.

**Refactoring** (also known as _re-architecting_) involves reimagining how an application is architected and developed by using cloud-native features. Refactoring is driven by a strong business need to add features, scale, or performance that would otherwise be difficult to achieve in the application's existing environment.

**Repurchasing** involves moving from a traditional license to a SaaS model, e.g. by migrating from an on-premise CRM system to Salesforce.com.

**Retaining** consists of keeping applications that are critical for the business in the source environment. This might include applications that require major refactoring before they can be migrated, or, work that can be postponed until a later time.

**Retiring** is the process of removing applications that are no longer needed.

### AWS Well-Architected Framework

The **AWS Well-Architected Framework** helps you understand how to design and operate reliable, secure, efficient, and cost-effective systems in the AWS Cloud. It provides a way for you to consistently measure your architecture against best practices and design principles and identify areas for improvement.

The Well-Architected Framework is based on five pillars:
* Operational excellence
* Security
* Reliability
* Performance efficiency
* Cost optimization

**Operational excellence** is the ability to run and monitor systems to deliver business value and to continually improve supporting processes and procedures. Design principles for operational excellence in the cloud include perform operations as code, annotating documentation, anticipating failure, and frequently making small, reversible changes.

**Security** is the ability to protect information, systems, and assets while delivering business value through risk assessments and mitigation strategies. When considering security, you should apply best practices that include automate security best practices when possible, apply security at all layers, and protect data in transit and at rest.

**Reliability** is the ability of a system to do the following:
* Recover from infrastructure or service disruptions
* Dynamically acquire computing resources to meet demand
* Mitigate disruptions such as misconfigurations or transient network issues
Reliability includes testing recovery procedures, scaling horizontally to increase aggregate system availability, and automatically recovering from failure.

**Performance efficiency** is the ability to use computing resources efficiently to meet system requirements and to maintain that efficiency as demand changes and technologies evolve. Evaluating the performance efficiency of your architecture includes experimenting more often, using serverless architectures, and designing systems to be able to go global in minutes.

**Cost optimization** is the ability to run systems to deliver business value at the lowest price point. Cost optimization includes adopting a consumption model, analyzing and attributing expenditure, and using managed services to reduce the cost of ownership.