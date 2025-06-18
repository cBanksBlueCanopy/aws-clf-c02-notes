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



