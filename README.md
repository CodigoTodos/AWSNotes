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






