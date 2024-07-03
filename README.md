# AWS-Cloud-Practitioner
## Introduction
Almost all modern computing centers around a basic client-server model. Basically a customer makes a request, and with permissions, the server responds to that request.
![Client server](https://github.com/jhvreddy/AWS-Cloud-Practitioner/assets/100144454/2024f4cd-2216-428a-a3a2-7dd92c02b366)

### Cloud Computing
Cloud computing is the on-demand delivery of IT resources (compute power, database, storage, applications) over the internet with pay-as-you-go pricing. On-demand delivery indicates that AWS has the resources you need, when you need them. You don't need to tell us in advance that you're going to need them. Suddenly you find yourself needing 300 virtual servers. Well, just a few clicks and launch them. Or you need 2000 terabytes of storage. You don't have to tell us in advance, just start using the storage you need, when you need it. Don't need them anymore, just as quickly, you can return them and stop paying immediately. That kind of flexibility is just not possible when you're managing your own data centers.

**` Benefits of cloud computing `**
- ``Trade upfront expense for variable expense``

Upfront expense refers to data centers, physical servers, and other resources that you would need to invest in before using them. Variable expense means you only pay for computing resources you consume instead of investing heavily in data centers and servers before you know how you’re going to use them.
- ``Stop spending money to run and maintain data centers``

Computing in data centers often requires you to spend more money and time managing infrastructure and servers. A benefit of cloud computing is the ability to focus less on these tasks and more on your applications and customers.
- ``Stop guessing capacity``

With cloud computing, you don’t have to predict how much infrastructure capacity you will need before deploying an application.Instead of paying for unused resources or having to deal with limited capacity, you can access only the capacity that you need. You can also scale in or scale out in response to demand.
- ``Benefit from massive economies of scale``

By using cloud computing, you can achieve a lower variable cost than you can get on your own. AWS aggregates usage from hundreds of thousands of customers in the cloud, which leads to higher economies of scale. This translates into lower pay-as-you-go prices. 
- ``Increase speed and agility``

IT resources are only a click away, which means that you reduce the time to make resources available to your developers from weeks to minutes. This dramatically increases agility for the organization, because the cost and time it takes to experiment and develop is significantly lower.The flexibility of cloud computing makes it easier for you to develop and deploy applications.This flexibility provides you with more time to experiment and innovate. 
- ``Go global in minutes``

The global footprint of the AWS Cloud enables you to deploy applications to customers around the world quickly, while providing them with low latency. This means that even if you are located in a different part of the world than your customers, customers are able to access your applications with minimal delays. This means that you can provide lower latency and a better experience for your customers at a minimal cost.

### Compute in the cloud
AWS has different types of EC2 instances that you can spin up and deploy into your AWS environment. Each instance type is grouped under an instance family and are optimized for certain types of tasks. Instance types offer varying combinations of CPU, memory, storage, and networking capacity, and give you the flexibility to choose the appropriate mix of resources for your applications. The different instance families in EC2 are general purpose, compute optimized, memory optimized, accelerated computing, and storage optimized. 

**`General purpose`** instances provide a good balance of compute, memory, and networking resources, and can be used for a variety of diverse workloads 
- application servers
- gaming servers
- backend servers for enterprise applications
- small and medium databases

**`Compute optimized`** instances are ideal for compute-bound applications that benefit from **high-performance processors**. Like general purpose instances, you can use compute optimized instances for workloads such as web, application, and gaming servers.
- compute-intensive tasks like gaming servers
- high performance computing or HPC
- scientific modeling
- batch processing workloads that require processing many transactions in a single group.

**`Memory optimized`** instances are designed to deliver fast performance for workloads that process large datasets in memory.  
- Suppose that you have a workload that requires large amounts of data to be preloaded before running an application. This scenario might be a **high-performance database** or a workload that involves performing real-time processing of a large amount of unstructured data.

**`Accelerated computing`** use hardware accelerators, or coprocessors, to perform some functions more efficiently than is possible in software running on CPUs. Examples of these functions include floating-point number calculations, graphics processing, and data pattern matching.

**`Storage optimized`** are good for workloads that require high performance for locally stored data. They are designed for workloads that require high, sequential read and write access to large datasets on local storage.  
- distributed file systems
- data warehousing applications and
- high-frequency online transaction processing (OLTP) systems.

### Amazon Ec2-pricing
**`On-Demand`** On-Demand Instances are ideal for short-term, irregular workloads that cannot be interrupted. No upfront costs or minimum contracts apply. The instances run continuously until you stop them, and you pay for only the compute time you use.

Sample use cases for On-Demand Instances include developing and testing applications and running applications that have unpredictable usage patterns. On-Demand Instances are not recommended for workloads that last a year or longer because these workloads can experience greater cost savings using Reserved Instances.

**`Reserved Instances`** These are suited for steady-state workloads or ones with predictable usage and offer you up to a 75% discount versus On-Demand pricing. You qualify for a discount once you commit to a one or three-year term and can pay for them with three payment options: all upfront, where you pay for them in full when you commit; partial upfront, where you pay for a portion when you commit; and no upfront, where you don't pay anything at the beginning.

Reserved Instances are a billing discount applied to the use of On-Demand Instances in your account. There are two available types of Reserved Instances:
- Standard Reserved Instances
- Convertible Reserved Instances
You can purchase Standard Reserved and Convertible Reserved Instances for a 1-year or 3-year term. You realize greater cost savings with the 3-year option.

``Standard Reserved Instances`` This option is a good fit if you know the EC2 instance type and size you need for your steady-state applications and in which AWS Region you plan to run them. Reserved Instances require you to state the following qualifications:
- Instance type and size: For example, m5.xlarge
- Platform description (operating system): For example, Microsoft Windows Server or Red Hat Enterprise Linux
- Tenancy: Default tenancy or dedicated tenancy
You have the option to specify an Availability Zone for your EC2 Reserved Instances. If you make this specification, you get EC2 capacity reservation. This ensures that your desired amount of EC2 instances will be available when you need them. 

``Convertible Reserved Instances`` If you need to run your EC2 instances in different Availability Zones or different instance types, then Convertible Reserved Instances might be right for you. 

**Note** You trade in a deeper discount when you require flexibility to run your EC2 instances.

**`Savings Plan`** Savings Plan offers low prices on EC2 usage in exchange for a commitment to a consistent amount of usage measured in dollars per hour for a one or three-year term. This flexible pricing model can therefore provide savings of up to 72% on your AWS compute usage. This can lower prices on your EC2 usage, regardless of instance family, size, OS, tenancy, or AWS region. This also applies to AWS Fargate and AWS Lambda usage, which are serverless compute options

- The EC2 Instance Savings Plans are a good option if you need flexibility in your Amazon EC2 usage over the duration of the commitment term. You have the benefit of saving costs on running any EC2 instance within an EC2 instance family in a chosen Region (for example, M5 usage in N. Virginia) regardless of Availability Zone, instance size, OS, or tenancy. **The savings with EC2 Instance Savings Plans are similar to the savings provided by Standard Reserved Instances.**
- Unlike Reserved Instances, however, you don't need to specify up front what EC2 instance type and size (for example, m5.xlarge), OS, and tenancy to get a discount. Further, you don't need to commit to a certain number of EC2 instances over a 1-year or 3-year term. Additionally, the EC2 Instance Savings Plans don't include an EC2 capacity reservation option.



Data and Application lives and runs in a Region, one of the first decision you get to make is which region to pick?



**`Four Business factors`** influence the selection of a region
- Compliance  --> Data must live inside some boundary/not
- Proximity  --> How close you are to your customer base (Latency will be less)
- 
