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






