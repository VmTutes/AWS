
What are the three basic types of cloud computing? View Answer Currently, the three basic types of cloud computing include the following:

Infrastructure as a Service (IaaS) Platform as a Service (PaaS) Software as a Service (SaaS) 2.

What is the similarity between the Availability Zones and Regions? Hide Answer The similarity between Availability Zones and Regions is that they both provide geographical redundancy and isolation for cloud infrastructure in the AWS cloud. Availability Zones are distinct locations within a given Region, while Regions are geographic areas with multiple Availability Zones. 3.

Define auto-scaling. Hide Answer Auto-scaling is a cloud computing feature that allows a system to automatically scale its resources up or down based on demand or predetermined conditions. This is typically used to ensure that there are enough resources to handle the load on a system, while also avoiding over-provisioning and keeping costs low. 4.

List the steps involved in a CloudFormation Solution. Hide Answer AWS CloudFormation Solution helps you easily manage AWS resources. The steps are mentioned below:

Create and use an existing CloudFormation template with the help of YAML or JSON format The code then needs to be stored in an S3 bucket. Call the bucket using AWS CloudFormation and on your template you need to create a stack CloudFormation reads the files, their order, and the relationship between the services, provisions the services one after the other, and understands the services that are called. 5.

What is the process to upgrade or downgrade a system with near-zero downtime? Hide Answer This is one of the most common AWS basic interview questions. However, to answer this well, you must list down all the required steps for the procedure. Listed below are the steps to be followed to upgrade or downgrade a system ensuring near-zero downtime:

Open EC2 console Select Operating System AMI Initiate an instance with the new instance type. Install updates Install applications Test the instance If working, deploy to the new instance and replace the previous instance.Soon, it's deployed, and now you can upgrade or downgrade 6.

Give four AWS services that are not region-specific. Hide Answer Following are four examples of AWS services that are not region-specific:

Route 53: A domain name system service IAM: Helps access AWS resources securely Web Application Firewall: To separate web-application and the internet Cloudfront: A content delivery network to deliver app, videos or data from providers to consumers quickly. 7.

Give one difference between NAT Gateways and NAT Instances. Hide Answer The Bandwidth of NAT Gateway is up to 45 Gbps and can automatically scale based on traffic requirements whereas, in NAT Instance, it depends on instance bandwidth. 8.

Define Elastic Transcoder. Hide Answer Elastic Transcoder is an AWS service tool that supports multiple devices with various resolutions and formats of video, like laptops, tablets, and smartphones. It is a cloud-based media transcoding service provided by Amazon Web Services (AWS) that enables you to convert video and audio files from one format to another. The service supports a wide range of input and output formats, codecs, and resolutions, making it easier to deliver content to various devices, including laptops, tablets, and smartphones. 9.

Define Amazon EC2? Hide Answer EC2 is also called Elastic Compute Cloud. Amazon EC2 is used to launch virtual computing servers as needed, manage storage, and configure security and networking. 10.

Elaborate on the best practices for Amazon EC2. Hide Answer Amazon EC2 offers restricted access, allowing only trusted networks to access ports on an instance. In addition, Amazon EC2 allows you to access only those permissions you require and disable other password-based logins for instances launched from your AMI.

Some best practices are as follows:

Using identity federation to manage AWS resources and APIs Using least permissive rules Using Amazon inspector to check any software vulnerabilities 11.

Can S3 be used with EC2 instances? Hide Answer Yes, Amazon S3 can be used with Amazon EC2. Here, Amazon S3 gives developers access to a highly reliable, fast and scalable data storage infrastructure. 12.

Write some tools and techniques that are used in AWS to determine if you are paying more or not. Hide Answer AWS provides the following tools to get reliable data for making cost forecasts, optimizations, or for managing the costs.

AWS Cost Explorer: Helps to track costs incurred and data used over time. AWS Budgets: Helps set custom spending plan on aws for specific time. Cost Allocation Tags: Provides tags that can be assigned to resources within your AWS account so that you can track usage and cost of AWs resources. 13.

What is a T2 instance in AWS? Hide Answer T2 instances are low-cost instance types for general use. They provide base-level CPU performance but can provide bursts above the baseline. They work best where full CPU capacity is not needed constantly and is only needed to burst higher CPU performance. 14.

List other tools which log into the cloud environment other than the console. Hide Answer There are various tools that can log into the cloud environment, in addition to the console. Some common ones include:

Putty AWS CLI for Linux AWS CLI for Windows Eclipse AWS SDK 15.

List the services that can be used to create a centralized logging solution. Hide Answer A centralized logging solution enables organizations to gather, analyze and display Amazon CloudWatch Logs in one central place. You can use Amazon CloudWatch Logs, Amazon ElasticSearch, and Amazon Kinesis to create a centralized logging solution. 16.

List the two native AWS security logging capabilities. Hide Answer Two popular AWS services that provide security log data to provide insight into how the service is operating are:

AWS CloudTrail AWS Config Besides this, AWS Security Hub and AWS GuardDuty can also be used for insights into your security. 17.

Explain the DDoS attack. Hide Answer DDoS is a cyber-attack. Here, the perpetrator accesses a website and creates numerous sessions so that the other fair users cannot access the service. 18.

List the tools to minimize DDoS attacks on your AWS services. Hide Answer The following tools can be used to minimize DDoS attacks on AWS services:

AWS Shield AWS Waf Amazon CloudFront ELB Virtual Private Cloud (VPC) 19.

Using what do you monitor website metrics in real-time in AWS? Hide Answer Using Amazon CloudWatch, you can set up a system monitor to monitor state changes in scheduled events, Amazon EC2, Auto-scaling lifecycle events, AWS API calls and Console sign-in events.

Beside this, you can also use AWS Lambda and AWS Elasticsearch for real-time website metrics monitoring. 20.

List the different types of virtualization in AWS. Hide Answer There are three types of virtualization in AWS. These include:

Hardware Virtual Machine (HVM) Paravirtualization (PV) Paravirtualization on HVM 21.

How are stopping and terminating an EC2 instance different? Hide Answer Stopping an EC2 instance means you are normally shutting it down and moving it to a stopped state. On the other hand, terminating the instance means you are permanently deleting the instance. When this happens, it’s attached volumes are deleted and you cannot recover them. 22.

Tell the names of three types of EC2 instances based on their costs. Hide Answer The three types of EC2 instances based on their costs are as follows:

On-demand Instance Spot Instance Reserved Instance 23.

Write steps to enable SSH agent forwarding? Hide Answer SSH agent forwarding is a process whereby a SSH server gets access to SSH client and can be enabled as follows:

Enable SSH agent

#starting up ssh-agent in the background $ eval "$(ssh-agent -s)" Agent pid 6969

Now, we add SSH key to the SSH-agent

$ ssh-add ~/.ssh/id_rsa

Connect to the host

ssh -i ~/.ssh/id_rsa user@our_host_ip 24.

Are Solaris and AIX operating systems available with AWS? Hide Answer No, both operating systems are not available with Amazon Web Service. 25.

How do you set CloudWatch to recover an EC2 instance? Hide Answer You can follow these steps to set the AWS CloudWatch to recover an EC2 instance:

Create an Alarm using Amazon CloudWatch Then, Define Alarm→ Actions tab Choose to Recover this 26.

List the three common types of AMI designs. Hide Answer The three most common types of AMI designs are as follows:

Fully Baked AMI Just Enough Baked AMI (JeOS AMI) Hybrid AMI 27.

Explain Key-Pairs in AWS. Hide Answer Key-pairs in AWS are secured login information for virtual machines. They are password protected login credentials to verify your identity while connecting the Amazon EC2 instances. AWS key-pairs are made up of private and public keys that connect to the instances. 28.

Define Amazon S3. Hide Answer S3 stands for Simple Storage Service. Amazon S3 is the best-supported storage platform available. It helps to supervise data for cost optimization, compliance, and access control. 29.

How will you recover an EC2 instance for which you have lost the key? Hide Answer The following steps can be followed to recover an EC2 instance whose key has been lost:

Check that the EC2Config service is running Stop the original instance before proceeding further Separate the root volume for the instance Attach it to a temporary instance Mount the volume on temporary instance Modify the configuration file Unmount the volume and detach it from temporary instance Reattach the volume to original instance Restart the original instance 30.

List some policies you can set for your users’ passwords. Hide Answer Some of the policies that can be set for a user’s passwords, include:

Minimum length of the password Particular character types Automatic expiration of password.
