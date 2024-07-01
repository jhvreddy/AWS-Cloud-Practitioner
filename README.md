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

**`Compute optimized`** instances are ideal for compute-bound applications that benefit from ``high-performance processors``. Like general purpose instances, you can use compute optimized instances for workloads such as web, application, and gaming servers.
- compute-intensive tasks like gaming servers
- high performance computing or HPC
- scientific modeling
- batch processing workloads that require processing many transactions in a single group.

**`Memory optimized`** instances are good for memory-intensive tasks. 
- Suppose that you have a workload that requires large amounts of data to be preloaded before running an application. This scenario might be a ``high-performance database`` or a workload that involves performing real-time processing of a large amount of unstructured data.

**`Accelerated computing`** use hardware accelerators, or coprocessors, to perform some functions more efficiently than is possible in software running on CPUs. Examples of these functions include floating-point number calculations, graphics processing, and data pattern matching.

**`Storage optimized`** are good for workloads that require high performance for locally stored data. They are designed for workloads that require high, sequential read and write access to large datasets on local storage.  
- distributed file systems
- data warehousing applications and
- high-frequency online transaction processing (OLTP) systems.

Data and Application lives and runs in a Region, one of the first decision you get to make is which region to pick? 

**`Four Business factors`** influence the selection of a region
- Compliance  --> Data must live inside some boundary/not
- Proximity  --> How close you are to your customer base (Latency will be less)
- 
