# AWS Notes

Based in this free udemy Course: https://www.udemy.com/course/amazon-web-services-aws-v/ 

## Storage Services

**Simple Storage Service (S3)** - It's designed to store and access any type of data over the Internet. It's a serverless service and as such we don't need to worry about what is behind it. There's obviously a file server an operating system a hard drive but we don't need to be concerned about that at all. We just simply need to create this thing called a bucket and then we upload objects to that bucket, the bucket grows as we add objects to it and the size of that bucket is theoretically unlimited. AWS just looks after everything for us.

**Glacier** - Amazon Glacier is the cheapest storage option on AWS and it's used for long-term archiving of data. It's a serverless service just like Amazon s3 but it is not as readily accessible as s3 so it should only be used for content that is to be archived. You can also set up a lifecycle rule that will automatically migrate old data in Amazon s3 automatically over to Glacier for long-term archiving. 

**Elastic Block Store (EBS)** -  Amazon elastic block store or EBS for short is a highly available, low latency block storage and it's specifically for attaching to servers that are launched with the Amazon ec2 service. It's like attaching a hard drive to your computer at home, works in the same manner. It's block device storage.

**Elastic File System (EFS)** - Amazon Elastic file system or EFS for short is network attached storage and it's specifically for Amazon EC2 servers. Because it is network attached store, this allows multiple servers to access one data source in a similar way to NAS on your network at home can be accessed by multiple computers on that network.

**Storage Gateway** - The AWS Storage Gateway enables hybrid storage between on-premise environments and the AWS cloud. It provides a low latency performance by caching frequently used data on-premises while storing the less frequently data in Amazon Cloud storage services.

**Snowball** - A Snowball device is a portable, petabyte scale, data storage device that can be used to migrate data and large amount of data from on-premise environments over to the AWS cloud. You simply download your data to the Snowball device, then you send it off to AWS who will then upload that data to an AWS storage service for you.

![imagem](https://github.com/CodigoTodos/AWSNotes/assets/71842002/86f19dab-bf57-4064-b961-cd32a3730d37)

![imagem](https://github.com/CodigoTodos/AWSNotes/assets/71842002/bf4fdb0d-8060-41a9-ad6b-7835b043ce90)

## Databases Services

**Relational Database Service (RDS)** - The relational database service or RDS for short is a fully managed database service that makes it easy to launch database servers in the AWS cloud and scale them when required the RDS service can launch service for mySQL including variations of the mySQL database engine with MariaDB and Amazon's own enterprise version of mySQL Amazon Aurora, standard postgre SQL is also available and also available as Amazon's Enterprise Aurora postgre SQL, Microsoft SQL server and oracle are also available. 

**DynamoDB** - Amazon DynamoDB is AWS as no SQL database as a service it's a service  like Amazon s3 and as such you don't need to worry about the underlying infrastructure behind it AWS takes care of everything for you and it provides high speed extremely low latency performance.

**RedShift** - Amazon redshift is a fast fully managed petabyte scale data warehouse that is based upon the postgre SQL database engine if you're looking for a big data storage solution redshift is perfect for this. 

**ElastiCache** - ElastiCache is an in-memory data store or cache in the cloud it allows you to retrieve information from fast fully managed in-memory caches instead of relying for slower disk based databases 

**Database Migration Services (DMS)** - The AWS database migration service or orchestrates a migration of databases over to AWS easily and securely it can also migrate data from one database engine type to another totally different database engine type for example you can use it to migrate from Oracle over to Amazon Aurora.

**Amazon Neptune** - Amazon Neptune is a fast reliable fully managed graph database service it has a purpose-built high performance graph database engine optimized for storing billions of relationships and clearing the graph with millisecond latency.

![imagem](https://github.com/CodigoTodos/AWSNotes/assets/71842002/504b1f83-76fe-4415-8bd3-e25dac37dcce)

## Compute Services

**Elastic Compute Cloud (EC2)** - Amazon Elastic Compute cloud or ec2 for short provides virtual servers in the AWS cloud you can launch one or thousands of instances simultaneously and only pay for what you use there's a broad range of instance types with varying compute and memory capabilities and those will be optimized for different use cases.

**EC2 Autoscaling** - Amazon ec2 auto scaling allows you to dynamically scale your Amazon ec2 capacity up or down automatically according to conditions that you define it can scale up or down by launching or terminating instances based on demand it can also perform health checks on those instances and replace them when they become unhealthy. 

**Amazon Lightsail** - Amazon Lightsail, it's the easiest way to launch virtual servers running applications in the AWS cloud. AWS will provision everything you need including DNS management and storage to get you up and running as quickly as possible. 

**Elastic Container Service (ECS)** - Amazon Elastic container service or ECS for short is a highly scalable high-performance container management service for docker containers the containers they will run on a managed cluster of ec2 instances. 

**AWS Lambda** - AWS lambda is a serverless service and lets you run code in the AWS cloud without having to worry about provisioning or managing that service you just upload your code and AWS takes care of everything for you.

![imagem](https://github.com/CodigoTodos/AWSNotes/assets/71842002/f7ac0c56-2c07-4173-b8c1-552237eadace)

## Networking & Content Delivery

**CloudFront** - Amazon CloudFront is a global content delivery network or CDN for short that securely delivers your frequently requested content to over 100 edge locations across the globe and by doing this it achieves low latency and high transfer speeds for your end-users it also provides protection against DDoS attacks.

**Virtual Private Cloud (VPC)** - Amazon virtual private cloud or VPC for short lets you provision a logically isolated section of the AWS cloud and you can launch AWS resources in that virtual network that you yourself define and this is your own personal private space within the AWS cloud and no one can enter it unless you allow them to enter it.

**Direct Connect** - AWS Direct Connect is a high speed dedicated network connection to AWS enterprise's can use it to establish a private connection to the AWS cloud in situations where a standard internet connection won't be adequate AWS.

**Elastic Load Balancing (ELB)**  - Elastic load balancing or ELB for short or automatically distributes incoming traffic for your application across multiple ec2 instances and also in multiple availability zones so if one availability zone goes down the traffic will still go to the other availability zone and your application will continue to deliver responses to requests it also allows you to achieve high availability and fault tolerance by distributing traffic evenly amongst those instances and it can also bypass unhealthy instances.

**Route 53** - Amazon route 53 is a highly available and scalable domain name system or DNS for short and it can handle direct traffic for your domain name and direct that traffic to your back-end web serve.

**API Gateway** - Amazon API gateway is a fully managed service that makes it easy for developers to create and deploy secure application programming interfaces or api's at any scale it handles all of the tasks involved in accepting and processing up to hundreds of thousands of concurrent API calls it's a service service and as such you don't need to worry about the underlying infrastructure AWS looks after everything for you. 

![imagem](https://github.com/CodigoTodos/AWSNotes/assets/71842002/09919f9b-1075-4b0c-a337-54b5874e50da)

![imagem](https://github.com/CodigoTodos/AWSNotes/assets/71842002/d5b35bed-90a3-4e10-9690-9a2225149644)

![imagem](https://github.com/CodigoTodos/AWSNotes/assets/71842002/fd46539f-d1cf-4174-88dd-b9c6dca39186)

## AWS Management Tools

**Cloud Formation** - CloudFormation allows you to use a text file to define your infrastructure and, to use his text file to deploy resources on the AWS cloud. This allows for the defining of your infrastructure as code and you can manage your infrastructure with the same version control tools that you use to manage your code.

**AWS Service Catalog** - Service Catalog allows enterprises to catalogue resources that can be deployed on the AWS cloud. This allows an enterprise to achieve common governance and compliance for its IT resources by clearly defining what is allowed to be deployed on the AWS cloud.

**AWS CloudWatch** - AWS CloudWatch is a monitoring service for AWS cloud resources and applications that are deployed on the AWS cloud. It can be used for triggering scaling operations or it can also be used for providing insight into your deployed resources. 

**AWS Systems Manager** - AWS Systems Manager provides a unified user interface that allows you to view operational data from multiple AWS services and to automate tasks across your AWS resources. That helps to shorten the time to detect and resolve operational problems.

**CloudTrail** - AWS CloudTrail monitors and logs AWS account activity including actions taken through the AWS management console, the AWS software development kits, the command-line tools and other AWS services. So this greatly simplifies security analysis of the activity of users of your account.

**AWS Config** - AWS Config enables you to assess, audit and evaluate the configurations of your AWS resources. This simplifies compliance auditing, security analysis, change management and control and also, operational troubleshooting.

**AWS Opsworks** - AWS Opsworks provides managed instances of Chef and Puppet. Chef and Puppet can be used to configure and automate the deployment of AWS resources.

**AWS trusted advisor** - AWS trusted advisor is an online expert system that can analyze your AWS account and the resources inside it and then advise you on how to achieve high security and best performance from those resources.









