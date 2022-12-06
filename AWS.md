# Aws
VmTutes-Amazon Web Services

Amazon Web Services(AWS)
========================

Index:-
-------
$ Traditional Infrastructure Scalling (Physical Servers)
$ Cloud Computing
$ Cloud Computing Providers(Vendors)
$ Cloud Service Models
$ Introduction to AWS
$ Why AWS?
$ AWS Global infra
$ EC2
$ Mutli-Factor authentication
$ Putty
$ MobaExterm
$ Basic Networking
$ IP Addressing
$ Subnets
$ VPC
$ Elastic IP
$ security groups

Amazon Web Services is a subsidiary of Amazon rendering on-demand cloud computing platforms and application programming interfaces to selves, organizations, and governments, on a metered pay-as-you-go basis.
Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides reliable, resizable measuring capacity in the cloud that is designed to create web-scale cloud computing more convenient for the developers.
It renders total control of computing resources that can run on Amazon's proven computing environment.


Traditional Infrastructure Scalling(Physical Servers):-
------------------------------------------------------
	>> Expensive
	>> Time Consumption
	>> Physical Server Purchase:- Lenghthy Process (Quate-->>Approved-->>Delivery-->>Fixing-->>Installations-->>Configurations..etc) 
	>> Man Power:- system admins, backup admins, Data Center admins, storage administrators...etc
	>> Scalling Issues:- unexpected grouth in your business
        >> you may have the good demand but you don't have enoughf resources(Lack of resources)
        >> you may have enoughf resources, But you don't have demand(so, Here Wasting the resources)   	

Cloud Computing:-
----------------
Getting Required IT Resources from internet.

	Def:- Cloud Computing is the On-Demand delivering of database storage, Applications, 
      	      and other IT Rsources through a cloud service platform via INTERNET with pay-as-you-go Pricing.
	>> Less Expensive
	>> 0% Investment for your Infrastructure
	>> Measured Services :- Pay based on your consumption
        >> Rapid Elasticity :- Resources are quickly scalable and flexible based on your business needs
	>> Resource Pulling:- One resource can access by multile customers, Instead of accessing from different entitys.
	>> Global Infrastructure
        
          
               
        Pre-Req:-  No need to install any software and hardware, Only internet connection is enoughf to access your services.

Cloud Computing Providers(Vendors):- 
-------------------------------------
                                             AWS,
                                             Azure,
                                             GCP,
                                             Digital Occean,
                                             IBM Bluemix/Softlayer,
                                             Alibaba, ...etc


Cloud Service Models:-
----------------------
Infrastructure As A Service(IAAS):-
		- A New Flat where you not have all amenities except windows and doors
                - Computers, Network, VM's and Storage, Operating systems, IP Addresse Firewalls,...etc
		- AWS Login, EC2, VPC, S3...etc 
		- Amazon's AWS is MASTER in the Iaas
		
Platform As A Service(PAAS) (Vendor Restricted):-
                - It is like fully Furnished Flat(Studio Apartment with all amenities)
		- Operating systems(UBUNTU,REDHAT,AMAZON-LINUX), Programming Languages(c++), Storage(RDS), Permissions...etc
		- Microsoft Azure is MASTER in the Paas. 
		
Software As A Service(SAAS) (Ready Made):-
		- Salesforce, Slack, DropBox, Office 365, ZOHO,...etc
		- Development, Deployment, servers, Resorces, Process, Storage, No need to install in PC.
		- If you need 100 Mail accounts, you can directly contact office 365.

 Note:- Backup as a service (Baas)
        security as a service (Saas)
        Disaster recovery as a service (DRaaS) 
 
Why AWS?
--------
1. Linux
2. aws services are very less in cost.
3. one year free aws account
4. Iaas --->> Infrastructure As A Service

It is Based on different Criterias like, speed, security, Support, Cost ,Flexible, User Friendly....etc

AWS Global infrastructure
-------------------------
 - Magic Quadrant for Cloud Infrastructure as a Service
 - AWS Global Infrastructure Map
      > AWS now spans 77 Availability Zones(data centers) within 24 geographic regions around the world
      > how to find location of data centers
      > archetecture of global infra...
      

Free Tier
==========
 aws.amazon.com/free

 How to know whether account is created or not
===============================================
 	1. it will debit 2 Rs (or) 1$ from your debit/credit card 
 	2. Go to EC2 and check whether all the options are displaying or not

   Note:- in case if it is not activated, you can raise a support request

Amazon Elastic Compute Cloud (Amazon EC2)
=========================================
Def:- Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure and resizable compute capacity in the cloud.

1. choose AMI(amazon machine image)
     - aws providing few default images in quick start section, and we can create our own images also(i.e my AMI's)
2. choose Instance Type
     - instance types differ like nano, micro, medium, large, extra-large with latest hardware machines.
3. Configure Instance
     - select number of instances required
4. Add Storage
     - default 8gb in t2.micro
5. Add Tags
     - a quick and easy accessibility
6. Configure Security Group
     - A security group is a set of firewall rules that control the traffic for your instance. On this page, you can add rules to             allow specific traffic to reach your instance.
7. Review
     - Review your instance launch details. You can go back to edit changes for each section


Note:- t2, t3, c1, c2...etc about underlying the hardware, Highest the number latest the hardware


key pair:-
=========
A key pair, consisting of a private key and a public key, is a set of security credentials that you use to prove your identity when connecting to an instance.

Ways to connect to Ec2 Instance:-
===============================
1. by installing 3rd party tools
2. by using default installed tools 
3. aws cloud-shell (VmTutes Recommended)
4. Amazon Ec2 Instance Connect (VmTutes Recommended)

How to connect to aws EC2 instance by Installing 3rd party tools in your computer
=================================================================================
From Windows:
-------------
1. Putty
2. Windows Terminal
3. MobaXterm (vmtutes Recommended)
4. Solar PuTTY
5. WinSCP
6. SmarTTY
7. Xshell ...etc

   MobaXterm:- (vmtutes Recommended)
   ---------------------------------
step-1. https://mobaxterm.mobatek.net/download.html
step-2. select mobaxterm portable edition in website for download and unzip it using WinRAR software.
step-3. select SESSION in mobaxterm dashboard and select SSH protocal
step-4. Give remote host(public ip address or public DNS name)
step-5. specify username (default user name in aws cloud is "ec2-user")
step-6. browse and give private key under advanced SSH Settings
step-7. give session name under bookmark settings 
Note:- 
  > You can check the "Enable SSH keepalive" box under "Settings" --> "Configuration" --> "SSH" tab.
  > Enabling this option will ensure that the connection is kept "fresh" in the device's connection table.
  > here directly we can connect to EC2 instances with PEM files, no need of PPK.


  Putty:- 
  ----- 
>. Generate key-pair, Privacy-Enhanced Mail(.PEM) :- 
   A key pair, consisting of a private key and a public key, is a set of security credentials that you use to prove your identity when    connecting to an instance. Amazon EC2 stores the public key, and you store the private key. You use the private key, instead of a    password, to securely access your instances. Anyone who possesses your private keys can connect to your instances, so it's    important that you store your private keys in a secure place.

>. Download and install putty and puttygen softwares
    https://www.putty.org/ (putty)
    https://the.earth.li/~sgtatham/putty/latest/w64/puttygen.exe (puttygen)

>. convert .pem to .ppk by using puttygen software.
>. connect to EC2 instance with putty tool by using Putty Private Key(.PPK)


From Mac:-
----------
1. Putty for mac
2. iterm
3. Termius
4. ZOC Terminal
5. Tabby ...etc

How to connect to aws EC2 instance Without Installing any 3rd party tools in your computer
==========================================================================================
From Winodws:-
------------
# Command Prompt(CMD)--> (VmTtues Recommanded)

1. Open command prompt and navigate to private key location in your computer (eg:- cd /Downloads/vmtutes.pem)
2. Run this command, if necessary, to ensure your key is not publicly viewable.
    -> chmod 400 VmTutes.pem
3. Connect to your instance using its Public IP/DNS:
    -> Example:   ssh -i "VmTutes.pem" ec2-user@ec2-52-90-56-98.compute-1.amazonaws.com


From Mac:-
----------
# Mac Terminal

1. Open an SSH client. (open Terminal in mac) 
        Note:-  Press Command + Space Bar on your Mac Keyboard and search for terminal, open it.
2. Locate your private key file(cd Downloads/)
3. Run this command, if necessary, to ensure your key is not publicly viewable.
     -> chmod 400 vm-key.pem
4. Connect to your instance using its Public IP/DNS:
     -> Example:   ssh -i "Vinodh-Machireddy-key.pem" ec2-user@ec2-54-215-187-184.us-west-1.compute.amazonaws.com


How to connect to aws EC2 Instance using Cloud-Shell
====================================================

AWS CloudShell is a browser-based shell that gives you command-line access to your AWS resources in the selected AWS region. AWS CloudShell comes pre-installed with popular tools for resource management and creation.
You have the same credentials as you used to log in to the console.
- With AWS CloudShell, you have persistent storage of 1 GB for each AWS Region at no cost.
- CloudShell runs on Amazon Linux 2, with 1 vCPU and 2 GiB RAM
- pre-installed software like python, git, basic linux commands, node.js etc
- Concurrent shells: You can run up to 10 shells at the same time in each AWS Region at no charge.
- Supported AWS Regions for AWS CloudShell. https://docs.aws.amazon.com/cloudshell/latest/userguide/supported-aws-regions.html
- active sessions: AWS CloudShell is an interactive shell environment—if you don't interact with it using your keyboard or pointer      for 20–30 minutes, your shell session ends. Running processes don't count as interactions.

Note:- https://docs.aws.amazon.com/cloudshell/latest/userguide/limits.html (or)
Note:- https://docs.aws.amazon.com/cloudshell/latest/userguide/welcome.html

How to connect to aws EC2 Instance using amazon EC2 Instance Connect
====================================================================
- Amazon EC2 Instance Connect is a simple and secure way to connect to your instances using Secure Shell (SSH).
- By using this we can connect to instance directly without any 3rd party tools.
- Supported Linux distributions: Amazon Linux 2 (any version), Ubuntu 16.04 or later
- EC2 Instance Connect is now available at no additional cost in US East (Ohio and N. Virginia),
  	US West (N. California and Oregon),
  	Asia Pacific (Mumbai, Seoul, Singapore, Sydney, and Tokyo), 
  	Canada (Central), 
  	EU (Frankfurt, Ireland, London, and Paris), and South America (São Paulo) AWS regions.
Note:- https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-connect-methods.html


After connecting to instance Do This steps:-
===========================================
1. create user
     # useradd VmTutes
2. Generate Password for vmtutes
     # passwd VmTutes
3. add VmTutes user in "visudo" (or) /etc/sudoers file for sudo permissions
     # vmtutes ALL=(ALL) NOPASSWD: ALL
4. Enable "PasswordAuthentication yes" in vi /etc/ssh/sshd_config  file.
5. Restart the "sshd" service
     # systemctl restart sshd
6. ssh vmtutes@52.90.56.98


Multi-factor authentication (MFA)
---------------------------------
- high security for your account
- no one can tamper your password
- here it will generate every time new code to enter 
	eg:- like, RSA secure code

1. Go to my security credentials--->MFA-->manage MFA device -->virtual MFA device-->show QR code
2. Go to google play store-->install google Multi-factor authentication app-->scan QR code--> and enter 6 digit code.
3. How to remove -->go to MFA---> select manage--> remove


 Virtual MFA Applications

Applications for your smartphone can be installed from the application store that is specific to your phone type. The following table lists some applications for different smartphone types.
 Android 	Authy, Duo Mobile, LastPass Authenticator, Microsoft Authenticator, Google Authenticator
 iPhone 	Authy, Duo Mobile, LastPass Authenticator, Microsoft Authenticator, Google Authenticator


Tracking your AWS Free Tier usages
----------------------------------

1. Sign in to the AWS Management Console and open the Billing and Cost Management console at https://console.aws.amazon.com/billing/
2. Under Preferences in the navigation pane, choose Billing preferences.
3. Under Cost Management Preferences, under Receive AWS Free Tier Usage Alerts in the Email Address dialog box, enter the email    address where you want to receive the usage alerts.
4. Scroll to the end of the page and choose Save preferences.

   
Networking
==========
- servers
- lan 
- switch
- router
- vlan
- subnets


Layers of OSI Model
OSI--> OpenSource Systems Interconnetion Model 
OSI model has seven layers which are as follows:

The Application Layer -->L7
The Presentation Layer -->L6
The Session Layer -->L5
The Transport Layer-->L4
The Network Layer --> L3 
The Data Link Layer--> L2
The Physical Layer --> L1


IPaddressing
============
ip address:- is a uniq identity for every device over the internet 

types:-
--------
private ip and
public ip

ip classes
----------

Class A 1.0.0.1 to 126.255.255.254
 - private class A 10.0.0.0 - 10.255.255.255
Class B 128.1.0.1 to 191.255.255.254
 - private class B 172.16.0.0 - 172.31.255.255
Class C 192.0.1.1 to 223.255.254.254
 - private class C 192.168.0.0 - 192.168.255.255
Note:- this 3 classes comes under civilian network


Class D 224.0.0.0 to 239.255.255.255
Class E 240.0.0.0 to 254.255.255.254
Note:- we will not use this D and E classes, Only for militry,defence,navy, research and development purposes.

- NAT network address translation

ip versions:-
-------------
ipv4 - 32 bit     0.0.0.0 to 255.255.255.255
ipv6  - 128 bit


- 192.168.1.200
- 2 types of ip addr
    > IPV4 - 32 bit
   
- 000
  001
  010
  011
  100
  101
  110
  111 

sub-networking(subnets)
-----------------------
A subnetting, or subnetworking, is the process of splitting a single large network into two or more strands. (or) dividing a large network into multiple small networks.
 
10.0.0.1-254 network 
    10.0.0.0 - network Address
    10.0.0.1
    10.0.0.2
    10.0.0.3
    10.0.0.255: Network broadcast address. We do not support broadcast in a VPC.
255.255.255.0/24  - subnet mask

usa
10.1.0.0/16  - 255.255.0.0 (main network)
10.1.1.0/24
10.1.2.0/24
10.1.3.0/24
.
.
.
..
10.1.255.0/24


india 10.91.0.0/16 - 65,025 IP's
paki  10.92.0.0/16 - 65,025 IP's
uk    10.44.0.0/16 - 65,025 IP's
aus   10.61.0.0/16 - 65,025 IP's
mala  10.60.0.0/16 - 65,025 IP's


VPC
====
- virtual private cloud
- Amazon Virtual Private Cloud is a commercial cloud computing service that provides users a virtual private cloud.

public cloud 

private cloud


vpc is region specific, it will spane to all az in the region


1. isolation of the resources/servers
2. we can create diff vpc's for diff environments(like testing,dev,pre-prod,prod). so, it makes management easy
3. ip address overlapping 

note:- we can create same(name) vpc in other region also.
note:- we can create multiple subnets in one AZ with diff ip address range. we can use same ip addr range in another vpc.
note:- in one region 5 VPC's you can create and you need permission to extend

subnets
-------
- create subnets by dividing VPC ip range (10.1.0.0/16) 
- we can also create multiple subnets in one AZ/DC

Internet Gateway(IGW)
---------------------

- An Internet Gateway (IGW) is a logical connection between an Amazon VPC and the Internet.
- It is not a physical device.
- Only one IGW can be associated with one VPC.
- If a VPC does not have an Internet Gateway, then the resources in the VPC cannot be accessed from the Internet

- after creating IGW we need to attach to VPC to communicate with internet

Route Table
-----------
- A route table contains a set of rules, called routes, that are used to determine where network traffic from your subnet or gateway   is directed. To put it simply, a route table tells network packets which way they need to go to get to their destination.
- default direction is local, means by default it communicates with local servers in AZ/DC of a region. 10.1.0.0/16
- if you want to communicate ouside with internet by using IGW. give 0.0.0.0/0

Security Group
==============
what is SG:- An AWS security group acts as a virtual firewall for your EC2 instances to control incoming and outgoing traffic. Both              inbound and outbound rules control the flow of traffic to and traffic from your instance, respectively.


How it works:- AWS Security Groups help you secure your cloud environment by controlling how traffic will be allowed into your EC2                machines. With Security Groups, you can ensure that all the traffic that flows at the instance level is only through                   your established ports and protocols.

- Basically security groups are  FIREWALLS at instance level like ( EC2,LOAD BALANCER, S3,RDS...etc)
- STATEFULL firewall:- only one side traffic need to be opened

what is FIREWALL:- a firewall is a network security system that monitors and controls incoming and outgoing network traffic based on   ----------------   predetermined security rules.

Rules:-
------
OUTBOUND:- going out --> by default it allow all the traffic
INBOUND:- coming in(carefull)

PORTS:- applications runs on port numbers
-------
SSH - 22
HTTP - 80
HTTPS - 443
RDP - 3389
MSSQL - 1433
DNS - 53

note:-   once we create a VPC you will get default SG, in which OUTBOUND traffic allows default.(any one can go out) 
note:- we can assign 5 SG's to an instance and you need permission to extend.

Network Access Control List (NACL)
==================================

- NACL is a FIREWALL
- Basically SG are FIREWALLS at subnet level
- by default NACL will be create for VPC
- STATELESS:- both the sides traffic need to be opened(in and out bounds)

Note:- if you do any changes in NACL it applys to all the subnets which are associate with NACL. (99% WE WILL NOT CHANGE)


key pairs
=========

A key pair, consisting of a private key and a public key, is a set of security credentials that you use to prove your identity when connecting to an instance.

- aws will have public key and you will be given private key.
- we need to use private key to login to the ec2 instance.

LOCK - private key - this key will be with AWS servers
KEY -  publick key - this key will be with users


Elastic ip
==========

Private ip addresses:-   are not reachable over the internet, and can be used for communication between the instances in your VPC. 
                         (for internal communication only and it is mandatory) 

Public ip addresses:- A public IP address is an IPv4 address that's reachable from the Internet. You can use public addresses for                            communication between your instances and the Internet.
                      (you can connect to your instance from anywhere with public ip, and it is not mandatory)

Elastic ip:- An Elastic IP address is a reserved public IP address that you can assign to any EC2 instance in a particular region,              until you choose to release it.

   - An Elastic IP address is static; it does not change over time.
   - To use an Elastic IP address, you first allocate one to your account, and then associate it with your instance. 

Elastic IP address pricing:- 

To ensure efficient use of Elastic IP addresses, we impose a small hourly charge if an Elastic IP address is not associated with a running instance, or if it is associated with a stopped instance or an unattached network interface. While your instance is running, you are not charged for one Elastic IP address associated with the instance, but you are charged for any additional Elastic IP addresses associated with the instance. 


EBS
===

- Elastic block storage
- Elastic Block Store (EBS) is a block storage service based in the AWS cloud. EBS stores huge amounts of data in blocks, which work   like hard drives (called volumes). You can use it to store any type of data, including file systems, transactional data, NoSQL and   relational databases, backup instances, containers, and applications.
- it is a permanent storage, data will not be deleted when you start and stop the instance/server.
- only one volume can assign to one server only.
- we can increase EBS storage from 1gb - 16tb
- EC2 boot volume is always EBS volume

- instance storage
  ================
  1. An instance store provides temporary block-level storage for your instance.
  2. data will be deleted when you stop the instance.
  3. EC2 boot volume cannot be boot


                                                 ====THE END====       
			VmTutes, +91-7204143230(WhatsApp/Call), Email:- Vinodh-Machireddy@VmTutes.com
      
      
      
      
