# AWS Cloud Practitioner CLF-C02
---
## Cloud Computing
- Is the on-demand delivery of compute power, database, storage, applications, and other IT rsources.  Generally charge with **pay-as-you-go-pricing**.

## Go Global in Minutes
- Deploy in several regions around the world with just a few clicks.
- Over 30 geographic regions throughout the world.
- **Regions** have at least **3 availability zones**, each AZ is at least 600 miles apart.
- **Edge locations** service locations that are serviced by **availability zones**.

## Using Multiple Availability Zones
- Every AWS region is segemented into distinct AZs.
- Each AZ has its own power, cooling, and network connectivity forming an isolated failure domain.
- Customers are encouraged to run their workloads in more than one AZ.
- This ensures that customer applications can survive even a complete AZ failure.
- Standard S3 are replicated across three AZs.
- In an Amazon Relational Database Service Multi-AZ deployment, Amazon RDS automatically creates a primary database instance and synchronously replicates the data to an instance in a different AZ in the same region.
- When there's a failure, RDS automatically fails over to a standby instance without manual intervention.

## Using Multiple Regions
- Can deploy to multiple regions
- Multiple regions gives you greater control over recovery time.
- Common reasons to utilize multiple AWS regions:
    - Disaster recovery
    - Lowering latency 
    - Data dispersion initiatives
    - Data sovereignty

## Three types of service
### Infrastucture as a Service (IaaS)
- Offers basic building blocks of cloud information
- Provides access to networking features, computers, and data storage space
- Delivers customers the highest level of flexibility
- Compares to existing IT resources

*What's provided*
- AWS Endpoints
- Foundation Services
    - Compute
    - Storage
    - Database
    - Networking & CDN
    - ML - AI (not on exam)
- AWS Global Infrastructure
    - Region
    - Availability Zones (at least 3)
    - Edge Locations
- AWS IAM

### Platform as a Service (PaaS)
- Removes the need for organizations to manage the underlying infrustructure
- Allows customers to focus on the deployment and management of their applications

*What's provided*
- Development and SDK platforms
- Container Services
- Managed and fully managed relational and document databases
- Managed security and threat modeling services
- Single sign-on, ML, AI, IOT services

### Software as a service (SaaS)
- Offers customers a comprehensive solution run and managed by the service provider.
- In most cases, this involves various end-user applications.

*SaaS offerings*
- Customer relationship management (CRM)
- Enterprise resource management (ERM)
- Human resources and workplace tools
- Finance, salses, and marketing
- Payroll Services
- Email, collaboration, and cloud storage
- Help/service desk
- Virtual call center
- Business analytics

## Cloud computing deployment models
### Cloud Model
- A cloud-based application is fully deployed in the cloud, and all parts are in the cloud.

### Hybrid
- Some things run in the cloud and some things do not.
- Online retailers may use hybrid cloud for "bursting up"

### On-Premise
- Your own IT setup, your own server.

## AWS Shared responsibility model (SRM)
- Customers should carefully evealuate the selected services
- Their responsibilities vary, contingent on the services used, the integration of those services into their IT environment, and any relevant laws and regulations
   - This is highly applicable to the Platform as a Service (PaaS) models
- The nature of this shared responsibility also provides the flexibility and customer control that permits the deployment.

### AWS Responsibilities
- AWS is responsible for defending the infrastructure that runs all the services offered in the AWS Cloud.
- This infrastructure is composed of the hardware, software, networking, and facilities that run AWS Cloud services all over the world.
- Responsibilities:
    - AWS responsibility: security **of** the cloud
    - Customer responsibility: security **in** the cloud

### Shared Controls
- **Patch management** - AWS must patch and fix config flaws within the infrastructure, but customers are responsible for patching their guest operating systems and applications.
- **Configurations management** - AWS preserves the configuration of its infrastructure devices, but customers are responsible for configuring their own guest operating systems, databases, and applications.
- **Awareness and training** - AWS trains AWS employees, but the customer must provide their own training for their own employees.

### Customer Responsibilities on AWS
- Driven by the cloud services that a customer chooses.
- Customers that deploy an EC2 instance are responsible for managing: 
    - The guest operating system (updates and security patches)
    - Any application software or utilities installed by the customer on the instances
    - Configuration of the AWS-provided firewall on each instance

## Advantages of High Availability
- Protect against data center, availability zone (AZ), server, network, and storage subsystem failures
    - Keep your organization or business running with little or no downtime
- All AZs in an AWS region are interconnected with high-bandwidth, low-latency networking, over fully redundant, dedicated metro fiber
- Data centers located in different AWS AZs have a discrete, uninterruiptible power supply and onsite backup generation facilities.

## Advatnages of Elasticity
- Provides the ability to almost instatnly provision and de-provision assorted cloud resources
    - Virtual instance, containers, appliances, dtabase tables, and more
- It involves leveraging dynamic auto scaling technologies
- Challenges with predicting demand leads to higher costs for the enterprise.
- Recent circumstances have revealed how de-provisioning may be the more vital aspect of elasticity.
- Use auto-scaling to reduce waste

## Advantages of Agility
- Agility leverages features for rapid deployment, testing, experimentation, and innovation
- Customers can quickly overcome geographical limitations
- Content creators can get customer content as close to the consumer as possible
- Agility means reducing time and costs for testing, innovations, and experimentation

## Cloud Adoption Resources
- **AWS Professional Services** - A global team of experts that can help customers realize their desired business outcomes.
- **AWS Solutions Architects** - Certified cloud architects
- **AWS Activate for Startups** - Free templates, tools, resources, content, and expert support to accelerate the startup.
- **AWS Knowledge Center** - helps answer the questions most frequently asked by AWS Support customers
- **AWS Compliance**
- **The AWS Cloud Adoption Framework**

## The AWS Cloud Adoption Framework
- The AWS CAF organizes guidance into siz areas of focus, called Perspectives
- Each Perspective speaks to discrete responsibilities
- The plannin gprocess assists the right stakeholders across the oraganization prepare for their coming changes
- In general, the Business, People, and Governance Perspectives focus on business capabilities
- The Platform, Security, and Operations Perspectives focus on technical capabilities.
- **Four Pillars**:
    - **Envision** - Identify and prioritize transformation opportunities in line with your strategic objectives.
    - **Align** - Identify capability gaps and cross-organizational dependencies.
    - **Launch** - Deliver pilots in production and demonstrate incremental business value.
    - **Scale** - Expand pilots and business value to desired scale.

## The AWS CAF Governance Perspective Capabilities
- Program and project management
- Benefits management
- **Risk management**
- **Cloud financial management**
- Application portfolio management
- Data governance
- Data curation
- **EXAM: NOT PRODUCT MANAGEMENT**

## Costs of On-Premises Environments
- On-premises costs can quickly be burdensome and prohibitive.
- Customers are discovering the massive savings in labor costs and other overhead by moving to the AWS cloud.
- Altough capital expenditures like hardware, racks, and network equipment are a one-time purchase, they typically have a refresh cycle of five years.

## Cost Savings of Moving to the cloud
- The value of cloud extends beyond total cost of ownership (TCO) reduction
- Productivity, operational resilience, and corporate agility are enhanced.
- Average cost savings of 31%

| Fixed Cost Examples                     | Variable Cost Examples                                   |
| --------------------------------------- | -------------------------------------------------------- |
| Data Centers and server farms           | Virtual instances of Windows and Linux                   |
| Physical blade servers and racks        | Serverless solutions linke Functions as a Service (FaaS) |
| Storage Area Networks (SAN)             | Relational database services                             |
| Buildings, HVAC, Environmental Controls | Elastic file services                                    |

## AWS Licensing Strategies
- **Buy licenses from AWS** - allows you to fully compliant Microsfot software licenses bundled with Amazon EC2 or Amazon RDS instances and pay for them as you go with no upfront costs or long-term investments.
- **Bring licenses to AWS** - If you've already purcahse Microsoft software, you have the option to bring your own licenses (BYOL) to the AWS Cloud.
    - Without software assurance
    - With software assurance

## The Right Sizing Concept
- Right sizing - **What is the practice of mapping instance types and sizes to worklowad performance and capacity requirements at the lowest feasible cost?**
- Involves observing deployed instances and recognizing openings to eradicate or downsize without compromising capacity or other requirements.
- It is a key mechanism for optimizing costs and is often overlooked by organizations when they first transfer to the AWS Cloud.

## Data Transfer Charges
- **There is no charge for inbound data transfer across all services in all regions at Amazon Web Services**
- Data transfer from AWS to the internet is charged per service, with rates specific to the initiating region
- Data transfer within AWS can be from the customer's workload to other AWS services, or it could be between different components of the customer workload.
- When a customer workload accesses AWS services, they may invite data transfer charges.

## AWS Tags
- A tag is a label that a customer or AWS assigns to an AWS resource
- Every tag is made up of a key and a value
- For each resource, the tag key must be unique, and each tag key can have only a single value
- Customers can use tags to organize their resources

## Cost Allocation Tags
- Two types of cost allocation tags:
    - AWS-generated tags
    - User-defined tags
- AWS defines, creates, and applies the AWS-generated tags for the customer
- The customer defines, creates, and applies the user-defined tags
- **Customers must activate both types of tags separately before they can appear in *Cost Explorer* or on a *cost allocation* report**

## AWS Organizations
- AWS organizations provide policy-based management for multiple AWS accounts, including:
    - Creating groups of accounts
    - Automating account creation using console and APIs
    - Applying and managing policies for account groups
- Customers can centrally manage Service Control Policies (SCPs) across multiple accounts without using manual processes
    - An SCP allows administrators to place guardrails on highly privileged principals with "deny" statements in JSON-managed security policies

## Comparing AWS Support Plans
- **Developer** - Recommended if you are experimenting or testing in AWS.
- **Business** - Minimum recommended iter if you have production workloads in AWS
- **Enterprise On-Ramp** - Recommended if you have production and/or business critical workloads in AWS
- **Enterprise** - Recommended if you have business and/or mission critical workloads in AWS

## Trusted Advisor
- Recommendations
    - Cost optimization
    - **Performance**
    - Security
    - **Fault Tolerance**
    - **Service Limits**
    - **Operational Excellence**

## Governance at AWS
- Governance of the corporate environment is critical to understand why and how cloud services are consumed
- The cloud environment must align with the organization's strategy on cloud service provider utilization
- All organizations, regardless of size and industry, need to establish a capability to effectively use cloud services, define policies and standeards, understand and mitigate risks, and approve essential legal, commercial, and regulatory requirements.

## AWS Compliance Concepts
- AWS supports over 140 security standards and compliance certifications around the globe including:
    - Payment Card Industry Data Security Standard (PCI-DSS)
    - Health Insurance Portablility and Accountablility Act(HIPPA)/HEalth Information Technology for Economic and Clinical Health Act (HITECH)
    - Federal Risk and Authorization management Program (FedRAMP)
    - General Data Protection Regulation (GDPR)
    - Federal Inforamtion Processing Standard 140-2 (FIPS 140-2)
    - National Institute of Standards and Technology 800-171(NIST 800-171)

## Governance and Compliance Support Services
- CloudWatch - Visualizes real time logs.
- CloudTrail - Monitors API calls.
- AWS Audit Manager - Maps customer compliance
- AWS Config - Evaluates configurations.

## AWS Artifact
- Is a console-based, self-service auditing object retrieval service taht gives customers quick and simple access to AWS compliance documentation and agreements.
- Artifact **Agreements** enable customers to examine, approve, and manage agreements in AWS Organizations.
- Artifact **reports** deliver compliance reports from third-party auditors who have tested and verified that AWS is compliant with a variety of global, regional, and industry-specific security standards and regulations.

## AWS Audit Manager
- Customers use audit manager to map their compliance requirements to AWS usage data with prebuilt and custom frameworks and automated evidence collection.
- Over time the organization can save time by incorporating audit compliance processes into the DevOps model.
- Audit Manager creates an HTTPS API endpoint to accomplish its solutions.

## Well-Architected Framework Pillars
- **Operational Excellence**
    - Design Priniples
        - Perform operations as code
        - Make frequent, samll, reversible changes
        - Refine operations procedures frequently
        - Anticipate failure
        - Learn from all operational failures
- Security
- **Reliability**
- **Performance Efficiency**
- Cost Optimization
- **Sustainability**

## Common VPC Addressing
- Default VPC CIDR prefix is 172.16.0.0/16 (Don't use 172.17.0.0)
- Default subnets are /20 that provides 4089 hosts
- Need ~2000 hosts? Use a /21 CIDR
- Need ~1000 hosts? Use a /22 CIDR
- Need ~500 hosts? Use a /23 CIDR
- Need ~250 hosts? Use a /24 CIDR
- **All IPv6 hosts have a /64 CIDR**

## VPC Peering
- Used to send data from one Subnet/VPC to another.

## AWS Transit Gateway
- Simplifies peering.

## AWS Certificate Manager (ACM)
- AWS customers can leverage the AWS Certificate Manager(ACM) to provision, manage, and deploy public and private TLS certificates for use with AWS services and even internal connected resources
- ACM removes the time-consuming manual process of acquiring, loading, and renewing TLS certificates
    - Domain-validated public certificates
    - Private certificates from AWS Private CA
    - Importaed public or private certificates

## AWS Load Balancing
- Is a technique for allocating network traffic equally across a pool of resources that host an application.
- Modern applications must process millions of users at the same time and respond with the requested files, videos, images, and other data in a rapid and reliable way
- To accommodate high amounts of traffic, most applications have numerous resource servers that transfer data between them

## Edge Network Services 
### Amazon CloudFront
- Is a content deilvery network (CDN) service designed for high performance, security, and developer suitability.
- Securely delivers data, videos, applications, and APIs to customers globally with low latency and high transfer speeds within a developer-friendly environment.
- Is integrated with AWS - both physical locations that are directly connected to the AWS global edge locations and various service endpoints.

### Global Accelerator
- Is a networking service that enables customers to expand the availability, performance, and security of their public applications
- Offers two global static public IPs that represent a fixed entry point to application endpoint such as Application Load Balancers, network Load Balancer, Amazon Elastic Compute Cloud (EC2) instances, and elastic IPs.
- Connect up to 10 regions
    - Network Load Balancer
    - Application Load Balancer
    - Amazon EC2

## AWS Outposts
- Outposts is a collection of fully managed solutions that deliver AWS infrastructure and services to most on-premises or edge locations for a reliablehybrid cloud experience.
- With AWS Outposts, customers can run some AWS services on-premises and connect to a wide array of services available in the local AWS Region.
- It is available in a variety of form factors including racks and multiple racks:
    - The AWS Outposts rack is an industry-standeard 42U form factor 
    - The AWS Outposts servers come in a 1U or 2U form factor

## AWS Security Triad
- Infrastructure security
- Identity and Access Management (IAM)
- Key Management Service (KMS)

## NACLs
- A NACL is agnostic of Transmission Control Protocol (TCP) connections or User Datagram Protocol (UDP)/Internet Control Message Protocol (ICMP) flows
- They are stateless (static) in that the return traffic must be explicitly allowed in the inbound NACL
- These firewalls work together with security groups and can permit or deny traffic before it reaches the interfaces

## Security Groups
- Security Group (SG) firewalls apply to individual Elastic Compute Cloud (EC2) instances in a subnet
- They operate at the hypervisor level attached to the virtual elastic network interfaces (eth0)
- SGs are layer 3/4 stateful virtual "Allow Only" firewalls
- They have no explicit deny rules like NACLs
- ALL EC2 instances are launced with the default SG unless oterwise designated
- All rules in all applied SGs are evaluated before a decisioion is made

## Web Application Firewall (WAF)
- AWS WAF is an HTTP/S deep packet inspection firewall that defends against common web exploits and bots that can affect availability, compromise security, or consume excessive resources
- With AWS WAF, customers can create secruity rules or use third-party solutions that control bot traffic and bnlock common attack patters such as SQL injection or cross-site scripting (XSS)
- WAF is usually bundled with Shiled Standard for AWS customers

## AWS Firewall Manager
- Firewall Manager is an Amazon Web Services security management servcie taht enables clients to centrally configure and administer firewall rules across accounts and applications in AWS organizations.
- As new applications are built or bought, Firewall Manager simplifies the process of introducting them and associated resources into compliance by enforcing a common set of security rules.

## Least Privilege Principle
- Least privilege is the principle that a security architecture should be utilizing so taht each subject is granted the minimum system resources and authorizations that the entity needs to condut its activities.
- When related to data and information, this is often called the "need to know" principle.
- At AWS, this ofent applied with a role-based access control (RBAC) model unless federated single sign-on (SSO) is being used.

## AWS IAM Least Privilege
- When setting permissions with Identity and Access Management policies, grant only the permissions necessary to perform a task
- This is accomplished by defining the actions that can be taken on specific resource objects under certain conditions
- Administrators often begin with borader permissions, then subsequently explore the permissions that are needed for a particular workload or use case.

## The AWS Root Account
- When the customer first creates an AWS account, they begin with a single sign-in identity that has complete access to all AWS services and resources in the account
- Username and email address must be unique when creating an account.
- The IAM password policy does not apply to the root account
- Always use a physiucal or software-based multi-factor token access on the root account

## Root Account Distinctives
- Customers are strongly discouraged from using the root user for programmatic or everyday tasks
- Root user credentials are only used to perform a few account and service management tasks
- Only the root account user can:
    - Change the support plan and modify payment options and billing
    - Close an AWS account
    - Sign up for GovCloud
    - Transfer a Route 53 domain to another account
    - Create an organization
- **Never Aceess AWS programatically as Root User**

## AWS Secrets Manager
- AWS Secrets Manager helps customers manage, retrieve, and rotate database credentials, API Keys, and other secrets throught their lifecycles
- These elements should not be stored in the source
- It is supported by AWS HSM-enabled Key Management System (KMS)
- AWS Lambda automatically rotates the secrets 
- Service is commonly leveraged by RDS, Redshift clusters, DocumentDB, and other services

## AWS Systems Manager
- AWS Systems Manager is a secure end-to-end management solution for resources on AWS and in multicloud and hybrid environments
- Improves visiblity and control in the cloud, on premises, and at the edge
- Automates configuration and ongoing management of applications and resources
- **EXAM**: Session Manager is a popular managed Bastion service

## Amazon Cognito
- Supports different authentication methods, for SSO.

# DAY 2
## Amazon CloudWatch
- Amazon CloudWatch is used for management and governance
- It is a monitoring and management service designed for developers, system operators, site reliablilty engineers (SRE), and managers
- cloudWatch offers data, meaningful metrics, and actionable instights to: 
    - Monitor applications
    - Recognize and respond to system-wide performance changes
    - Optimize resource utilization
    - Gain a unified view of operational health

## CloudWatch Use Cases
- **Monitor critical metrics and logs**, visualize application and infrastructure stacks, generate alarms, and correlate metrics and logs to recognize and resolve the root cause of performance issues.
- Monitor applications and Trigger automated CloudWatch Alarms and Lambda workflows to enhance the customer experience
- Explore, analyze, and visualize logs instantly to optimize resources, leverage CloudWatch Alarms to automate capacity, and do resource planning for Auto Scaling.

## AWS CloudTrail
- With CloudTrail, customers can log, continuously monitor, and retain account activity related to all **API calls** across the AWS infrastructure
- Within CloudTrail, CloudTrail Insights can be enabled where CloudTrail can automatically detect unusual API activities in AWS accounts
- **Example**; CloudTrail Insights could detect taht a higher number of Amazon EC2 instances tahn usual have recently launcehd in an account or abnormal account acitvity hass occurred then review the full event details to determine which actions need to be take next.

## AWS CloudTrail Use Cases
- Detect that a higher number of Amazon EC2 instances than usualy have recently launched
- Identify which users and accounts called AWS, the source IP address from which the calls were made, and when the calls occurred
- Create a workflow to add a specific policy to an Amazon S3 bucket when CloudTrail logs an API call that makes that bucket public
- Connect your VPC to CloudTrail by defining an interface VPC endpoint for CloudTrail
- **Exam**: CloudTrail is one of the most common tools for getting insights into security event at AWS.

## Security Hub
- Customers can use AWS Security Hub to automate security best practice checks, combine security alerts into a single place and forma, and understand the global overall security posture across accounts
- It is similare to a virtual security opperations center (SOC) for the public and hybrid cloud deployment
- **Exam**: Use security Hub to generate a unified report across all security services

## Security Hub Use Cases
- Continuous monitoring and visibility
- Trigger automated responses
- Visualize security posture
- Perform Cloud Security Posture management
- Initiate Security Orchestartion
- Save time and money by simplifying integrations
- Discover new security findings and insights

## Amazon Inspector
- Automated vulerability management service that continually scans AWS workloads for weaknesses and inadvertent network exposures
- Automatically finds and scans running Elastic Compute (EC2) instances, container images in Amazon Elastic Container Registry (ECR) and AWS Lambda functions forn known vulerabilities and unintended exposure
- Creates a finding when it discovers a software vulerability or network configuration issue
- A finding describes the vulerability, idntifies the affected resource, rates the severity of the vulerability, and provides remediations 
- Customers can analyze results using the Amazon Inspector console or visualize and process discoveries through other associated AWS services 

## AWS Shield Standard and Advanced
- Standard provides DDoS protection provided at no extra cost
- Basic protection against common DoS floods and exploits
- Most common DDoS comes from botnet servers
- Combined with GuardDuty, NACLs, SGs, and WAF for layered defence
- Additional protection from kknown DDoS attacks with Shield Advanced
    - **Advanced must also have a Business or Enterprise support plan for 24/7 DRT 

## AWS GuardDuty
- GuardDuty is a managed threat detection service that constantly monitors for malevolent and unauthorized behavior
- Just turn it on, no config
- Watches out for unusual application programming interface (API) calls or potentially unauthorized deployments that indicate a possible account compromise (zero day)
- Detects potentially comporomised instances or reconnaissance by advanced persistent threat actors
- Utilizes proprietary machine learning (ML) and artificial intelligence (AI) along with strategic partners like CrowdStrke, Splunk, Trend Micro, Trustwave, Rapid7, and Alert Logic
- The finding details include information about what occurred, what AWS resources were involved in the suspicious activity, when this activity took place, and other data
- The finding type provides a description of the potential security issue.
- GuardDuty now uses AI to conduct "pre-crime" identification of bad actors 7-10 days in advance of malware release

## Amazon Detective
- Streamlines the investigative process and assists security teams in performing rapid and efficient **eDiscovery** initiaitives
- Customers can quickly analyze and dtermine the nature and extent of possible security issues with Amazon Detective prebuilt data aggregations, summaries, and context
- Detective automatically gathers log data from AWS resources and uses machien learning (ML), statistical analysis, and graphy theory to generate a linked dataset to drive more efficient security inquiries

## Amazon Macie
- Is a data security service that uses machine learning (ML) and pattern matching to discover and help protect the customer's sensitive data
- Discovers sensitive data and provides visibility into data security risks, allowing automated protection
- It is also a common service to deploy behind an API gateway with serverless technologies

## AWS Security Blog
- Features regular posts by AWS experts and other industry professionals
- Excellent research and information-gathering source for all things AWS
- Customers can search based on various categories, topics, keywords, products, solutions, industries, and even learning levels

## AWS Key Management Service (AWS KMS)
- lets customers create, manage, and control cryptograhpic keys across most applications and services
- can encrypt data across AWS workloads, digitally sign data, encrypt within applications using the AWS Encryption SDK, and generate and verify message authentication codes (MACs)
- The customer managed keys (CMKs) never leave the AWS FIPS 140-validated HSMs unencrypted
- Customers have complete control over permissions, administration, and usage across AWS services

## AWS CloudFormation
- AWS CloudFormation empowers customers to model, deploy, and manage AWS and third-party resources by handling **infrastructure as code**, is a cloud template language
- The cloud template language comes in either JSON or YAML formats
- Customers can automate, test, and deploy infrastructure templates with continous integration and delivery (CI/CD) automations

## AWS Batch
- lets developeers, scientists, and engineers powerfully run batch jobs
- Customers can analyze:
    - Financial services
    - Life sciences
    - Digital media
- **Exam**: AWS Batch for running hundereds of thousands of batch and machine learning compouting jobs without installing software or servers

## Reserved Instance Behavior and Flexibility
- Amazon EC2 Reserved Instances (RIs) offer a substantial discount (up to 72%) when compared to On-Demand pricing
- RIs can deliver a capacity reservation, offering extra confidence in the ability to launch the number of instances reserved when needed
- Customers have the flexibility to change families, OS types, and tenancies while benefitting from RI pricing when they use **Convertible RIs**

## Amazon EC2 RI Instance Types
- **Standard RIs** provide the most significant discount (up to 72% off On-Demand) for regular usage
- **Convertible RIs** provide a discount (up to 54% off On-Demand) and the capability to change the attributes of the RI if the exchange leads to the creation of Reserved Instances of equl or greater value
- **Scheduled RIs** are available to launch within the time windows you reserve

## Spot Instances
- EC2 Spot Instances leverage unused EC2 capacity in the AWS cloud
- They are available at up to a 90% discount compared to On-Demand prices
- Spot Instances for various stateless, fault-tolerant, or flexible applications such as big data, containerized workloads, CI/CD, web servers, high-performance computing (HPC), and test & development workloads

## Savings Plan
- provides low prices in exchange for commitment and the commitment cannot be changed after purchase
- **Compute** Savings Plans offer the most flexibility and prices that are up to 66 percent off On-Demand rates
- **EC2 Instance** Savings Plans provide savings up to 72% off On-Demand
- **SageMaker** Savings Plans provide savings up to 64% off On-Demand rates

## Dedicated Hosts and Instances
- An important difference between a Dedicated Host and a Dedicated instance is that a Dedicated Host gives the customer additional visibility and control over how instances are placed on a physical server
- Customers can consistently deploy their instances to the same physcial server over time

## AWS Placement Groups
- is a configuration option that AWS offers taht lets customers house a sgroup of interdependent EC2 instances in a certain way across the underlying hardware on which those instances reside
- The instances could be placed close together, spread through different racks, or spread through different AZs

## Containers
- In AWS, customers can also build and run containerized applications
- Is a discrete environment within an operating system where one or more applications can run that is typicaly assigned all the resources and dependencies needed to function
- It is a modular and portable environment that included the application binaries, software dependencies, and hardware rfequirements wrapped up into an independent, self-contained unit

## Microservices
- Microservices are specific service-oriented application components made up of small independent services taht communicate over well-defined APIs for notification and process queueing
- Microservices make applications and apps faster to develop and easier to scale by small, self-contained teams of developers
    - Microservices are about the design of software
    - Containers are about packaging software for deployment

## Lightsail
- **websites** allows companies to build small business applications such as file storage and sharing, backups, financial and accounting software, and more
- Customers can build a website in just a few clicks, with pre-configured applications like WordPress, Magento, Prestashop, and Joomla
- Some customers can easily create and delete development sandboxes and test environments risk free

## Elastic Beanstalk
- is an AWS service for deploying and scaling **web applications** and services
- customers can upload their code and let Elastic Beanstalk automatically handle the deployment
- does everything from capacity provisioning, load balancing, and auto scaling to application health monitoring

## Elastic Container Registry (Amzaon ECR)
- is a fully managed container registry offering high-performance hosting
- Customers can dependably deploy application images and artifcacts anywhere
- Developers can manage software vulenrabilities, streamline deployment workloads, and manage image lifecycle policies

## Elastic Kubernetes Service (Amazon EKS)
- Amazon EKS is a managed Kubernetes service taht makes it easy to run Kubernetes on AWS and on-premises
- Automatically manages the availability and scalabilityy of the Kubernetes control plane nodes responsible for scheduling containers, managing application availability, storing cluster data, and more
- EKS offers all the performance, scalability, reliability, and availability of the AWS infrastructure

## AWS Fargate
- serverless, pay-as-you-go compute engine that lets customers construct applications without servers
- is attuned with Elastice Container Service (ECS) and Amazon Elastic Kubernetes Service (EKS)
- tasks include choosing an Open Container Initiative (OCI)-compliant container image, defining memory and compute resources, and running the container with serverless compute
- Multiple CPU architectures and operating systems are supported

## AWS Lambda
- **function**, is a serverless, eent-driven compute service taht enables customers to run code for practically any application or backend service without deploying or managing servers
- Customers can trigger Lambda from over 200 AWS services and Software as a Service (SaaS) applications
- It uses the pay-as-you-go model

## Auto Scaling Services
- AWS Auto Scaling montors client applications and routinely regulates cpacity to maintain stable, predictable performance at the lowest probable cost
- simple to setu up application scaling for multiple resources across multiple services in a matter of minutes
- offers an efficient graphjical user interface to construc scaling plans and launch templates for resources, includeing EC2 instances, Spot Fleets, ECS tasks, DynamoDB tables, indexes, and even Amazon Aurora (RDS) Replicas

## Auto Scaling
- makes scaling easy with common suggestions that let customers optimize perfomance, costs, or balance between them
- Customers often combine existing EC@ instances with AWS Auto Scaling to **scale out** extra resources for other AWS services
- Applications always have the proper resources at the right time with AWS
- **use with CloudWatch**

## Block Storage
- Three types of storage:
    - Object
    - File
    - Block
- Block storage is a classic technology that manages data storage and storage devices
- it takes any data, like a file or database entry, and distributes it into equal size blocks (512-bit is legacy, 4K is common)
- stores the data block on supporting physical storage in a manner that is optimized for fast access and retrieval (RAID arrays)
- Developers prefer block storage for applications that require efficient, fast, and reliable data access
- Block storage offers a more direct pipeline to the data
- By comparison, file storage has an extra layer consisting of a file system (NFS, SMB, CIFS) fo process before accessing the data
- **Use Cases**
    - Storage Area networks
    - Containerized applications
    - Transactional workloads
    - Analytics and data warehousing
    - Virtual Machines

## Object Storage
- is a technology that stores and controls data in an unstructured format called objects
- Modern enterprises generate and analyze large amounts of unsturctured data sucah as photos, graphics, audio, files, videos, email, web pages, and sensor data.
- This solution creates a flat structure instead of a hierarchical or tiered storage.

## Object Storage Use Cases
- **Cloud-native applications** - use technologies like containerization and serverless to address customer needs in a rapid and flexible way
- **Machine Learning (ML)** - requires object storage because of the scale and cost efficiency to "teach" a computer system to make predictions or inferences
- **Backup and recovery** - deploy object storage systems to duplicate content in case a physical device fails.

## Elastic File System (EFS)
- offers a simple, scalable, elastic file system for workloads using AWS Cloud services and on-premises resources
- automatically grows and shrinks as files are added or removed with no need for management or provisioning
- is built to scale on demand to petabytes without disrupting applications, growing and shrinking automatically as you add and remove files
- it is a fully managed service that requires no changes to existing applications and tools

## FSx
- makes it easy and cost effective to launch, run, and scale reature-rich, high-performance file systems in the cloud supporting a wide range of workloads with its reliability, security, scalability, and broad set of capabilities
- is built on the latest AWS compute, networking, and disk technologies to provide high performance and lower TCO
- Customers can choose between four widely-use file systems: NetApp ONTAP, OpenZFS, Windows File Server, and Lustre

## AWS Storage Gateway
- is a hybrid storage service taht enables your on-premises applications to seamlessly use AWS cloud storage
- You can use the service for backup and archiving, disaster recovery, cloud data processing, storage tiering, and migration
- Can be appliance-based or in a hypervisor
- Often used in conjunction with AWS Direct Connect 10 or 100 Gbps connections

## Relational Databases
- A database transaction is one or more "all-or-nothing" SQL statements that are performed as a serfies of operations that establish a single logicl unit of work
- Data integrity is the genreal fullness, accuracy, and consistency of data
- Relational databases use a set of constrains called keys to enforce data integrity in the database
- To ensure data integrity, all database transactions must be ACID compliant: Atomic, Consistent, Isolated and Durable

## NoSQL Databases
- Purpose built for designated data models
- Have elastic schemas for constructing modern applications
- Commonly known for their simplicity of development, functionality, and scalable performance
- use a diversity of data models
- database types are optimized explicitly for applications that demand large data volumn, low latency, and flexible data models
- This is accomplished by bypassing some of the data consistency restrictions of other databases, such as the relational type.

## Amazon DynamoDB
- Is a fast, malleable NoSQL database service for single-digit millisecond performance at any scale
- Is a fully managed, serverless, key-value NoSQL database designed to run high-performance applications
- Delivers built-in security, nonstop backups, automated multi-Region replication, in-memory caching, and powerful data import and export tools
- **Exam: they refer to DynamoDB as a "non-relational" database**

## Memory-based Databases
- In-memory databases are purpose-built databases that typically depend on high-speed memory chip clusters for data storage, as opposed to databases that store data on disk or solid-state drives (SSDs)
- In-memory data storage is intended to allow for nominal response times by abolishing the need to access physical disks

## Amazon ElastiCache for Redis
- is an extremely fast in-memory data store taht provides sub-millisecond latency to enable internet-scale real-time applications
- is constructed on open source Redis and compatible with the Redis APIs
- self-managed Redis applications can function effortlessly with Redis ElastiCache without any code changes
- joins the speed, ease, and flexibility of open-source Redis with manageability, security, and scalability from AWS

## Appropriate Migration Strategies: Database Replication
- refers to the process of copuying data from a primary database to one or more replica databases to improve data availability and system fault-tolerance and reliability
- DB replication is usually a continual process occurring in real-time as data is created, modified, or deleted in the primary database
    - It can also occur as one-time or scheduled batch projects

## Database Replication Use Cases
- **Customers can create tasks for ongoing replication using AWS Database Migration Service (DMS)**
- Data can be migrated to S3 storage to match the organizational data life cycle
- A newer solution would be to use Amazon Elastic File System (EFS) replication to create a replica of their EFS file system in the Aws Region of their choosing
- AWS customers may decide to innovate and build new database applications with Amazon Relational Database Service (RDS)

## Data Lifecycle Policies
- Customers can formulate a data lifecycle initiative for several areas:
    - Block storage using levels of SSD/HDD
    - Object storage using S3 storage tiers
    - S3 Glacier archiving retrieval plans
    - Manage EBS snapshots and EBS-backed Amazon Machine Images (AMIs)
    - Moving data to AWS with AWS Snow services
    - Supporting enterprise backup and restore policies
    - Enabling cloud disaster recovery 
    - Database replication plans

## Amazon EMR (Formerly Amazon Elastic MapReduce)
- is the industry-leading cloud big data solution for petabyte-scale data processing, interactive analytics, and machine learning
- utilizes open-source frameworks such as Apache Spark, Apache Hive, and Presto
- **Amazon EMR Serverless is a new option in EMR**
    - It makes it sim ple and cost-effective for engineers and analysts to run applications built using open-source big data frameworks like Apache Spark, Hive, or Presto
    - There is no need to tune, operate, optimize, secure, or manage clusters

## Amazon EventBridge
- is a serverless event bus to assist customers in constructing event-driven or SaaS applications at scale
- The event bus delivers streams of real-time data from event sources such as Shopify to targets like AWS Lambda and other SaaS applications
- Customers can accelerate modernizing and re-orchestrating their architecture with decoupled services and applications
- Leverage AWS Artificial Intelligence/Machine Learning services and get valuable insights

## Amazon Simple Notification Service (Amazon SNS)
- Amazon SNS sends notifications two ways:
    - Application-to-Application (A2A)
    - Application to Person (A2P)
- A2A offers high-throughput, push-based, many-to-many messaging between distributed systems, microservices, and event-driven serverless applications
    - **Exam: Call SNS notifications with AWS Step Functions**
- A2P functionality lets you send messages to customers with SMS, push notifications, and email

## Amazon Simple 