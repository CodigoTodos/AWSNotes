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

## AWS Application Services

**Step Functions** - Step Functions makes it easy to coordinate the components of distributed applications and micro services using a visual workflow for example you may want a second function to always follow the first and only run if and when the first succeeds and you may want to execute two functions in parallel for example you define your application visually as a series of steps you define the process flow of those steps and then you can deploy your application automatically.

**Simple WorkFlow Service (SWF)** - Amazon simple workflow service works in a similar way to step functions in coordinating multiple components of a business process for new applications it's recommended to use step functions not the swf.

**Simple Notification Servce (SNS)** - Service Amazon simple notification service or SNS for short is a flexible fully managed pub/sub messaging service what that means is that you can create a topic and users subscribe to that topic and when you publish a message to the topic the users that have subscribed to that topic will receive that message it can also be used for push notifications for mobile devices.

**Simple Queue Service (SQS)** – Amazon simple queue service or sqs for short is a fully managed Message Queuing service and that makes it easy to decouple your applications from demand what that means is that it allows messages to build up in a queue until the processing server that processes those messages can catch up with the demand.

![imagem](https://github.com/CodigoTodos/AWSNotes/assets/71842002/8c60d335-7d96-4374-b81d-1060d2b2d586)

## Costumer Engagement

**Amazon Connect** – Amazon Connect is a self-service contact center in the AWS cloud and that is delivered on a pay-as-you-go pricing model it has a drag-and-drop graphical user interface and that allows you to create process flows that define customer interactions without having any coding at all.

**Amazon Pinpoint** - Amazon Pinpoint allows you to send email SMS and mobile push messages for targeted marketing campaigns as well as direct messages to your individual customers for example an order confirmation.

**Simple Email Service (SES)** - Amazon simple email service or SES for short is a cloud-based bulk email sending service.

## Analytics and Machine Learning

**Amazon EMR** - Elastic MapReduce or EMR for short is AWS's Hadoop framework as a service you can also run other frameworks in Amazon EMR that integrate with Hadoop such as Apache spark HBase Presto and Flink. Data can be analyzed by EMR in a number of AWS data stores including Amazon s3 and Amazon DynamoDB.

**Amazon Athena** - Amazon Athena allows you to analyze data stored in an Amazon s3 bucket using standard SQL statement.

**ElasticSearch Service** -  standard SQL statement. Amazon Elastic search is a fully managed service for elastic.co's elasticsearch framework this allows high-speed querying and analysis of data that is stored on AWS.

**Amazon Kinesis** - Amazon Kinesis allows you to collect, process and analyze real-time streaming data.

**Amazon QuickSight** - Amazon quicksight is a business intelligence reporting tool similar to tableau or if you're a Java programmer similar to BIRT and is fully managed by AWS. 

**DeepLens** – AWS deeplens is a deep learning enabled video camera, it has a deep learning software development kit that allows you to create advanced vision system applications.

**SageMaker** - Amazon Sage Maker is AWS's flagship machine learning product it allows you to build and train your own machine learning models and then deploy them to the AWS cloud and use them as a back-end for your applications.

**Amazon Rekognition** - Amazon Rekognition provides deep learning based analysis of video and images.

**Amazon Lex** - allows you to build conversational chatbots, these can be used in many applications such as first-line support for customers.

**Amazon Polly** – Amazon Polly provides natural sounding text-to-speech.

**Amazon Comprehend** - Amazon comprehend can use deeper learning to analyze text for insights and relationships this can be used for customer analysis or for advanced searching of documents.

**Amazon Translate** – Amazon Translate can use machine learning to accurately translate text to a number of different languages.

**Amazon Transcribe** - Amazon Transcribe is an automatic speech recognition service that can analyze audio files that are stored in Amazon s3 and then return that transcribed the text.

## Security Identity and Compliance 

**AWS Artifact** - AWS artifact is an online portal that provides access to AWS security and compliance documentation and that documentation can be readily available when needed for auditing and compliance purposes.

**AWS certificate manager** -  Issues ssl certificates for HTTPS communication with your website it integrates with AWS services such as route 53 and cloudfront and the certificates that are provisioned through AWS certificate manager are completely free.

**Amazon Cloud Directory** - Amazon Cloud directory is a cloud-based directory service that can have hierarchies of data in multiple dimensions unlike conventional LDAP based directory services that can only have a single hierarchy.

**AWS directory service** -  is a fully managed Microsoft Active Directory service in the AWS cloud.

**AWS cloud HSM** - is a dedicated hardware security module in the AWS cloud this allows you to achieve corporate and regulatory compliance while at the same time greatly reducing your costs over using your own HSM in your own infrastructure.

**Amazon Cognito** - provides sign in and sign up capability for your web and mobile applications you can also integrate that signup process with external orth providers such as Google and Facebook and also SAML 2 providers as well. 

**AWS identity and access management (IAM)** - allows you to manage user access to your AWS services and resources in your account, users and groups of users have individual permissions that allow or deny access to your resources. 

**AWS Organizations** -  AWS Organizations provides policy based management for multiple AWS accounts this is great for large organizations that have multiple accounts and they want to manage those and the users that use those accounts centrally.

**Amazon inspector** - is an automated security assessment service it can help to identify vulnerabilities or areas of improvement within your AWS account. 

**AWS key management service (kms)**  - makes it easy to create and control encryption keys for your encrypted data and it also uses hardware security modules to secure your keys it's integrated well with AWS services such as Amazon s3 redshift and EBS.

**AWS shield** - provides protection against distributed denial of service or DDoS for short protection against DDoS attacks the standard version of a double shield is implemented automatically on all AWS accounts.

**Web Application Firewall (WAF)** – is a Web Application Firewall that sits in front of your website to provide additional protection against common attacks such as SQL injection and cross-site scripting it has different sets of rules that can be used for different applications.

## AWS Developer Tools

 AWS Cloud9 - is an integrated development environment running in the AWS cloud it allows you to deploy servers directly to AWS from an integrated development environment.
AWS CodeStar - makes it easy to develop and deploy applications to AWS it can manage the entire CI CD pipeline for you it has a project management dashboard including and integrated issue tracking capability powered by Atlassian JIRA software.
AWS X-Ray makes it easy to analyze and debug applications this provides you with a better insight to the performance of your application and the underlying services that it relies upon.
AWS CodeCommit - is a git repository just like github and it's running in the AWS cloud 
AWS CodePipeline - is a continuous integration and continuous delivery service or CI CD for short it can build test and then deploy your code every time a code change occurs. 
AWS CodeBuild -  Compiles your source code runs tests and then produces software packages that are ready to deploy on AWS.
AWS CodeDeploy -  is a service that automates software deployments to a variety of compute services including Amazon ec2 AWS lambda and even instances that are running on premises

## AWS Media Services

**AWS Elemental MediaConvert** - is a file based video transcoding service for converting video formats for video on the main content 
**AWS MediaPackage** - prepares video content for delivery over the internet it can also protect against piracy through the use of digital rights management.
**AWS Elemental MediaTailor** - Inserts individually targeted advertising into video streams viewers receive streaming video with ads that are personalized for them.
**AWS Elemental MediaLive** - is a broadcast grade live video processing service for creating video streams for delivery to televisions and Internet connected devices.
**Elemental MediaStore** - Is a storage service in the AWS cloud that is optimized for media.
**Amazon Kinesis VideoStreams** - Streams video from connected devices through to the AWS cloud for analytics machine learning and other processing applications.

## AWS Mobile Services

**AWS Mobile Hub** - Allows you to easily configure your AWS services for mobile applications in one place it generates a cloud configuration file which stores information about those configured services.

**AWS Device Farm** - Is an app testing service for Android iOS and web applications it allows you to test your app against a large collection of physical devices in the AWS cloud.

**AWS AppSync** - Is a graph QL back-end for mobile and web applications. 

## AWS Migration Services

**AWS Application Discovery Service** - AWS application discovery service gathers information about an enterprise's on-premises data centers to help plan migration over to AWS data that is collected is retained in an encrypted format in an AWS application discovery service data store.

**AWS Database Migration Service** - Orchestrates the migration of databases over to the AWS cloud you can also migrate databases with one database engine type to another totally different database engine type.

**AWS Server Migration Service** - Can automate the migration of thousands of on-premise workloads over to the AWS cloud this reduces costs and minimizes our downtime for migrations.

**AWS snowball** - is a portable petabyte scale data storage device that can be used to migrate data from on-premises environments over to the AWS cloud you can download your data to the snowball device and then send it to AWS who will then upload that to a storage service for you.

## AWS Business Productivity & App Streaming

**Amazon WorkDocs** - is a secure fully managed file collaboration and management service in the AWS cloud the web client allows you to view and provide feedback for over 35 different file types including Microsoft Office file types and PDF. 

**Amazon WorkMail** - is a secure managed business email and calendar service. 

**Amazon Chime** - is an online meeting service in the AWS cloud it is great for businesses for online meetings video conferencing calls chat and to share content both inside and outside of your organization.

**Amazon WorkSpaces** - is a fully managed secure desktop as a service it can easily provision streaming cloud-based Microsoft Windows desktops.

**Amazon AppStream 2.0** - is a fully managed secure application streaming service that allows you to stream desktop applications from AWS to an html5 compatible web browser, this is great for users who want access to their applications from anywhere.
 
**AWS IOT** - is a managed cloud platform that lets embedded devices such as microcontrollers and Raspberry Pi, to securely interact with cloud applications and other devices.

**Amazon FreeRTOS** - is an operating system for microcontrollers such as the microchip pic32 that allows small low-cost low-power devices to connect to AWS Internet of Things.

**AWS Greengrass** -  is a software that lets you run local AWS lambda functions and messaging data caching sync and machine learning applications on AWS IOT connected devices. AWS Greengrass extends AWS services to devices so they can act locally on the data they generate while still using cloud-based AWS IOT capabilities.

## AWS Game Development

**Amazon Gamelift** - allows you to deploy scale and manage your dedicated game servers in the AWS cloud. 
**Amazon Lumberyard** - it's a game development environment and cross-platform triple-a game engine on the AWS cloud. 

## AWS Elastic Beanstalk

Elastic Beanstalk it's been around for quite some time. It was first launched in 2011 it allows you to quickly deploy and manage applications on environments and those
environments are launched for you without you having to worry about how it all works, it'll automatically handle capacity provisioning, it'll launch a load balancer for you if
you need that, it'll Auto scale for you and it can also implement health monitoring so that if one of these instances that are launched becomes unhealthy it can replace those
automatically for you. If you need to change your code after you have deployed it it's quite easy to upload new versions of that code and that can be done through the console or
the command-line interface and also complete environments can also be redeployed if need be. Your application that you're deploying could be a Docker container it could be raw
code it could be nodejs, java, .net. PHP, Ruby, Python, or GO you just supply your code and Elastic Beanstalk

![imagem](https://github.com/CodigoTodos/AWSNotes/assets/71842002/dbbf4b7b-383d-4bcb-803d-f2ed4f34bb53)

![imagem](https://github.com/CodigoTodos/AWSNotes/assets/71842002/797986e0-c72a-477a-bc7c-5fa8696e37b3)
