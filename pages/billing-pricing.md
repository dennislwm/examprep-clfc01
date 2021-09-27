# Domain 4: Billing and Pricing

<!-- TOC -->

- [Domain 4: Billing and Pricing](#domain-4-billing-and-pricing)
    - [Compare and contrast the various pricing models for AWS (for example, On-Demand Instances, Reserved Instances, and Spot Instance pricing)](#compare-and-contrast-the-various-pricing-models-for-aws-for-example-on-demand-instances-reserved-instances-and-spot-instance-pricing)
        - [Identify scenarios/best fit for On-Demand Instance pricing](#identify-scenariosbest-fit-for-on-demand-instance-pricing)
        - [Identify scenarios/best fit for Reserved Instance pricing](#identify-scenariosbest-fit-for-reserved-instance-pricing)
            - [Describe Reserved-Instances flexibility](#describe-reserved-instances-flexibility)
            - [Describe Reserved-Instances behavior in AWS Organizations](#describe-reserved-instances-behavior-in-aws-organizations)
        - [Identify scenarios/best fit for Spot Instance pricing](#identify-scenariosbest-fit-for-spot-instance-pricing)
        - [Dedicated Hosts](#dedicated-hosts)
        - [Amazon EC2 Savings Plan](#amazon-ec2-savings-plan)
        - [Free Tier](#free-tier)
        - [How Are You Charged?](#how-are-you-charged)
            - [Simple Storage Service (S3)](#simple-storage-service-s3)
            - [Elastic Cloud Compute (EC2)](#elastic-cloud-compute-ec2)
    - [Recognize the various account structures in relation to AWS billing and pricing](#recognize-the-various-account-structures-in-relation-to-aws-billing-and-pricing)
        - [AWS Organizations](#aws-organizations)
            - [What are AWS Organizations?](#what-are-aws-organizations)
            - [AWS Organization Benefits](#aws-organization-benefits)
        - [Recognize that consolidated billing is a feature of AWS Organizations](#recognize-that-consolidated-billing-is-a-feature-of-aws-organizations)
        - [Identify how multiple accounts aid in allocating costs across departments](#identify-how-multiple-accounts-aid-in-allocating-costs-across-departments)
    - [Identify resources available for billing support](#identify-resources-available-for-billing-support)
        - [AWS Budgets](#aws-budgets)
        - [AWS Total Cost of Ownership (TCO) Calculator](#aws-total-cost-of-ownership-tco-calculator)
            - [What is the AWS TCO Calculator?](#what-is-the-aws-tco-calculator)
        - [Identify ways to get billing support and information](#identify-ways-to-get-billing-support-and-information)
            - [Cost Explorer, AWS Cost and Usage Report, Amazon QucikSight, third-party partners, and AWS Marketplace tools](#cost-explorer-aws-cost-and-usage-report-amazon-quciksight-third-party-partners-and-aws-marketplace-tools)
            - [Open a billing support case](#open-a-billing-support-case)
            - [The role of the Concierge for AWS Enterprise Support Plan customers](#the-role-of-the-concierge-for-aws-enterprise-support-plan-customers)
        - [Identify where to find pricing information on AWS services](#identify-where-to-find-pricing-information-on-aws-services)
            - [AWS Simple Monthly Calculator](#aws-simple-monthly-calculator)
            - [AWS Services product pages](#aws-services-product-pages)
            - [AWS Pricing API](#aws-pricing-api)
        - [Recognize that alarms/alerts exist](#recognize-that-alarmsalerts-exist)
        - [Identify how tags are used in cost allocation](#identify-how-tags-are-used-in-cost-allocation)

<!-- /TOC -->

## Compare and contrast the various pricing models for AWS (for example, On-Demand Instances, Reserved Instances, and Spot Instance pricing)

### Identify scenarios/best fit for On-Demand Instance pricing

On-demand instances are ideal for short-term, irregular workloads that cannot be interrupted. No upfront costs or minimum contracts apply. 

On-demand purchasing allows you to choose any _instance type_ you like and provision/terminate it at any time (on demand). This is the most expensive and most flexible purchasing option.

You are only charged when the instance is running (and bulled by the hour). There are no long-term contracts or complex licensing requirements.

Volume discounts are available. So the more you use a service, the cheaper it can get (per unit used). There are no termination fees.

### Identify scenarios/best fit for Reserved Instance pricing

Reserved instances are recommended for workloads that last a year or longer.

Reserved purchasing allows you to purchase an instance for a set time period of one (1) or three (3) years. This allows for a significant price discount over using on demand.

#### Describe Reserved-Instances flexibility

You can select to pay upfront, partial upfront, or no upfront. Once you buy a reserved instance, you own it for the selected time period and are responsible for the entire price - regardless of how often you use it.

#### Describe Reserved-Instances behavior in AWS Organizations

At the end of a Reserved instance term, you are charged On-Demand rates until you either terminate the instance or purchase a new Reserved instance that matches the instance attributes (instance type, region, tenancy, and platform).

### Identify scenarios/best fit for Spot Instance pricing

Spot instances are ideal for workloads with flexible start and end times, or that can withstand interruptions. Spot instances are unused Amazon EC2 compute capacity and offer you cost savings at up to 90% off of On-Demand prices.

Spot pricing is a way for you to "bid" on an instance type, and then only pay for and use that instance when the spot price is equal to or below your "bid" price. This allows Amazon to sell the use of unused instances, for short amounts of time, at a substantial discount.

Spot prices fluctuate based on supply and demand in the spot marketplace. You are charged by the minute.

When you have an active bid, an instance is provisioned for you when the spot price is equal to or less than your bid price. A provisioned instance automatically terminates when the spot price is greater than your bid price.

### Dedicated Hosts

Dedicated hosts are physical servers with Amazon EC2 instance capacity that is fully dedicated to your use and it is the most expensive Amazon EC2 option. You can purchase either On-Demand or Reserved Dedicated hosts.

### Amazon EC2 Savings Plan

Amazon EC2 Savings Plan enables you to reduce your EC2 costs by committing to a 1-year or 3-year term. This term commitment results in savings of up to 66% over On-Demand costs. Any usage beyond the commitment is charged at regular On-Demand rates.

### Free Tier

AWS offers a _Free Tier_ option for those new to AWS. Free Tier offers limited AWS resources to you free of charge for 12 months (new accounts only).

### How Are You Charged?

#### Simple Storage Service (S3)

**How much data**
* Applies to data at rest in S3
* Charged per GB stored
* Price per GB varies based on region and storage class

**Request Pricing (moving data in/out of S3)**
* PUT, POST, LIST, GET request (API request)
* Lifecycle transition request
* Data retrieval, data archive, data restore

Note: Free Tier use is available for EC2.

#### Elastic Cloud Compute (EC2)

**Purchasing Options**

Most common (not an inclusive list):
* On demand
* Reserved
* Spot

**Instance Type**

* General purpose
* Compute optimized
* Accelerated computing
* Memory optimized
* Storage optimized

**EBS Optimized**

An option for higher IOPS performance.

**AMI Type**

Think operating system:
* Linux (price varies based on distro/software packages)
* Windows (price varies based on distro/software packages)

**Data Transfer**

In/out of the instance.

**Region**

In which region the instance is provisioned.

## Recognize the various account structures in relation to AWS billing and pricing

### AWS Organizations

#### What are AWS Organizations?

**AWS Organizations** allows you (or your company) to manage billing and access to groups of AWS accounts that you create based on policies that you apply. Organizations enables you to centrally manage policies across multiple AWS accounts, without requiring custom scripts and manual processes.

You can create **Service Control Policies (SCPs)** that centrally control AWS services use across multiple AWS accounts. You can also use Organizations to help automate the creation of new AWS accounts through APIs.

Organizations helps simplify the billing for multiple AWS accounts by enabling you to setup a single payment method for all the accounts through consolidated billing. AWS Organizations is available to all AWS customers at no additional charge.

You can apply SCPs to the organization root, an individual member account, or an organizational unit (OU). An SCP affects all IAM users, groups, and roles within an account, including the AWS account root user.

#### AWS Organization Benefits

* Centrally manage access policies across multiple AWS accounts
* Policy-based management to control access to AWS services
* Automate AWS account creation and management
* Consolidate billing across multiple AWS accounts

### Recognize that consolidated billing is a feature of AWS Organizations

The _consolidated billing_ feature of AWS Organizations enables you to receive a single bill for all AWS accounts in your organization. The default maximum number of accounts allowed for an organization is 4, but you can contact AWS Support to increase your quota, if needed.

On your monthly bill, you can review itemized charges incurred by each account, which enables you to have greater transparency into your organization's accounts while still maintaining the convenience of receiving a single monthly bill.

Another benefit of consolidated billing is the ability to share bulk discount pricing, Savings Plans, and Reserved Instances across the accounts in your organization.

### Identify how multiple accounts aid in allocating costs across departments

## Identify resources available for billing support

AWS helps you reduce Total Cost of Ownership (TCO) by reducing the need to invest in large capital expenditures and providing a PAYG model that empowers you to invest in the capacity that you need and use it only when the business requires it.

### AWS Budgets

In **AWS Budgets**, you can create budgets to plan your service usage, costs, and instance reservations. This helps you to accurately determine how close your usage is to your budgeted amounts or to the AWS Free Tier limits.

You can also set custom alerts when your usage exceeds (or is forecasted to exceed) the budgeted amount.

### AWS Total Cost of Ownership (TCO) Calculator

#### What is the AWS TCO Calculator?

The TCO calculator is a free tool provided by AWS that allows you to estimate the cost savings of using the AWS cloud vs. using an on-premises (or colocation) data center. The TCO calculator can also provide directional guidance on cost savings.

The TCO calculator works by you inputting elements of your current or theoretical on-premises data center and comparing those cost requirements to how much it would cost in AWS. Elements can be added/modified as you move through the process to best estimate the cost savings.

The TCO calculator provides a detailes set of reports that can be used in executive presentations.

### Identify ways to get billing support and information

**AWS Billing & Cost Mangement**

**AWS Billing & Cost Mangement** dashboard is used to pay your AWS bill, monitor your usage, and analyze and control your costs.

* Compare your current MTD balance with the previous month
* Get a forecast of the next month based on current usage
* View MTD spend by service
* View Free Tier usage by service
* Access Cost Explorer and create budgets
* Purchase and manage Savings Plans
* Publish **AWS Cost and Usage Reports**

#### Cost Explorer, AWS Cost and Usage Report, Amazon QucikSight, third-party partners, and AWS Marketplace tools

**Cost Explorer**

Cost Explorer is a free tool that allows you to view charts of your costs for the past 13 months. You can forecast how much you are likely to spend over the next twelve months.

You can use Cost Explorer to discover patterns in how much you spend on AWS resources over time, and identify problem areas. You can identify which services you use the most, as well as metrics like which AZs have the most traffic or which linked AWS account is used the most.

**Cost and Usage Report**

The **AWS Cost and Usage Reports (AWS CUR)** contains the most comprehensive set of cost and usage data available. You can receive reports that break down your costs by the hour, day, or month, by product or product resource, or by tags that you define yourself.

AWS Cost Explorer includes a default report of the costs and usage for your top five cost-accruing AWS services. You can apply custom filters and groups to analyze your data.

**AWS Account Support Plans**

THere are four tiers in the AWS Account Support plans:
1. Basic Support - included with any AWS account, but has no access to a cloud support rep
2. Developer Support - starts at $29 per month, gets business hours access to a **Cloud Support Associate**
3. Business Support - starts at $100 per month, gets 24/7 access to all **Cloud Support Engineer**
4. Enterprise Support - starts at $15,000 per month, gets 24/7 access to all **Sr. Cloud Support Engineer**

**Basic Support**

The Basic Support is included for all AWS customers and includes:
* **Customer Service & Communities** - 24x7 access to customer service, documentation, whitepapers, and support forums.
* **AWS Trusted Advisor** - Access to the seven core Trusted Advisor checks and guidance to provision your resources following best practices to increase performance and improve security.
* **AWS Personal Health Dashboard** - A personalized view of the health of AWS services, and alerts when your resources are impacted.

**Developer Support**

The Developer Support gets the same benefit as Basic Support in terms of Customer Service & Communities, AWS Trusted Advisor and AWS Personal Health Dashboard. In addition, it also gets:
* **Enhanced Technical Support** - business hours email access to a Cloud Support Associate
* **Case Severity / Response Time** 
    * General guidance < 24 business hours
    * System impaired < 12 business hours
* **Architectural Guidance** - General

**Business Support**

The Business Support gets the same benefit as Basic Support in terms of Customer Service & Communities and AWS Personal Health Dashboard. In addition, it also gets:
* **AWS Trusted Advisor** - Access to the _full_ set of Trusted Advisor checks and guidance to provision
* **Enhanced Technical Support** - 24x7 phone, email, and chat access to all Cloud Support Engineers
* **Case Severity / Response Time**
    * General guidance < 24 hours
    * System impaired < 12 hours
    * Production system impaired < 4 hours
    * Production system down < 1 hour
* **Architectural Guidance** - Contextual to your use-cases

**Enterprise Support**

The Business Support gets the same benefit as Business Support in terms of Customer Service & Communities, AWS Trusted Advisor and AWS Personal Health Dashboard. In addition, it also gets:
* **Enhanced Technical Support** - 24x7 phone, email, and chat access to all Sr. Cloud Support Engineers
* **Case Severity / Response Time**
    * General guidance < 24 hours
    * System impaired < 12 hours
    * Production system impaired < 4 hours
    * Production system down < 1 hour
    * Business-critical system down < 15 minutes
* **Architectural Guidance** - Consultative review and guidance based on your applications

**AWS Trusted Advisor**

**AWS Trusted Advisor** is an online tool that provides you real time guidance to help you provision your resources following AWS best practices. It helps you reduce cost, increase performance, and improve security by optimizing your AWS environment.

Trusted Advisor four categories:
* cost optimization
* performance
* security
* fault tolerance

Seven checks that cover basic security and performance that are available to all AWS Support plans:
1. Security groups (port checks)
2. IAM use
3. Is MFA enabled on the root IAM user account?
4. EBS public snapshots
5. RDS public snapshots
6. Service limites
7. S3 bucket permissions

Additional checks and guidance available to only the Business Support and Enterprise Support plans:
* access to the full set of Trusted Advisor checks
* notifications to stay up to date with weekly resource deployments
* programmatic access to retrieve/refresh Trusted Advisor results via API

#### Open a billing support case

#### The role of the Concierge for AWS Enterprise Support Plan customers

### Identify where to find pricing information on AWS services

#### AWS Simple Monthly Calculator

**AWS Simple Monthly Calculator** is used to estimate the anticipated AWS bill based on scenarios. Simple Monthly Calculator estimates your monthly bill and can provide a per-service breakdown of cost.

AWS Simple Monthly Calculator is being replaced by **AWS Pricing Calculator**, which estimates cost for AWS services based on use case. The new calculator can be found [here](https://calculator.aws/#/).

The Pricing Calculator may be used to estimate cost using various workloads including on-demand and reserved instances. Pricing Calculator also helps you identify the cost-effective use case for your instance. Service costs may also be compared on a per-region basis.

#### AWS Services product pages

#### AWS Pricing API

### Recognize that alarms/alerts exist

### Identify how tags are used in cost allocation
