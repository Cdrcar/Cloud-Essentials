# Amazon - Cloud Essentials Course
Cloud Computing: On demand delivery of IT resources over the internet with pay as you go pricing.
![](Screenshot%202023-09-02%20at%2023.30.33.png)

Module 1
# Learning objectives
In this module, you will learn how to:
* Summarize the benefits of AWS.
* Describe differences between on-demand delivery and cloud deployments.
* Summarize the pay-as-you-go pricing model.
---

Module 2
# Learning objectives
In this module, you will learn how to:
* Describe the benefits of Amazon EC2 at a basic level.
* Identify the different Amazon EC2 instance types.
* Differentiate between the various billing options for Amazon EC2.
* Summarize the benefits of Amazon EC2 Auto Scaling.
* Summarize the benefits of Elastic Load Balancing.
* Give an example of the uses for Elastic Load Balancing.
* Summarize the differences between Amazon Simple Notification Service (Amazon SNS) and Amazon Simple Queue Service (Amazon SQS).
* Summarize additional AWS compute options.

Q&A
1. Which Cloud job role must be proficient with configuration management and changes? - System Administrator
2. Which Cloud job role must be proficient with programming scripting languages? - DevOps Administrator
3. Which Cloud job role is the AWS Cloud Subject Matter Expert (SME) for your business?  - Cloud Architect
4. Which on-premises IT job role maps to the AWS Cloud Architect job role? - IT Solutions Architect
5. Which Cloud job role oversees database and developer teams? - DevOps Administrator

6. Which Amazon EC2 instance type is suitable for data warehousing applications? - Storage optimised:  Require high, sequential read and write access to large datasets on local storage 
7. Which Amazon EC2 instance type balances compute, memory, and networking resources? - General purpose
8. Which Amazon EC2 instance type is ideal for high-performance databases? - Memory optimised: Designed to deliver fast performance for workloads that process large datasets in memory. In computing, memory is a temporary storage area.
9. Which Amazon EC2 instance type offers high-performance processors? - Compute optimised: Ideal for compute-bound applications that benefit from high-performance processors. 

10. Which Amazon EC2 pricing option provides a discount when you specify a number of EC2 instances to run a specific OS, instance family and size, and tenancy in one Region?  - Standard Reserved Instances
11. Which Amazon EC2 pricing option provides a discount when you make an hourly spend commitment to an instance family and Region for a 1-year or 3-year term? - EC2 Instance Savings Plans

12. Which AWS service is the best choice for publishing messages to subscribers? Amazon Simple Notification Service (Amazon SNS)

*EC2:* a service that lets you run virtual servers in the cloud. If you have applications that you want to run in Amazon EC2, you must do the following:
* Provision instances (virtual servers).

* Upload your code.

* Continue to manage the instances while your application is running.

*Serverless Computing* -> AWS Lambda

![](Screenshot%202023-09-01%20at%2018.02.43.png)
*Lambda*:

![](Screenshot%202023-09-01%20at%2018.07.33.png)

*Containerized applications* -> Amazon Elastic Container Service (Amazon ECS)
*Containers* provide you with a standard way to package your application’s code and dependencies into a single object.  To ensure that the application’s environment remains consistent regardless of deployment. When running containerised applications, it’s important to consider *scalability*.

 *Amazon Elastic Container Service (Amazon ECS)*

ECS is a highly scalable, high-performance container management system that enables you to run and scale containerised applications on AWS. 

*Docker*
Amazon ECS supports Docker containers.   [Docker](https://www.docker.com/) 
  [(opens in a new tab)](https://www.docker.com/)  is a software platform that enables you to build, test, and deploy applications quickly. 

*Amazon Elastic Kubernetes Service (Amazon EKS)*
Is a fully managed service that you can use to run Kubernetes on AWS.   [Kubernetes](https://kubernetes.io/) [(opens in a new tab)](https://kubernetes.io/)  is open-source software that enables you to deploy and manage containerised applications at scale. 

*AWS Fargate*
  [AWS Fargate](https://aws.amazon.com/fargate/) [(opens in a new tab)](https://aws.amazon.com/fargate/) is a server-less compute engine for containers. It works with both Amazon ECS and Amazon EKS. 
When using AWS Fargate, you do not need to provision or manage servers. AWS Fargate manages your server infrastructure for you. 

_Resume Module 2_
* Amazon EC2 instance types and pricing options
* Amazon EC2 Auto Scaling
* Elastic Load Balancing
* AWS services for messaging, containers, and serverless computing

  *Q&A*
1. You want to use an Amazon EC2 instance for a batch processing workload. What would be the best Amazon EC2 instance type to use?

The correct response option is *Compute optimized*.(Hight performance processor)
 
The other response options are incorrect because:
* General purpose instances provide a balance of compute, memory, and networking resources. This instance family would not be the best choice for the application in this scenario. Compute optimized instances are more well suited for batch processing workloads than general purpose instances.
* Memory optimised instances are more ideal for workloads that process large datasets in memory, such as high-performance databases.
* Storage optimized instances are designed for workloads that require high, sequential read and write access to large datasets on local storage. The question does not specify the size of data that will be processed. Batch processing involves processing data in groups. A compute optimized instance is ideal for this type of workload, which would benefit from a high-performance processor.

2. What are the contract length options for Amazon EC2 Reserved Instances? (Select TWO.) 1 and 3 years

3. You have a workload that will run for a total of 6 months and can withstand interruptions. What would be the most cost-efficient Amazon EC2 purchasing option? - Spot Instance

4. Which process is an example of Elastic Load Balancing? - Ensuring that no single Amazon EC2 instance has to carry the full workload on its own

5. You want to deploy and manage containerised applications. Which service should you use? - Amazon Elastic Kubernetes Service (Amazon EKS):  Kubernetes is open-source software that enables you to deploy and manage containerised applications at scale.
The other response options are incorrect because:
* AWS Lambda is a service that lets you run code without provisioning or managing servers.
* Amazon Simple Queue Service (Amazon SQS) is a service that enables you to send, store, and receive messages between software components through a queue.
* Amazon Simple Notification Service (Amazon SNS) is a publish/subscribe service. Using Amazon SNS topics, a publisher publishes messages to subscribers.

---
Module 3
# Learning objectives
In this module, you will learn how to:
* Summarize the benefits of the AWS Global Infrastructure.
* Describe the basic concept of Availability Zones.
* Describe the benefits of Amazon CloudFront and edge locations.
* Compare different methods for provisioning AWS services.

1. Which statement best describes an Availability Zone? - A single data center or group of data centers within a Region

CDN -> Amazon CloudFront

 *Edge locations*
An *edge location* is a site that Amazon CloudFront uses to store cached copies of your content closer to your customers for faster delivery.

*How to Provision AWS Resources*

—> _Amazon Console_ : web-based interface for accessing and managing AWS services There can be human error (example, forget a checkbox). Manual tool, not great for automation.
—> _Amazon CLI_ : To save time when making API requests, you can use the AWS CLI. AWS CLI enables you to control multiple AWS services directly from the command line within one tool. AWS CLI is available for users on Windows, macOS, and Linux. Tool that allows you to script or programme the API call. Allows me to make API calls using the Terminal in my machine
—> _Amazon Software Development Kits (SDKs)_: Interact with AWS resources through various programming languages.

Else I can use these tools: AWS Elastic Beanstalk or CloudFormation

*AWS Elastic Beanstalk*
With *AWS Elastic Beanstalk*, you provide code and configuration settings, and Elastic Beanstalk deploys the resources necessary to perform the following tasks:
* Adjust capacity
* Load balancing
* Automatic scaling
* Application health monitoring

*AWS CloudFormation*
With *AWS CloudFormation*, you can treat your infrastructure as code. This means that you can build an environment by writing lines of code instead of using the AWS Management Console to individually provision resources. AWS CloudFormation provisions your resources in a safe, repeatable manner, enabling you to frequently build your infrastructure and applications without having to perform manual actions. It determines the right operations to perform when managing your stack and rolls back changes automatically if it detects errors.

_Resume Module 3_:
* AWS Regions and Availability Zones
* Edge locations and Amazon CloudFront
* The AWS Management Console, AWS CLI, and SDKs
* AWS Elastic Beanstalk
* AWS CloudFormation

  *Q&A*
1. Which statement is TRUE for the AWS global infrastructure? A Region consists of three or more Availability Zones.
2. Which factors should be considered when selecting a Region?
Compliance with data governance and legal requirements
Proximity to your customers
Pricing
3. Which statement best describes Amazon CloudFront? - A global content delivery service
4. Which site does Amazon CloudFront use to cache copies of content for faster delivery to users at any location? -  Edge Location
5. Which action can you perform with AWS Outposts? - Extend AWS infrastructure and services to different locations including your on-premises data center.

---

Module 4
# Learning objectives
In this module, you will learn how to:
* Describe the basic concepts of networking.
* Describe the difference between public and private networking resources. 
* Explain a virtual private gateway using a real life scenario. 
* Explain a virtual private network (VPN) using a real life scenario.
* Describe the benefit of AWS Direct Connect. 
* Describe the benefit of hybrid deployments. 
* Describe the layers of security used in an IT strategy.
* Describe the services customers use to interact with the AWS global network.


-> *Amazon Virtual Private Cloud (Amazon VPC)* Amazon VPC enables you to provision an isolated section of the AWS Cloud. In this isolated section, you can launch resources in a virtual network that you define. A Virtual Private Cloud (VPC) exists within a *single AWS region* and can span *multiple AZs*. Create a VPN connection between the VPC and the internal corporate network.
 
-> *Internet gateway*
To allow public traffic from the internet to access your VPC, you attach an *internet gateway* to the VPC.

-> *Virtual private gateway*
To access private resources in a VPC, you can use a *virtual private gateway*. 

-> *AWS Direct Connect* [AWS Direct Connect](https://aws.amazon.com/directconnect/)  is a service that lets you to establish a dedicated private connection between your data center and a VPC.  


![](Screenshot%202023-09-01%20at%2020.37.02.png)


-> *Subnets*
![](Screenshot%202023-09-01%20at%2020.37.38.png)
-> *Network traffic in a VPC*
When a customer requests data from an application hosted in the AWS Cloud, this request is sent as a packet. A *packet* is a unit of data sent over the internet or a network. 
It enters into a VPC through an internet gateway. Before a packet can enter into a subnet or exit from a subnet, it checks for permissions. These permissions indicate who sent the packet and how the packet is trying to communicate with the resources in a subnet.

-> *Network ACLs* (Access Control List)
A network ACL is a virtual firewall that controls inbound and outbound traffic at the subnet level.Each AWS account includes a default network ACL. When configuring your VPC, you can use your account’s default network ACL or create custom network ACLs. 
By default, your account’s default network ACL allows all inbound and outbound traffic, but you can modify it by adding your own rules. For custom network ACLs, all inbound and outbound traffic is denied until you add rules to specify which traffic to allow.

->  *Stateless packet filtering*
Network ACLs perform *stateless* packet filtering. They remember nothing and check packets that cross the subnet border each way: inbound and outbound. 

![](Screenshot%202023-09-01%20at%2020.42.27.png)

-> *Security groups*
A security group is a virtual firewall that controls inbound and outbound traffic for an Amazon EC2 instance.  By default, a security group denies all inbound traffic and allows all outbound traffic.

-> *Stateful packet filtering*
Security groups perform *stateful* packet filtering. They remember previous decisions made for incoming packets.

![](Screenshot%202023-09-01%20at%2020.44.37.png)

![](Screenshot%202023-09-01%20at%2020.45.07.png)

								*Q&A*
1. Which statement best describes an AWS account’s default network access control list? - By default, an AWS account’s default Network Access Control List (*NACL*) is *stateless* and *allows all inbound and outbound traffic*. You can customize the rules for NACLs to control the traffic flow as per your security requirements.

-> *Domain Name System (DNS)*
![](Screenshot%202023-09-01%20at%2020.55.46.png)

For example, suppose that you want to visit AnyCompany’s website. 

.. When you enter the domain name into your browser, this request is sent to a customer DNS resolver. 

.. The customer DNS resolver asks the company DNS server for the IP address that corresponds to AnyCompany’s website.

.. The company DNS server responds by providing the IP address for AnyCompany’s website, 192.0.2.0.

-> *Amazon Route 53*
  [Amazon Route 53](https://aws.amazon.com/route53) is a DNS web service. It gives developers and businesses a reliable way to route end users to internet applications hosted in AWS. 
Amazon Route 53 connects user requests to infrastructure running in AWS (such as Amazon EC2 instances and load balancers). It can route users to infrastructure outside of AWS.
Another feature of Route 53 is the ability to manage the DNS records for domain names. You can register new domain names directly in Route 53. You can also transfer DNS records for existing domain names managed by other domain registrars. This enables you to manage all of your domain names within a single location.

![](Screenshot%202023-09-01%20at%2020.58.12.png)

![](Screenshot%202023-09-01%20at%2020.58.48.png)

							*Q&A*
1. Which statement best describes DNS resolution? Translating a domain name to an IP address

2. Your company has an application that uses Amazon EC2 instances to run the customer-facing website and Amazon RDS database instances to store customers’ personal information. How should the developer configure the VPC according to best practices? Place the Amazon EC2 instances in a public subnet and the Amazon RDS database instances in a private subnet.
3. Which component can be used to establish a private dedicated connection between your company’s data center and AWS? AWS Direct Connect
4. Which statement best describes security groups? They are stateful and deny all inbound traffic by default. Security groups are stateful. This means that they use previous traffic patterns and flows when evaluating new requests for an instance. By default, security groups deny all inbound traffic, but you can add custom rules to fit your operational and security needs.
5. Which component is used to connect a VPC to the internet? Internet gateway. 
6. Which service is used to manage the DNS records for domain names? Amazon Route 53.

---
Module 5.
-> Learning objectives

* Summarize the basic concept of storage and databases.
* Describe the benefits of Amazon Elastic Block Store (Amazon EBS).
* Describe the benefits of Amazon Simple Storage Service (Amazon S3).
* Describe the benefits of Amazon Elastic File System (Amazon EFS).
* Summarize various storage solutions.
* Describe the benefits of Amazon Relational Database Service (Amazon RDS).
* Describe the benefits of Amazon DynamoDB.
* Summarize various database services.

  Storage
*Instance Stores and Amazon Elastic Block Store (Amazon EBS)*

-> *Instance stores*
Block-level storage volumes behave like physical hard drives.
An   [instance store](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html) provides temporary block-level storage for an Amazon EC2 instance. An instance store is disk storage that is physically attached to the host computer for an EC2 instance, and therefore has the same lifespan as the instance. *When the instance is terminated, you lose any data in the instance store.*

_->  *Amazon Elastic Block Store (Amazon EBS)* (Block Storage)_

 [Amazon Elastic Block Store (Amazon EBS)](https://aws.amazon.com/ebs)  is a service that provides block-level storage volumes that you can use with Amazon EC2 instances. If you stop or terminate an Amazon EC2 instance, all the data on the attached EBS volume remains available. To create an EBS volume, you define the configuration (such as volume size and type) and provision it. After you create an EBS volume, it can attach to an Amazon EC2 instance.
Because EBS volumes are for data that needs to persist, it’s important to back up the data. You can take incremental *backups* of EBS volumes by creating Amazon EBS *snapshots*.
![](Screenshot%202023-09-01%20at%2021.18.57.png)

1. Which of the following are characteristics of the Amazon EBS service?  Best for data that requires retention. Separate drives from the host computer of an EC2 instance.

_*Amazon Simple Storage Service (Amazon S3)* (Object Storage)_

It is a service that provides object-level storage. Amazon S3 stores data as objects in buckets.
You can upload any type of file to Amazon S3, such as images, videos, text files, and so on. For example, you might use Amazon S3 to store backup files, media files for a website, or archived documents. Amazon S3 offers unlimited storage space. The maximum file size for an object in Amazon S3 is 5 TB.
8 categories:
### S3 Standard
* Designed for frequently accessed data
* Stores data in a minimum of three Availability Zones

### S3 Standard-Infrequent Access (S3 Standard-IA)
* Ideal for infrequently accessed data
* Similar to Amazon S3 Standard but has a lower storage price and higher retrieval price

### S3 One Zone-Infrequent Access (S3 One Zone-IA)
* Stores data in a single Availability Zone
* Has a lower storage price than Amazon S3 Standard-IA

### S3 Intelligent-Tiering
* Ideal for data with unknown or changing access patterns
* Requires a small monthly monitoring and automation fee per object

### S3 Glacier Instant Retrieval
* Works well for archived data that requires immediate access
* Can retrieve objects within a few milliseconds

### S3 Glacier Flexible Retrieval
* Low-cost storage designed for data archiving
* Able to retrieve objects within a few minutes to hours

### S3 Glacier Deep Archive
* Lowest-cost object storage class ideal for archiving
* Able to retrieve objects within 12 hours

### S3 Outposts
* Creates S3 buckets on Amazon S3 Outposts
* Makes it easier to retrieve, store, and access data on AWS Outposts

1. You want to store data that is infrequently accessed but must be immediately available when needed. Which Amazon S3 storage class should you use? The S3 Standard-IA storage class is ideal for data that is infrequently accessed but requires high availability when needed. Both S3 Standard and S3 Standard-IA store data in a minimum of three Availability Zones. S3 Standard-IA provides the same level of availability as S3 Standard but at a lower storage price.

If I have to make many changes,  Amazon Elastic Block Store (Amazon EBS) wins over S3. Otherwise S3 wins (99.999999999 durability)

_*Amazon Elastic File System (Amazon EFS)* (File Storage)_

Compared to block storage and object storage, file storage is ideal for use cases in which a large number of services and resources need to access the same data at the same time. In *file storage*, multiple clients (such as users, applications, servers, and so on) can access data that is stored in shared file folders. In this approach, a storage server uses block storage with a local file system to organize files. Clients access data through file paths.


![](Screenshot%202023-09-01%20at%2021.46.52.png)

								Databases
**_*Amazon Relational Database Service (Amazon RDS)*_**

Relational databases use *structured query language (SQL)* to store and query data. This approach allows data to be stored in an easily understandable, consistent, and scalable way. For example, the coffee shop owners can write a SQL query to identify all the customers whose most frequently purchased drink is a medium latte.
![](Screenshot%202023-09-01%20at%2021.52.13.png)
  [Amazon Relational Database Service (Amazon RDS)](https://aws.amazon.com/rds/) is a service that enables you to run relational databases in the AWS Cloud. Amazon RDS is a managed service that automates tasks such as hardware provisioning, database setup, patching, and backups. 

Amazon RDS provides a number of different security options. Many Amazon RDS *database engines* offer encryption at rest (protecting data while it is stored) and encryption in transit (protecting data while it is being sent and received).

-> Amazon RDS database engines
Amazon RDS is available on six database engines, which optimize for memory, performance, or input/output (I/O). Supported database engines include:
* Amazon Aurora
* PostgreSQL
* MySQL
* MariaDB
* Oracle Database
* Microsoft SQL Server

-> Amazon Aurora
  [Amazon Aurora](https://aws.amazon.com/rds/aurora/)  is an enterprise-class relational database. It is compatible with MySQL and PostgreSQL relational databases. It is up to five times faster than standard MySQL databases and up to three times faster than standard PostgreSQL databases. Consider Amazon Aurora if your workloads require high availability. It replicates six copies of your data across three Availability Zones and continuously backs up your data to Amazon S3.

_*Amazon DynamoDB*_ (Non relational Database No SQL, Pupose built, Millisecond response, fully managed, Highly Scalable)
-> Nonrelational databases
In a *nonrelational database*, you create tables. A table is a place where you can store and query data.
Nonrelational databases are sometimes referred to as “NoSQL databases” because they use structures other than rows and columns to organize data. One type of structural approach for nonrelational databases is key-value pairs. With key-value pairs, data is organized into items (keys), and items have attributes (values). You can think of attributes as being different features of your data.


![](Screenshot%202023-09-01%20at%2022.09.56.png)
->   [Amazon DynamoDB](https://aws.amazon.com/dynamodb/) is a key-value database service. It delivers single-digit millisecond performance at any scale. Serverless and Auto Scalable:
![](Screenshot%202023-09-01%20at%2022.10.51.png)

1. What are the scenarios in which you should use Amazon Relational Database Service (Amazon RDS)? (Select TWO.)
Using SQL to organize data
Storing data in an Amazon Aurora database

*Amazon Redshift*
  [Amazon Redshift](https://aws.amazon.com/redshift) is a data warehousing service that you can use for big data analytics. It offers the ability to collect data from many sources and helps you to understand relationships and trends across your data.

*AWS Database Migration Service*
Enables you to migrate relational databases, nonrelational databases, and other types of data stores. For example, suppose that you have a MySQL database that is stored on premises in an Amazon EC2 instance or in Amazon RDS. Consider the MySQL database to be your source database. Using AWS DMS, you could migrate your data to a target database, such as an Amazon Aurora database.

*Additional Database Services*

![](Screenshot%202023-09-01%20at%2022.24.12.png)
![](Screenshot%202023-09-01%20at%2022.24.29.png)


							*Q&A*
1. Which Amazon S3 storage classes are optimized for archival data? (Select TWO.)  - Amazon S3 Glacier Flexible Retrieval, Amazon S3 Glacier Deep Archive
2. Which statement or statements are TRUE about Amazon EBS volumes and Amazon EFS file systems? - EBS volumes store data within a single Availability Zone. Amazon EFS file systems store data across multiple Availability Zones.
3. You want to store data in an object storage service. Which AWS service is best for this type of storage? Amazon Simple Storage Service (Amazon S3)
4. Which statement best describes Amazon DynamoDB? - A serverless key-value database service
5. Which service is used to query and analyze data across a data warehouse? Amazon Redshift:  It is a data warehousing service that you can use for big data analytics. Use Amazon Redshift to collect data from many sources and help you understand relationships and trends across your data.

---
Module 6
# Learning objectives
* Explain the benefits of the shared responsibility model.
* Describe multi-factor authentication (MFA).
* Differentiate between the AWS Identity and Access Management (IAM) security levels.
* Explain the main benefits of AWS Organizations.
* Describe security policies at a basic level.
* Summarize the benefits of compliance with AWS.
* Explain additional AWS security services at a basic level.

*AWS Shared Responsibility Model*

![](Screenshot%202023-09-01%20at%2022.41.08.png)— Customers are responsible for the security of everything that they create and put /in/the AWS Cloud.
— AWS is responsible for security /of/the cloud.

1. Which tasks are the responsibilities of customers? (Select TWO.) Setting permissions for Amazon S3 objects. Patching software on Amazon EC2 instances.

_*User Permissions and Access*_

*AWS Identity and Access Management (IAM)*
Enables you to manage access to AWS services and resources securely.   
IAM gives you the flexibility to configure access based on your company’s specific operational and security needs. You do this by using a combination of IAM features, which are explored in detail in this lesson:
* IAM users, groups, and roles
* IAM policies
* Multi-factor authentication
-> AWS account root user
When you first create an AWS account, you begin with an identity known as the   *root user*.
![](Screenshot%202023-09-01%20at%2022.50.31.png)

-> *IAM users*
An *IAM user* is an identity that you create in AWS. It represents the person or application that interacts with AWS services and resources. It consists of a name and credentials.
By default, when you create a new IAM user in AWS, it has no permissions associated with it. To allow the IAM user to perform specific actions in AWS, such as launching an Amazon EC2 instance or creating an Amazon S3 bucket, you must grant the IAM user the necessary permissions.

-> *IAM policies*
An *IAM policy* is a document that allows or denies permissions to AWS services and resources.  
IAM policies enable you to customize users’ levels of access to resources. For example, you can allow users to access all of the Amazon S3 buckets within your AWS account, or only a specific bucket.

-> *IAM groups*
An IAM group is a collection of IAM users. When you assign an IAM policy to a group, all users in the group are granted permissions specified by the policy. 
Here’s an example of how this might work in the coffee shop. Instead of assigning permissions to cashiers one at a time, the owner can create a “Cashiers” IAM group. The owner can then add IAM users to the group and then attach permissions at the group level. 
![](Screenshot%202023-09-01%20at%2022.59.55.png)

-> *IAM roles*
In the coffee shop, an employee rotates to different workstations throughout the day. Depending on the staffing of the coffee shop, this employee might perform several duties: work at the cash register, update the inventory system, process online orders, and so on. 
An IAM role is an identity that you can assume to gain temporary access to permissions.  

-> *Multi-factor authentication*
In IAM, multi-factor authentication (MFA) provides an extra layer of security for your AWS account.

_*AWS Organizations*_
Suppose that your company has multiple AWS accounts. You can use   [AWS Organizations](https://aws.amazon.com/organizations)  to consolidate and manage multiple AWS accounts within a central location.
When you create an organization, AWS Organizations automatically creates a *root*, which is the parent container for all the accounts in your organization. 
In AWS Organizations, you can centrally control permissions for the accounts in your organization by using   [service control policies (SCPs)](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scps.html)  *SCPs* enable you to place restrictions on the AWS services, resources, and individual API actions that users and roles in each account can access.

-> *Organizational units*
In AWS Organizations, you can group accounts into organizational units (OUs) to make it easier to manage accounts with similar business or security requirements. When you apply a policy to an OU, all the accounts in the OU automatically inherit the permissions specified in the policy.  
![](Screenshot%202023-09-01%20at%2023.11.42.png)

![](Screenshot%202023-09-01%20at%2023.11.54.png)

![](Screenshot%202023-09-01%20at%2023.12.09.png)

1. You are configuring service control policies (SCPs) in AWS Organizations. Which identities and resources can SCPs be applied to? (Select TWO.)
An organizational unit (OU), An individual member account


*Compliance*

*AWS Artifact*
It is a service that provides on-demand access to AWS security and compliance reports and select online agreements. AWS Artifact consists of two main sections: AWS Artifact Agreements and AWS Artifact Reports.

-> AWS Artifact Agreements
Suppose that your company needs to sign an agreement with AWS regarding your use of certain types of information throughout AWS services. You can do this through *AWS Artifact Agreements*. 
 
In AWS Artifact Agreements, you can review, accept, and manage agreements for an individual account and for all your accounts in AWS Organizations. 

-> AWS Artifact Reports
Next, suppose that a member of your company’s development team is building an application and needs more information about their responsibility for complying with certain regulatory standards. You can advise them to access this information in *AWS Artifact Reports*.
 
AWS Artifact Reports provide compliance reports from third-party auditors. These auditors have tested and verified that AWS is compliant with a variety of global, regional, and industry-specific security standards and regulations. 

1. Which tasks can you complete in AWS Artifact? (Select TWO.)
Access AWS compliance reports on-demand. Review, accept, and manage agreements with AWS.

*Denial-of-Service Attacks*
A *denial-of-service (DoS) attack* is a deliberate attempt to make a website or application unavailable to users.
![](Screenshot%202023-09-02%20at%2011.17.53.png)

*Distributed denial-of-service attacks*
In a DDoS attack, multiple sources are used to start an attack that aims to make a website or application unavailable.

![](Screenshot%202023-09-02%20at%2011.18.59.png)

*AWS Shield*

AWS Shield is a service that protects applications against DDoS attacks. AWS Shield provides two levels of protection: Standard and Advanced.

![](Screenshot%202023-09-02%20at%2011.20.43.png)
*Additional Security Services*
You must ensure that your applications’ data is secure while in storage *(encryption at rest)* and while it is transmitted, known as *encryption in transit*.
  [AWS Key Management Service (AWS KMS)](https://aws.amazon.com/kms)   enables you to perform encryption operations through the use of *cryptographic keys*. A cryptographic key is a random string of digits used for locking (encrypting) and unlocking (decrypting) data.

-> *AWS WAF*
  [AWS WAF](https://aws.amazon.com/waf) is a web application firewall that lets you monitor network requests that come into your web applications.   Works together with Amazon CloudFront and an Application Load Balancer.  AWS WAF blocks or allows traffic (similar to network access control lists). However, it does this by using a   [web access control list (ACL)](https://docs.aws.amazon.com/waf/latest/developerguide/web-acl.html)  to protect your AWS resources. 
![](Screenshot%202023-09-02%20at%2011.36.59.png)

-> *Amazon Inspector*
To perform automated security assessments, they decide to use   [Amazon Inspector](https://aws.amazon.com/inspector/) 

-> *Amazon GuardDuty*
  [Amazon GuardDuty](https://aws.amazon.com/guardduty)  is a service that provides intelligent threat detection for your AWS infrastructure and resources. It identifies threats by continuously monitoring the network activity and account behaviour within your AWS environment.

![](Screenshot%202023-09-02%20at%2011.39.39.png)

							*Q&A*
1. Which statement best describes an IAM policy? A document that grants or denies permissions to AWS services and resources
2. An employee requires temporary access to create several Amazon S3 buckets. Which option would be the best choice for this task? IAM role
3. Which statement best describes the principle of least privilege? Granting only the permissions that are needed to perform specific tasks
4. Which service helps protect your applications against distributed denial-of-service (DDoS) attacks? _AWS Shield_
As network traffic comes into your applications, AWS Shield uses a variety of analysis techniques to detect potential DDoS attacks in real time and automatically mitigates them.
The other response options are incorrect because:
* Amazon _GuardDuty_ is a service that provides intelligent threat detection for your AWS infrastructure and resources. It identifies threats by continuously monitoring the network activity and account behavior within your AWS environment.
* _Amazon Inspector_ checks applications for security vulnerabilities and deviations from security best practices, such as open access to Amazon EC2 instances and installations of vulnerable software versions.
* _AWS Artifact_ is a service that provides on-demand access to AWS security and compliance reports and select online agreements.
5. Which task can AWS Key Management Service (AWS KMS) perform? Create cryptographic keys.
---

Module 7
# Learning objectives
In this module, you will learn how to:
* Summarize approaches to monitoring your AWS environment.
* Describe the benefits of Amazon CloudWatch.
* Describe the benefits of AWS CloudTrail.
* Describe the benefits of AWS Trusted Advisor.

*Amazon Clock Watch*

  [Amazon CloudWatch](https://aws.amazon.com/cloudwatch/)  is a web service that enables you to monitor and manage various metrics and configure alarm actions based on data from those metrics. CloudWatch uses   [metrics](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/working_with_metrics.html) to represent the data points for your resources. AWS services send metrics to CloudWatch. CloudWatch then uses these metrics to create graphs automatically that show how performance has changed over time. 

*CloudWatch alarms*
With CloudWatch, you can create   [alarms](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/AlarmThatSendsEmail.html)  that automatically perform actions if the value of your metric has gone above or below a predefined threshold.  The CloudWatch   [dashboard](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Dashboards.html)  feature enables you to access all the metrics for your resources from a single location.

*AWS CloudTrail*
  [AWS CloudTrail](https://aws.amazon.com/cloudtrail/)   records API calls for your account. The recorded information includes the identity of the API caller, the time of the API call, the source IP address of the API caller, and more. You can think of CloudTrail as a “trail” of breadcrumbs (or a log of actions) that someone has left behind them.
![](Screenshot%202023-09-02%20at%2020.30.59.png)

*CloudTrail Insights*
Within CloudTrail, you can also enable   [CloudTrail Insights](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/logging-insights-events-with-cloudtrail.html) 
   [(opens in a new tab)](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/logging-insights-events-with-cloudtrail.html) . This optional feature allows CloudTrail to automatically detect unusual API activities in your AWS account. 

1. Which tasks can you perform using AWS CloudTrail? (Select TWO.) Track user activities and API requests throughout your AWS infrastructure. Filter logs to assist with operational analysis and troubleshooting

*AWS Trusted Advisor*
  [AWS Trusted Advisor](https://aws.amazon.com/premiumsupport/technology/trusted-advisor/) is a web service that inspects your AWS environment and provides real-time recommendations in accordance with AWS best practices. Trusted Advisor compares its findings to AWS best practices in five categories: _cost optimisation, performance, security, fault tolerance, and service limits._ For the checks in each category, Trusted Advisor offers a list of recommended actions and additional resources to learn more about AWS best practices. 
![](Screenshot%202023-09-02%20at%2020.36.43.png)

![](Screenshot%202023-09-02%20at%2020.36.04.png)

							*Q&A*
1. Which actions can you perform using Amazon CloudWatch? (Select TWO.) Monitor your resources’ utilisation and performance. Access metrics from a single dashboard.
2. Which service enables you to review the security of your Amazon S3 buckets by checking for open access permissions? _AWS Trusted Advisor_ is a web service that inspects your AWS environment and provides real-time recommendations in accordance with AWS best practices. The inspection includes security checks, such as Amazon S3 buckets with open access permissions. The other response options are incorrect because:
* Amazon CloudWatch is a web service that enables you to monitor and manage various metrics for the resources that run your applications.
* AWS CloudTrail is a web service that enables you to review details for user activities and API calls that have occurred within your AWS environment.
* Amazon GuardDuty is a service that provides intelligent threat detection for your AWS environment and resources. It identifies threats by continuously monitoring the network activity and account behavior within your AWS environment.
---
Module 8
# Learning objectives
* Describe AWS pricing and support models.
* Describe the AWS Free Tier.
* Describe key benefits of AWS Organizations and consolidated billing.
* Explain the benefits of AWS Budgets.
* Explain the benefits of AWS Cost Explorer.
* Explain the primary benefits of the AWS Pricing Calculator.
* Distinguish between the various AWS Support Plans.
* Describe the benefits of AWS Marketplace.

*AWS Free Tier*
Three types of offers are available: 
![](Screenshot%202023-09-02%20at%2020.49.57.png)

*AWS Pricing Concepts*

![](Screenshot%202023-09-02%20at%2020.55.14.png)

Example EC2 pricing


![](Screenshot%202023-09-02%20at%2021.00.58.png)
![](Screenshot%202023-09-02%20at%2021.01.17.png)

Example S3 pricing
![](Screenshot%202023-09-02%20at%2021.01.58.png)

![](Screenshot%202023-09-02%20at%2021.02.34.png)

*Billing Dashboard*
Use the   [AWS Billing & Cost Management dashboard](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-what-is.html)   to pay your AWS bill, monitor your usage, and analyze and control your costs.

*Consolidated billing*
The consolidated billing feature of _AWS Organizations_ enables you to receive a single bill for all AWS accounts in your organization. By consolidating, you can easily track the combined costs of all the linked accounts in your organization. The default maximum number of accounts allowed for an organization is 4, but you can contact AWS Support to increase your quota, if needed.

![](Screenshot%202023-09-02%20at%2021.06.08.png)
Consolidated billing also enables you to share volume pricing discounts across accounts. 

*AWS Budgets*
You can create budgets to plan your service usage, service costs, and instance reservations. The information in AWS Budgets updates three times a day. This helps you to accurately determine how close your usage is to your budgeted amounts or to the AWS Free Tier limits.
In AWS Budgets, you can also set custom alerts when your usage exceeds (or is forecasted to exceed) the budgeted amount.

*AWS Cost Explorer*
It is a tool that lets you visualize, understand, and manage your AWS costs and usage over time.
AWS Cost Explorer includes a default report of the costs and usage for your top five cost-accruing AWS services. You can apply custom filters and groups to analyze your data. For example, you can view resource usage at the hourly level.

*AWS Support Plans*
AWS offers four different   [Support plans](https://aws.amazon.com/premiumsupport/plans/)  to help you troubleshoot issues, lower costs, and efficiently use AWS services. 
You can choose from the following Support plans to meet your company’s needs: 
* Basic Support: Provides limited access to AWS Trusted Advisor checks.
* Developer Support: Focuses on best practice guidance, client-side diagnostic tools, and building-block architecture support.
* Business Support: Includes all AWS Trusted Advisor checks.
* Enterprise On-Ramp Support: Includes all AWS Trusted Advisor checks, proactive support services, and a Technical Account Manager (TAM).
* Enterprise Support: Includes all AWS Trusted Advisor checks, proactive services, and a designated Technical Account Manager (TAM).

The Developer, Business, Enterprise On-Ramp, and Enterprise Support plans include all the benefits of Basic Support, in addition to the ability to open an unrestricted number of technical support cases. These Support plans have pay-by-the-month pricing and require no long-term contracts.

In general, for pricing, the Developer plan has the lowest cost, the Business and Enterprise On-Ramp plans are in the middle, and the Enterprise plan has the highest cost.

*Technical Account Manager (TAM)*
The Enterprise On-Ramp and Enterprise Support plans include access to a Technical Account Manager (TAM).

The TAM is your primary point of contact at AWS. If your company subscribes to Enterprise Support or Enterprise On-Ramp, your TAM educates, empowers, and evolves your cloud journey across the full range of AWS services. TAMs provide expert engineering guidance, help you design solutions that efficiently integrate AWS services, assist with cost-effective and resilient architectures, and provide direct access to AWS programs and a broad community of experts.

1. Which Support plan includes all AWS Trusted Advisor checks at the lowest cost? Business

*AWS Marketplace*
It is a digital catalog that includes thousands of software listings from independent software vendors. You can use AWS Marketplace to find, test, and buy software that runs on AWS. 

![](Screenshot%202023-09-02%20at%2021.26.16.png)

					*Q&A*

1. Which action can you perform with consolidated billing? Combine usage across accounts to receive volume pricing discounts.
2. Which pricing tool is used to visualize, understand, and manage your AWS costs and usage over time? AWS Cost Explorer. AWS Cost Explorer includes a default report of the costs and usage for your top five cost-accruing AWS services. You can apply custom filters and groups to analyze your data. For example, you can view resource usage at the hourly level.
3. Which pricing tool enables you to receive alerts when your service usage exceeds a threshold that you have defined? AWS Budgets.
4. Your company wants to receive support from an AWS Technical Account Manager (TAM). Which support plan should you choose? Enterprise.
5. Which service or resource is used to find third-party software that runs on AWS? AWS Marketplace
---
Module 9

# Learning objectives
In this module, you will learn how to:
* Understand migration and innovation in the AWS Cloud.
* Summarize the AWS Cloud Adoption Framework (AWS CAF). 
* Summarize the six key factors of a cloud migration strategy.
* Describe the benefits of AWS data migration solutions, such as AWS Snowcone, AWS Snowball, and AWS Snowmobile.
* Summarize the broad scope of innovative solutions that AWS offers.

*AWS Cloud Adoption Framework (AWS CAF)*

-> *Six core perspectives of the Cloud Adoption Framework*
At the highest level, the   AWS Cloud Adoption Framework (AWS CAF) organizes guidance into six areas of focus, called *Perspectives*. 
— In general, the *Business*, *People*, and *Governance* Perspectives focus on _business capabilities_, whereas the               —*Platform*, *Security*, and *Operations* Perspectives focus on _technical capabilities_.

1. Which Perspective of the AWS Cloud Adoption Framework helps you design, implement, and optimise your AWS infrastructure based on your business goals and perspectives? _The Platform Perspective_ of the AWS Cloud Adoption Framework also includes principles for implementing new solutions and migrating on-premises workloads to the cloud.

*Migration Strategies*
# 6 strategies for migration
When migrating applications to the cloud, six of the most common   [migration strategies](https://aws.amazon.com/blogs/enterprise-strategy/6-strategies-for-migrating-applications-to-the-cloud/)   that you can implement are:

* Rehosting:  also known as “lift-and-shift” involves moving applications without changes. 

* Replatforming: also known as “lift, tinker, and shift,” involves making a few cloud optimizations to realize a tangible benefit. Optimization is achieved without changing the core architecture of the application.

* Refactoring/re-architecting:  (also known as *re-architecting*) involves reimagining how an application is architected and developed by using cloud-native features. 

* Repurchasing: involves moving from a traditional license to a software-as-a-service model. 

For example, a business might choose to implement the repurchasing strategy by migrating from a customer relationship management (CRM) system to Salesforce.com.

* Retaining: consists of keeping applications that are critical for the business in the source environment. This might include applications that require major refactoring before they can be migrated, or, work that can be postponed until a later time.

* Retiring:  is the process of removing applications that are no longer needed.

1. Which migration strategy involves moving to a different product? Repurchasing

*AWS Snow Family*

It is a collection of physical devices that help to physically transport up to exabytes of data into and out of AWS. 
![](Screenshot%202023-09-02%20at%2021.53.27.png)
![](Screenshot%202023-09-02%20at%2021.55.35.png)

![](Screenshot%202023-09-02%20at%2021.55.51.png)

![](Screenshot%202023-09-02%20at%2021.56.01.png)

*Innovation with AWS*
Conditions: 
* The current state
* The desired state
* The problems you are trying to solve

-> *Serverless applications*

With AWS, *serverless* refers to applications that don’t require you to provision, maintain, or administer servers. You don’t need to worry about fault tolerance or availability. AWS handles these capabilities for you.

AWS Lambda is an example of a service that you can use to run serverless applications. If you design your architecture to trigger Lambda functions to run your code, you can bypass the need to manage a fleet of servers.

-> *Machine learning*
Traditional *machine learning (ML)* development is complex, expensive, time consuming, and error prone. AWS offers Amazon SageMaker to remove the difficult work from the process and empower you to build, train, and deploy ML models quickly.

-> *Artificial intelligence*
AWS offers a variety of services powered by *artificial intelligence (AI)*. 

For example, you can perform the following tasks:
* Get code recommendations while writing code and identify security issues in your code with Amazon CodeWhisperer.
* Convert speech to text with Amazon Transcribe.
* Discover patterns in text with Amazon Comprehend.
* Identify potentially fraudulent online activities with Amazon Fraud Detector.
* Build voice and text chatbots with Amazon Lex.


*Amazon CodeWhisperer*
It’s an AI software coding companion. It analyzes code and comments as a developer writes code in their integrated development environment. 
						*Q&A*
1. Which service helps you to quickly build, train, and deploy machine learning models? Amazon SageMaker
2. Which Perspective of the AWS Cloud Adoption Framework helps you structure the selection and implementation of permissions? _Security Perspective._ The Security Perspective of the AWS Cloud Adoption Framework also helps you to identify areas on non-compliance and plan ongoing security initiatives.

The other response options are incorrect because:
* The Governance Perspective helps you to identify and implement best practices for IT governance and support business processes with technology.
* The Operations Perspective focuses on operating and recovering IT workloads to meet the requirements of your business stakeholders.
* The Business Perspective helps you to move from a model that separates business and IT strategies into a business model that integrates IT strategy.
3. Which statement best describes Amazon Lex? A service that enables you to build conversational interfaces using voice and text

---
Module 10
# Learning objectives
* Summarize the six pillars of the Well-Architected Framework.  
* Explain the six benefits of cloud computing.

*The AWS Well-Architected Framework*
Helps you understand how to design and operate reliable, secure, efficient, and cost-effective systems in the AWS Cloud. It provides a way for you to consistently measure your architecture against best practices and design principles and identify areas for improvement.
![](Screenshot%202023-09-02%20at%2022.20.28.png)

— *Operational excellence* is the ability to run and monitor systems to deliver business value and to continually improve supporting processes and procedures.   Performing operations as code, annotating documentation, anticipating failure, and frequently making small, reversible changes.
— The *Security* pillar is the ability to protect information, systems, and assets while delivering business value through risk assessments and mitigation strategies. 
Best practices:
* Automate security best practices when possible.
* Apply security at all layers.
* Protect data in transit and at rest
— *Reliability* is the ability of a system to do the following:
* Recover from infrastructure or service disruptions
* Dynamically acquire computing resources to meet demand
* Mitigate disruptions such as misconfigurations or transient network issues
Reliability includes testing recovery procedures, scaling horizontally to increase aggregate system availability, and automatically recovering from failure.
— *Performance efficiency* is the ability to use computing resources efficiently to meet system requirements and to maintain that efficiency as demand changes and technologies evolve. 
Evaluating the performance efficiency of your architecture includes experimenting more often, using serverless architectures, and designing systems to be able to go global in minutes.
— *Cost optimization* is the ability to run systems to deliver business value at the lowest price point.
Cost optimization includes adopting a consumption model, analyzing and attributing expenditure, and using managed services to reduce the cost of ownership.
— *Sustainability* is the ability to continually improve sustainability impacts by reducing energy consumption and increasing efficiency across all components of a workload by maximizing the benefits from the provisioned resources and minimizing the total resources required.

1. Which pillar of the AWS Well-Architected Framework focuses on the ability of a workload to consistently and correctly perform its intended functions? Reliability

*Benefits of the AWS Cloud*
* _Trade upfront expense for variable expense_: Upfront expenses include data centers, physical servers, and other resources that you would need to invest in before using computing resources. 

Instead of investing heavily in data centers and servers before you know how you’re going to use them, you can pay only when you consume computing resources.

* _Benefit from massive economies of scale_: By using cloud computing, you can achieve a lower variable cost than you can get on your own. 
Because usage from hundreds of thousands of customers aggregates in the cloud, providers such as AWS can achieve higher economies of scale. Economies of scale translate into lower pay-as-you-go prices.

* Stop guessing capacity: With cloud computing, you don’t have to predict how much infrastructure capacity you will need before deploying an application. 
For example, you can launch Amazon Elastic Compute Cloud (Amazon EC2) instances when needed and pay only for the compute time you use. Instead of paying for resources that are unused or dealing with limited capacity, you can access only the capacity that you need, and scale in or out in response to demand. 

* Increase speed and agility: The flexibility of cloud computing makes it easier for you to develop and deploy applications.
This flexibility also provides your development teams with more time to experiment and innovate.

* Stop spending money running and maintaining data centers: Cloud computing in data centers often requires you to spend more money and time managing infrastructure and servers. 
A benefit of cloud computing is the ability to focus less on these tasks and more on your applications and customers.

* Go global in minutes: The AWS Cloud global footprint enables you to quickly deploy applications to customers around the world, while providing them with low latency.
					
  *Q&A*
1. Which pillar of the AWS Well-Architected Framework includes the ability to run workloads effectively and gain insights into their operations? Operational Excellence
2. What are the benefits of cloud computing? (Select TWO.) Increase speed and agility. Stop spending money running and maintaining data centers.
---

Module 11

![](Screenshot%202023-09-02%20at%2022.40.12.png)




