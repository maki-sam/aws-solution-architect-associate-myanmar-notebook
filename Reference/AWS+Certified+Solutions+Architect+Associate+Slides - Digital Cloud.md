

© Digital Cloud Training| https://digitalcloud.training
## SECTION 1
## Let's Get Started!

© Digital Cloud Training| https://digitalcloud.training
The SAA-C03 Exam

© Digital Cloud Training| https://digitalcloud.training
The SAA-C03 Exam
## Level: Associate
Length: 130 minutes
Format: 65 questions
Cost: $150 USD
Delivery Method: Testing center or online
## Scoring:
•Scaled score between 100 –1000
•Minimum passing score of 720

© Digital Cloud Training| https://digitalcloud.training
The SAA-C03 Exam
Question format:
•Multiple-choice:Has one correct response and three
incorrect responses
•Multiple-response:Has two or more correct responses
out of five or more options

© Digital Cloud Training| https://digitalcloud.training
The SAA-C03 Exam
## Domain 1: Design Secure Architectures
•Task Statement 1.1: Design secure access to AWS resources
•Task Statement 1.2: Design secure workloads and applications
•Task Statement 1.3: Determine appropriate data security controls
## Domain 2: Design Resilient Architectures
•Task Statement 2.1: Design scalable and loosely coupled architectures
•Task Statement 2.2: Design highly available and/or fault-tolerant architectures

© Digital Cloud Training| https://digitalcloud.training
The SAA-C03 Exam
Domain 3: Design High-Performing Architectures
•Task Statement 3.1: Determine high-performing and/or scalable storage solutions
•Task Statement 3.2: Design high-performing and elastic compute solutions
•Task Statement 3.3: Determine high-performing database solutions
•Task Statement 3.4:Determine high-performing and/or scalable network architectures
•Task Statement 3.5: Determine high-performing data ingestion and transformation
solutions

© Digital Cloud Training| https://digitalcloud.training
The SAA-C03 Exam
Domain 4: Design Cost-Optimized Architectures
•Task Statement 4.1: Design cost-optimized storage solutions
•Task Statement 4.2: Design cost-optimized compute solutions
•Task Statement 4.3: Design cost-optimized database solutions
•Task Statement 4.4: Design cost-optimized network architectures

© Digital Cloud Training| https://digitalcloud.training
AWS Account Overview

© Digital Cloud Training| https://digitalcloud.training
AWS Account Overview
AWS Account
## Account Root User
## AWS IAM
UserGroupRolePolicy
IAM can be used to create users,
groups, roles and policies
Unique email
address required
The Root user has full control
over the account
It’s an IAM best practice to create individual users
and to avoid using the Root account

© Digital Cloud Training | https://digitalcloud.training
AWS Account Overview
AWS Account
us-west-1
us-east-1ap-southeast-2
## AWS IAM
## EC2
## RDS
## S3ALB
## EC2
## RDS
## S3ALB
## EC2
## RDS
## S3ALB
AWS Management
## Console
Authentication: IAM principals
authenticate to IAM using the
console, API, or CLI
Authorization: IAM principals
can then create resources
across AWS Regions
All AWS identities and resources are created
within the AWS account

© Digital Cloud Training | https://digitalcloud.training
Create your AWS Account

© Digital Cloud Training | https://digitalcloud.training
Free Plan vs Paid Plan
Paid PlanFree Plan
SameReceive USD $100 sign up credit and earn up to $100
in additional credits
Access to Always free services and short-term trial
offers
Access to Always free services
Access to all AWS services and featuresAccess to select AWS services and features
Pay for charges that exceed the credit balanceNo charges incur during usage
No automatic expiration; account remains active
indefinitely
Account expires after 6 months or once credits are
used—whichever comes first
N/A—the account is already Paid PlanAfter expiration, you can upgrade to a Paid Plan
within a 90-day grace period (reopens the account)
Note: Free plan and free credits are available to new customers only

© Digital Cloud Training | https://digitalcloud.training
Free Plan vs Paid Plan - Links
https://aws.amazon.com/free/
https://aws.amazon.com/free/free-tier-faqs/
https://
docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/free-tier-plans.html

© Digital Cloud Training | https://digitalcloud.training
Important note on upgrading from Free to Paid
“If your account is converted from the Free account plan to the Paid
account plan through AWS Organizations, AWS Partner programs, or
other enterprise programs, any remaining Free Tier credits will
expire and will not be applied to your Paid account usage.”
•If you manually upgrade from the Free account plan to the Paid account
plan any remaining Free Tier credits carry over and are automatically
applied to your future AWS bills
•Free Tier Credits expire twelve months from the date you opened your
account. However, remember that free accounts are shut down after 6
months

© Digital Cloud Training | https://digitalcloud.training
Which plan should you choose?
Choose Free Plan if:
•You’re worried about getting a
surprise bill
•You’re new to AWS and want to get
familiar before upgrading
•Short term uses, e.g. you’re just
doing a single course and don’t
need access to all services
Choose Paid Plan if:
•You’re more familiar with AWS and
confident with pricing and cost
controls
•You need access to services not
included in the free plan
•Longer term uses 6-months+
Best for: Beginners who want a
safe, time-limited way to explore
AWS without complex billing
Best for: Students building larger or
more varied projects, or needing
advanced services

© Digital Cloud Training | https://digitalcloud.training
What you need...
Credit card for setting up the account and
paying any bills
Unique email address for this account
Unique AWS account name / alias
john+ACCOUNT-ALIAS-1@gmail.com
john+ACCOUNT-ALIAS-2@gmail.com
john@gmail.com
Phone to receive an SMS verification code
Check if you can use a
dynamic alias with an
existing email address

© Digital Cloud Training | https://digitalcloud.training
Configure Account and
Create a Budget

© Digital Cloud Training | https://digitalcloud.training
## Account Configuration
•Configure Account Alias
•Enable access to billing for IAM users
•Update billing preferences
•Create a budget and alarm

© Digital Cloud Training | https://digitalcloud.training
Install Tools and
Configure AWS CLI

© Digital Cloud Training | https://digitalcloud.training
Install Tools and Configure AWS CLI
 Download the code (from the next lesson)
##  Install Visual Studio Code
 Install and Configure the AWS CLI
 Access AWS CloudShell

© Digital Cloud Training | https://digitalcloud.training
## SECTION 2
AWS Identity and Access Management
## (IAM)

© Digital Cloud Training | https://digitalcloud.training
AWS Identity and Access
Management (IAM)

© Digital Cloud Training | https://digitalcloud.training
AWS Identity and Access Management (IAM)
AWS Account
## Console
## CLI
## API
## AWS IAM
## Role
## User
## Federated
## User
## Application
## Identity-
based policy
## Resource-
based policy
## S3
## EC2
## IAM
RunInstances
GetBucket
CreateUser
IAM Principals must be authenticated to
send requests (with a few exceptions)
Actions are
authorized
on AWS
resources
A principalis a person or application that
can make a request for an action or
operation on an AWS resource
AWS determines whether
to authorize the request
## (allow/deny)

© Digital Cloud Training | https://digitalcloud.training
Users, User Groups, Roles and Policies
AWS Account
UserUser GroupsRolePolicy
## User Group
## User
The user gains the
permissions applied to the
group through the policy
Identity-based policies
can be applied to users,
groups, and roles
Roles are used for delegation
and are assumed
Policies define the permissions
for the identities or resources
they are associated with

© Digital Cloud Training | https://digitalcloud.training
IAM Users
## AWS IAM
## Account Root User
EthanAndreaEric
Friendly name:
## Andrea
## Amazon Resource Name:
arn:aws:iam::625148252389
:user/Andrea
The root user has full permissions.
It’s a best practice to avoid using
the root user account + enable MFA
Email used
for signup
Up to 5000 individual user
accounts can be created. Users
have no permissions by default
Authentication via username/password for
console or access keys for API/CLI

© Digital Cloud Training | https://digitalcloud.training
IAM User Groups
Admin GroupDevelopment GroupOperations Group
EthanAndreaEricSunilLee
User Groups are
collections of users
The main reason to use groups
is to apply permissions to
users using policies
The user gains the
permissions applied to the
group through the policy

© Digital Cloud Training | https://digitalcloud.training
IAM IAM Authentication Methods
AWS Management
## Console
## CLI
## API
## AWS IAM
## Username: John
## Password: Eo28720*!
MFA Token: (optional)
## John
Access key ID: AKIAXP4J2EKUQIQJTJLV
Secret access key:
wiMjGpewNMRHFi9ud0pJwh7NBX4F6i
## AWS IAM
## AWS API
John is authenticated and
can perform operations in
the console
Access keys are used for
programmatic access

© Digital Cloud Training | https://digitalcloud.training
Root User vs IAM User
## User
## Login Details
## Permissions
IAM User
## Root User
Email address
Friendly name: John
## +
AWS account ID or Alias
IAM Permissions
## Policy
## Full - Unrestricted

© Digital Cloud Training | https://digitalcloud.training
Creating IAM Users
and Groups

© Digital Cloud Training | https://digitalcloud.training
IAM Authentication and MFA

© Digital Cloud Training | https://digitalcloud.training
IAM IAM Authentication Methods
AWS Management
## Console
## CLI
## API
## AWS IAM
## Username: John
## Password: Eo28720*!
MFA Token: (optional)
## John
Access key ID: AKIAXP4J2EKUQIQJTJLV
Secret access key:
wiMjGpewNMRHFi9ud0pJwh7NBX4F6i
## AWS IAM
## AWS API
John is authenticated and can
perform operations in the console
Access keys are used for
programmatic access

© Digital Cloud Training | https://digitalcloud.training
Multi-Factor Authentication
Something you know:
EJPx!*21p9%
## Password
Something you have:Something you are:

© Digital Cloud Training | https://digitalcloud.training
Multi-Factor Authentication
Something you know:
EJPx!*21p9%
## Password
Something you have:
IAM User
Virtual MFA
Hardware device
e.g. Google Authenticator on
your smart phone
Security keys and time-based
one-time password (TOTP)
tokens

© Digital Cloud Training | https://digitalcloud.training
Setup Multi-Factor
Authentication (MFA)

© Digital Cloud Training | https://digitalcloud.training
## Permissions Boundaries

© Digital Cloud Training | https://digitalcloud.training
## Permissions Boundaries
## Joanne
## Developers
## Permissions
## Boundary
## IAM
## Amazon S3
S3:ListBuckets
iam:CreateUser
Policy allows full control of S3,
CloudWatch, EC2, and IAM
## Permissions
boundaries are
attached to users
and roles
The permissions boundary sets
the maximum permissions that
the entity can have
The operation fails because
the permissions boundary
does not allow it

© Digital Cloud Training | https://digitalcloud.training
## Privilege Escalation
## Lindsay
IAMFullAccess
## IAM
iam:CreateUser
X-User
AdministratorAccess
AWS Batch
Lindsay is assigned permissions
to AWS IAM only and cannot
launch AWS resources
Lindsay applies the
AdministratorAccess
policy to the X-User account
Lindsay mines bitcoins
Lindsay is now able to login with the
X-User account and gain full
privileges to the AWS account

© Digital Cloud Training | https://digitalcloud.training
## Preventing Privilege Escalation
## Lindsay
IAMFullAccess
## IAM
iam:CreateUser
X-User
AdministratorAccess
## Permissions
## Boundary
Lindsay is assigned permissions
to AWS IAM only and cannot
launch AWS resources
Lindsay applies the
AdministratorAccess
policy to the X-User account
The permissions boundary
ensures that users created by
Lindsay have the same or
fewer permissions
Lindsay does not have more privileges
when logging in as X-User and cannot
launch AWS resources

© Digital Cloud Training | https://digitalcloud.training
IAM Policy Evaluation

© Digital Cloud Training | https://digitalcloud.training
## Evaluation Logic

© Digital Cloud Training | https://digitalcloud.training
Steps for Authorizing Requests to AWS
## Console
## CLI
## API
## AWS IAM
Request context:
•Actions – the actions or operations the
principal wants to perform
•Resources – The AWS resource object upon
which actions are performed
•Principal – The user, role, federated user, or
application that sent the request
•Environment data – Information about the
IP address, user agent, SSL status, or time of
day
•Resource data – Data related to the
resource that is being requested
Identity-based policy
## Resource-
based policy
s3:GetObject
## User
## S3 Bucket
- Authentication – AWS
authenticates the principal
that makes the request
- Processing the request context
- Evaluating all policies
within the account
- Determining whether a
request is allowed or denied

© Digital Cloud Training | https://digitalcloud.training
Types of Policy
•Identity-based policies –   attached to users, groups, or roles
•Resource-based policies –   attached to a resource; define
permissions for a principal accessing the resource
•IAM permissions boundaries –   set the maximum
permissions an identity-based policy can grant an IAM entity
•AWS Organizations service control policies (SCP) –   specify
the maximum permissions for an organization or OU
•Session policies –   used with AssumeRole* API actions

© Digital Cloud Training | https://digitalcloud.training
Evaluating Policies within an AWS Account
## Identity-based
policy
## Resource-based
policy
## Effective
permissions
## Identity-based
policy
## Permisions
boundary
## Effective
permissions
## Identity-based
policy
## Organizations
## SCP
## Effective
permissions

© Digital Cloud Training | https://digitalcloud.training
## Determination Rules
1.By default, all requests are implicitly denied (though the
root user has full access)
2.An explicit allow in an identity-based or resource-based
policy overrides this default
3.If a permissions boundary, Organizations SCP, or session
policy is present, it might override the allow with an
implicit deny
4.An explicit deny in any policy overrides any allows

© Digital Cloud Training | https://digitalcloud.training
IAM Policy Structure

© Digital Cloud Training | https://digitalcloud.training
API Actions
Each AWS service has its own set of actions that
describe tasks you can perform with that service
Amazon EC2
" "Action": "ec2:RunInstances"
## AWS IAM
""Action": "iam:ChangePassword"
## Amazon S3
""Action": "s3:GetObject"
Amazon RDS
""Action": "rds:StopDBInstance"

© Digital Cloud Training | https://digitalcloud.training
Reading IAM Policies
All properties in a
single statement
block are evaluated
together
A policy may
contain more than
one permission
statement

© Digital Cloud Training | https://digitalcloud.training
Reading IAM Policies
The effect is either allow or deny
Action lists the specific
resource operations that
the policy affects
Resource lists the specific resources that the
policy applies to
A * is a wildcard

© Digital Cloud Training | https://digitalcloud.training
## Permission Statements - Conditions
Conditions allow for context-
based decisions. In this
example, access is allowed
Mon-Fri during business hours

© Digital Cloud Training | https://digitalcloud.training
IAM Policy Example – Source IP Address Condition
The specific API action is defined
The effect is to deny the API action if the
IP address is not in the specified range

© Digital Cloud Training | https://digitalcloud.training
IAM Policy Example – Encryption Condition
You can tell this is a resource-based policy
as it has a principal element defined
The policy grants read and write
access to an EFS file systems to all
IAM principals ("AWS ": "*")
the policy condition element
requires that SSL/TLS
encryption is used

© Digital Cloud Training | https://digitalcloud.training
IAM Policy Example – Prefix Condition
A variable is used for the s3:prefix that is
replaced with the user’s friendly name
The actions are allowed only within the
user’s folder within the bucket

© Digital Cloud Training | https://digitalcloud.training
## Access Evaluation Tools

© Digital Cloud Training | https://digitalcloud.training
IAM Best Practices

© Digital Cloud Training | https://digitalcloud.training
AWS IAM Best Practices
•Require human users to use federation with an identity provider to
access AWS using temporary credentials
•Require workloads to use temporary credentials with IAM roles to
access AWS
•Require multi-factor authentication (MFA)
•Rotate access keys regularly for use cases that require long-term
credentials
•Safeguard your root user credentials and don't use them for everyday
tasks
•Apply least-privilege permissions
•Get started with AWS managed policies and move toward least-
privilege permissions

© Digital Cloud Training | https://digitalcloud.training
AWS IAM Best Practices
•Use IAM Access Analyzer to generate least-privilege policies based on
access activity
•Regularly review and remove unused users, roles, permissions,
policies, and credentials
•Use conditions in IAM policies to further restrict access
•Verify public and cross-account access to resources with IAM Access
## Analyzer
•Use IAM Access Analyzer to validate your IAM policies to ensure
secure and functional permissions
•Establish permissions guardrails across multiple accounts
•Use permissions boundaries to delegate permissions management
within an account

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns –
## AWS IAM

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – AWS IAM
A select group of users only should be
allowed to change their IAM passwords
Create a group for the users and apply a
permissions policy that grants the
iam:ChangePassword API permission
An Amazon EC2 instance must be
delegated with permissions to an
Amazon DynamoDB table
Create a role and assign a permissions
policy to the role that grants access to
the database service
A company has created their first AWS
account. They need to assign
permissions to users based on job
function
Use AWS managed policies that are
aligned with common job functions
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – AWS IAM
A solutions architect needs to restrict
access to an AWS service based on the
source IP address of the requester
Create an IAM permissions policy and
use the Condition element to control
access based on source IP address
A developer needs to make
programmatic API calls from the AWS
## CLI
Instruct the developer to create a set of
access keys and use those for
programmatic access
A group of users require full access to
all Amazon EC2 API actions
Create a permissions policy that uses a
wildcard for the Action element relating
to EC2 (ec2:*)
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## SECTION 3
Amazon Elastic Compute Cloud (EC2)

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Overview

© Digital Cloud Training | https://digitalcloud.training
Amazon Elastic Compute Cloud (EC2)
EC2 instances are virtual servers
running in the AWS data centers
EC2 instances can run Windows or
Linux + a MacOS option on
dedicated hardware
EC2 instances are attached to the
network via an Elastic Network
Interface (ENI)
Private subnetPublic subnet
EC2 instances are launched in public
or private subnets within an Amazon
Virtual Private Cloud (VPC)
Amazon Elastic Block Store (EBS)
volumes are attached to EC2
instances for persistent storage

© Digital Cloud Training | https://digitalcloud.training
Amazon Elastic Compute Cloud (EC2)
Windows OS
## Website
Many instances run
on each host server
EC2 InstanceEC2 InstanceEC2 Instance
EC2 InstanceEC2 InstanceEC2 Instance
EC2 InstanceEC2 InstanceEC2 Instance
EC2 hosts are
managed by AWS
An EC2 instance is a virtual server
and is managed by the customer
A selection of instance types
come with varying combinations
of CPU, memory, storage and
networking
Amazon EC2 runs on servers
in AWS data centers

© Digital Cloud Training | https://digitalcloud.training
Flexible and On-Demand
Instances can be
stopped when not
needed
And then started
again
Or they can be
terminated

© Digital Cloud Training | https://digitalcloud.training
EC2 Instance Families & Types
•Instance families provide varying
combinations of hardware
resources
•Optimized for different compute
workloads
•Larger sizes provide greater
hardware capability
## General Purpose
## Compute Optimized
## Accelerated Computing
## Storage Optimized
## Memory Optimized

© Digital Cloud Training | https://digitalcloud.training
large
EC2 Instance Families & Types
## General Purpose
## Compute Optimized
## Accelerated Computing
## Storage Optimized
## Memory Optimized
m is the family name
5   Is the generation number
large is the size of the instance
## 5
m
## .

© Digital Cloud Training | https://digitalcloud.training
EC2 Instance Families & Types
t2.micro
1 vCPU
1 GiB Memory
0.0116 USD/hr
c3.xlarge
4 vCPUs
7.5 GiB Memory
0.21 USD/hr
m4.16xlarge
64 vCPUs
256 GiB Memory
3.2 USD/hr
*prices are for relative comparison and may not be accurate

© Digital Cloud Training | https://digitalcloud.training
Elastic Network Interfaces (ENIs)
## Availability Zone
## Availability Zone
Private subnet
Public subnet
Private subnet
Public subnet
Virtual private cloud (VPC)
eth0
Instances in private subnets
only have private IP addresses
eth0
## 10.0.1.23
## 10.0.0.12
## 52.63.195.113
Instances in public subnets may
have a private IP and a public IP
eth0
eth1
Additional ENIs can be attached
from subnets within the same AZ

© Digital Cloud Training | https://digitalcloud.training
Public, Private, and Elastic IP addresses
TypeDescription
Public IP addressReleased when the instance is stopped
Used in Public Subnets
## Chargeable
Associated with a private IP address on the instance
Cannot be moved between instances
Private IP addressRetained when the instance is stopped
Used in Public and Private Subnets
Elastic IP addressStatic Public IP address
## Chargeable
Associated with a private IP address on the instance
Can be moved between instances and Elastic Network Adapters

© Digital Cloud Training | https://digitalcloud.training
Network Interfaces (ENI, ENA, EFA)
Elastic network
interface
Elastic network
adapter
## Elastic Fabric
## Adapter
•Basic adapter type for when you
don’t have any high-performance
requirements
•Can use with all instance types
•Enhanced networking
performance
•Higher bandwidth and lower
inter-instance latency
•Must choose supported instance
type
•Use with High Performance
Computing and MPI and ML use
cases
•Tightly coupled applications
•Can use with all instance types

© Digital Cloud Training | https://digitalcloud.training
Amazon Elastic Block Store (EBS)
EC2 Instance
## Availability Zone
EBS Volume
EBS Volume
## C:D:
The volume is
attached over a
network
EBS volumes
exist within an
## Availability Zone
The volume is automatically
replicated within the AZ

© Digital Cloud Training | https://digitalcloud.training
Amazon EBS Volume Types
Volume TypeDurabilityVolume Size
(Min/Max)
Max IOPS (per
volume)
## Max Throughput
(per volume)
Multi-Attach
## Support
gp3 (General
Purpose SSD)
99.8% - 99.9%1 GiB - 16 TiB16,0001,000 MB/sNo
gp2 (General
Purpose SSD)
99.8% - 99.9%1 GiB - 16 TiB16,000250 MB/sNo
io2 (Provisioned
## IOPS SSD)
99.999%4 GiB - 16 TiB256,0004,000 MB/sYe s
io1 (Provisioned
## IOPS SSD)
99.9% - 99.99%4 GiB - 16 TiB64,0001,000 MB/sYe s
st1 (Throughput
Optimized HDD)
99.8% - 99.9%125 GiB - 16 TiB500500 MB/sNo
sc1 (Cold HDD)99.8% - 99.9%125 GiB - 16 TiB250250 MB/s No
## Magnetic
## (standard)
99.8% - 99.9%1 GiB - 1 TiB40-20090 MB/sNo

© Digital Cloud Training | https://digitalcloud.training
Amazon EBS Volume Use Cases
•gp3 (General Purpose SSD) – Most workloads, including databases
and dev/test environments
•gp2 (General Purpose SSD) – Boot volumes, dev/test, general
workloads
•io2 (Provisioned IOPS SSD) – High-performance databases, critical
applications
•io1 (Provisioned IOPS SSD) – Databases requiring high IOPS
•st1 (Throughput Optimized HDD) – Streaming, big data, log
processing
•sc1 (Cold HDD) – Archival storage, infrequent access workloads
•Magnetic (standard) – Legacy workloads, small boot volumes

© Digital Cloud Training | https://digitalcloud.training
Amazon EBS vs Instance Store
## Availability Zone
EBS Volume
EC2 Host Server
EBS Volume
EBS volumes are attached
over the network
Instance Store volumes are physically
attached to the host and offer high -
performance
Instance Store volumes are
ephemeral (non-persistent)
EBS volumes
offer persistent
storage

© Digital Cloud Training | https://digitalcloud.training
Launching Amazon EC2
## Instances

© Digital Cloud Training | https://digitalcloud.training
Launching an EC2 Instance
LinuxMicrosoft
## Windows
EC2 Instance
EBS Snapshot
FamilyTypevCPUsMemory (GiB)
General purposet2.micro11
Compute optimizedc5n.large25.25
Memory optimizedr5ad.large216
Storage optimizedd2.xlarge430.5
GPU instancesg2.2xlarge815
Select an instance type
## Amazon Machine Image
## (AMI)
Customized AMI
The instance type
defines the hardware
profile (and cost)
An AMI defines
the configuration
of the instance
A snapshot is a point-in -
time backup of an instance
You can customize your
instance and create a
custom AMI

© Digital Cloud Training | https://digitalcloud.training
Connecting to
Amazon EC2

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 User Data
and Metadata

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Metadata
•Instance metadata is data about your EC2 instance
•Instance metadata is available
athttp://169.254.169.254/latest/meta-data
•Examples:

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Metadata
•Examples ctd.:

© Digital Cloud Training | https://digitalcloud.training
IMDSv1 vs IMDSv2
Instance Metadata Service (IMDS)
comes in two versions:
•IMDSv1 – is older and less
secure
•IMDSv2 – is newer, more
secure, and requires a session
token for authorization
•Default EC2 launch settings may
disable IMDSv1

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 User Data
AWS Management Console
The code is run when
the instance starts for
the first time
## Web Server
Batch and PowerShell
scripts can be run on
## Windows

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 User Data via the AWS CLI
The user data is supplied by
specifying the file
aws ec2 run-instances --instance-type t2.micro --image-id
ami-   0440d3b780d96b29d --user-data file://user_data.sh

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 User Data
•User data must be base64-encoded
•Encoding is automatic with the console and
## AWS CLI
•User data is limited to 16 KB, in raw form,
before it is base64-encoded
•User data only runs the first time you launch
your instance

© Digital Cloud Training | https://digitalcloud.training
Using User Data and
## Metadata

© Digital Cloud Training | https://digitalcloud.training
Access Keys and IAM Roles
with EC2

© Digital Cloud Training | https://digitalcloud.training
Using Access Keys with Amazon EC2
## VPC
## Availability Zone
Private subnet
Public subnet
EC2 Instance
AWS Cloud
AWS CLI configured
with access keys
## Policy
## S3 Bucket
IAM User
The access key is
associated with an
IAM account
The access key will use the
permissions assigned to the IAM user

© Digital Cloud Training | https://digitalcloud.training
Using Access Keys with Amazon EC2
## VPC
## Availability Zone
Private subnet
Public subnet
EC2 Instance
AWS Cloud
## Policy
## S3 Bucket
IAM Role
Credentials are not
stored on the instance
The role is assumed
by the EC2 instance

© Digital Cloud Training | https://digitalcloud.training
Practice with Access Keys and
IAM Roles

© Digital Cloud Training | https://digitalcloud.training
EC2 Placement Groups

© Digital Cloud Training | https://digitalcloud.training
## Cluster Placement Groups
•Packs instances close together for low latency
•Gives very high network throughput
•Best for ENA/EFA and HPC or ML clusters
•Works best when all instances are launched at the
same time

© Digital Cloud Training | https://digitalcloud.training
## Cluster Placement Groups
## VPC
## Availability Zone
Uses enhanced networking, low network latency
and high throughput for inter-instance traffic
## Subnet
EC2 Instances
## Cluster Placement Group
Instances can be in multiple subnets but they
must be within the same availability zone

© Digital Cloud Training | https://digitalcloud.training
## Partition Placement Groups
•Splits instances into partitions to keep them on
separate hardware
•Reduces the risk of failure across the whole group
•Good for large, spread-out workloads like Hadoop,
HDFS, and Cassandra
•You control how many partitions you want to use

© Digital Cloud Training | https://digitalcloud.training
## Partition Placement Groups
## VPC
## Availability Zone
EC2 Instances
## Partition 1
EC2 Instances
## Partition 2
## Availability Zone
EC2 Instances
## Partition 3
Each partition is located on a separate AWS rack
Partitions can be in
multiple AZs
(up to 7 per AZ)
SubnetSubnet

© Digital Cloud Training | https://digitalcloud.training
## Spread Placement Groups
•Places each instance on separate hardware
•Gives the highest failure isolation
•Best for small numbers of critical instances
•Max of 7 instances per AZ

© Digital Cloud Training | https://digitalcloud.training
## Spread Placement Groups
## VPC
Availability ZoneAvailability Zone
Each instance is located on a
separate AWS rack
SubnetSubnet

© Digital Cloud Training | https://digitalcloud.training
AWS Placement Group Comparison
AttributeClusterPartitionSpread
GoalLowest latency, high
throughput
Isolate groups of instancesMaximize instance isolation
AZ ScopeSingle AZMulti-AZ allowedMulti-AZ allowed
Subnet UseMultiple subnets in same
## AZ
Multiple subnetsMultiple subnets
Hardware IsolationLowMedium (per-partition
isolation)
Highest (one instance per
rack)
Typical Use Case HPC, big data, high-speed
apps
Large distributed systems
(HDFS, Cassandra)
Critical workloads that must
not fail together
Instance LimitsNo special limitUp to 7 partitions per AZ7 instances per AZ
Risk of correlated failureHigherLowerLowest

© Digital Cloud Training | https://digitalcloud.training
EC2 Placement Group Use Cases
Tightly-coupled application that
requires low-latency, high
throughput network traffic
between instances
## Partition
## Spread
## Cluster
Distributed and replicated
NoSQL database; requires
separate hardware for node
groups
Small number of critical
instances that should be kept
separate from each other

© Digital Cloud Training | https://digitalcloud.training
## Network Interfaces
## (ENI, ENA, EFA)

© Digital Cloud Training | https://digitalcloud.training
Public subnet
EC2 Network Interfaces
eth0
Private subnet
eth1
## Availability Zone
EC2 Instance
## Availability Zone
Public subnetPrivate subnet
## 172.31.15.89
## 52.63.195.113
Additional ENIs can be attached
from subnets within the same AZ
Yo u   cannot attach ENIs from
subnets in different AZs
The primary network interface has a
private IP and optionally a public IP

© Digital Cloud Training | https://digitalcloud.training
EC2 Network Interfaces
Elastic network
interface (ENI)
Elastic network
adapter (ENA)
## Elastic Fabric
Adapter (EFA)
•Basic adapter type for when you
don’t have any high-performance
requirements
•Can use with all instance types
•Enhanced networking
performance
•Higher bandwidth and lower
inter-instance latency
•Must choose supported instance
type
•Use with High Performance
Computing and MPI and ML use
cases
•Tightly coupled applications
•Must choose supported instance
type

© Digital Cloud Training | https://digitalcloud.training
Elastic Network Interface (ENI)
Key points:
•Basic network interface every EC2 instance can use
•Supports multiple private IPs, secondary ENIs, and
security groups
•You can attach/detach it from instances (depending
on instance type)
•Works for general-purpose networking tasks
When to use:
•For normal EC2 networking—VPC communication,
standard Linux/Windows servers, NAT instances, etc.

© Digital Cloud Training | https://digitalcloud.training
Elastic Network Adapter (ENA)
Key points:
•Much higher bandwidth and lower latency than
standard ENI
•Supports up to 200 Gbps networking (depending on
instance family)
•Uses SR-IOV for direct access to hardware
•Needed for workloads that move a lot of data
When to use:
•High-throughput apps, databases, big data systems,
high-performance web servers, anything needing fast
packet processing

© Digital Cloud Training | https://digitalcloud.training
Elastic Fabric Adapter (EFA)
Key points:
•Delivers extremely low latency and high throughput
between instances
•Supports OS-bypass for faster communication
(important for MPI workloads)
•Allows tightly-coupled compute clusters to run like
on-prem HPC systems
When to use:
•Machine learning training clusters, high-performance
computing (HPC), simulations (weather, physics,
CFD), large-scale MPI workloads

© Digital Cloud Training | https://digitalcloud.training
Useful Facts about EC2 Networking
•Not every instance supports every adapter:
•ENI: Supported on all EC2 instances
•ENA: Used with most modern instance families (M5,
C5, R5, etc.)
•EFA: Only works on selected compute-heavy families
(C5n, P4d, Hpc6a, etc.)
•For ENA and EFA, placement groups help:
•Lower latency
•Higher throughput
•Better neighbor placement for HPC clusters
•Required for some EFA use cases

© Digital Cloud Training | https://digitalcloud.training
Useful Facts about EC2 Networking
•Jumbo frames support:
•Standard MTU = 1500 bytes
•Jumbo frames allows up to 9001 bytes
•ENI + ENA: support MTU 9001 (jumbo frames)
•EFA: supports jumbo frames for HPC and ML traffic
•EFA uses an extra interface:
•Your instance gets two interfaces
•ENI/ENA (normal traffic)
•EFA interface (HPC traffic only)

© Digital Cloud Training | https://digitalcloud.training
Useful Facts about EC2 Networking
•EFA is not for internet or cross-VPC traffic
•It only works for instance-to-instance inside the
same:
•Subnet
•Placement group
## •VPC
•EFA can skip parts of the Linux kernel network stack
to cut latency which is good for:
•ML training frameworks
•MPI workloads
•HPC codes

© Digital Cloud Training | https://digitalcloud.training
Useful Facts about EC2 Networking
•Instances can attach multiple ENIs, which helps
with:
•Splitting public and private traffic
•Using different security groups
•Building firewalls and NAT instances
•Multi-homed workloads
•Both ENA and EFA use Single Root I/O
Virtualization, meaning:
•Near-bare-metal network speeds
•Lower CPU load
•Less virtualization overhead

© Digital Cloud Training | https://digitalcloud.training
Public, Private and Elastic IP
## Addresses

© Digital Cloud Training | https://digitalcloud.training
Public subnet
Public, Private and Elastic IP Addresses
eth0eth1
## Availability Zone
EC2 Instance
## 172.31.15.89
## 52.63.195.113
## 172.31.55.108
Elastic IP
## 54.66.202.9
A public IP address is a
dynamic address
An Elastic IP address
is a static address
Virtual private cloud (VPC)

© Digital Cloud Training | https://digitalcloud.training
Public subnet
Public, Private and Elastic IP Addresses
eth0
eth1
## Availability Zone
EC2 Instance
## 172.31.15.89
## 52.63.195.113
## 172.31.55.108
## 54.66.202.9
EC2 Instance
eth0
Both ENIs and EIPs can be remapped to a different instance
Virtual private cloud (VPC)

© Digital Cloud Training | https://digitalcloud.training
Public subnet
Public, Private and Elastic IP Addresses
eth0
eth1
## Availability Zone
EC2 Instance
## 172.31.55.108
## 54.66.202.9
EC2 Instance
Public subnet
eth0
## Availability Zone
eth1
Virtual private cloud (VPC)

© Digital Cloud Training | https://digitalcloud.training
Public, Private and Elastic IP addresses
TypeDescription
Public IP addressReleased when the instance is stopped
Used in Public Subnets
## Chargeable
Associated with a private IP address on the instance
Cannot be moved between instances
Private IP addressRetained when the instance is stopped
Used in Public and Private Subnets
Elastic IP addressStatic Public IP address
## Chargeable
Associated with a private IP address on the instance
Can be moved between instances and Elastic Network Adapters

© Digital Cloud Training | https://digitalcloud.training
NAT for Public Addresses

© Digital Cloud Training | https://digitalcloud.training
NAT for Public Addresses
## Public / Elastic
## Internet
gateway
## Association
IGW performs
## 1:1 NAT
eth0
## 172.31.32.63
## 3.104.75.244
## Src: 54.23.86.101
## Dest: 172.31.32.63
## The Internet Gateway
performs N AT
## Src: 54.23.86.101
## Dest: 3.104.75.244
## Src: 172.31.32.63
## Dest: 54.23.86.101
## Src: 3.104.75.244
## Dest: 54.23.86.101

© Digital Cloud Training | https://digitalcloud.training
Working with ENIs and
IP Addresses

© Digital Cloud Training | https://digitalcloud.training
Private Subnets and
## Bastion Hosts

© Digital Cloud Training | https://digitalcloud.training
Private subnet
Private Subnets and Bastion Hosts
## Region
## VPC
## Availability Zone
Public subnet
## Internet
gateway
DestinationTa rget
172.31.0.0/16Local
## 0.0.0.0/0igw-id
## Public Subnet  Route Table
DestinationTa rget
172.31.0.0/16Local
## Private Subnet  Route Table
Private-IP
Private-IP
Public-IP

© Digital Cloud Training | https://digitalcloud.training
Private Subnets and
## Bastion Hosts

© Digital Cloud Training | https://digitalcloud.training
NAT Gateways and
NAT Instances

© Digital Cloud Training | https://digitalcloud.training
Private subnet
NAT Gateways
## VPC
Public subnet
## Internet
gateway
NAT Gateways deployment
requirements:
•Deployed in public subnets
•Have an Elastic IP attached
•Route to the NAT gateway
added to private subnet
## Web Service
What source addresses
does the web service see?
## 54.142.59.121
Elastic IP:
## Private Subnet Route Table
DestinationTa rget
10.0.0.0/16Local
## 0.0.0.0/0nat-gateway-id

© Digital Cloud Training | https://digitalcloud.training
Private subnet
NAT Instances
## VPC
Public subnet
## Internet
gateway
NAT Instance deployment
requirements:
•Deployed in public subnets
•Have an Elastic IP attached
•Route to the NAT instance
added to private subnet
•Uses a special AMI with the
string “amzn-ami-vpc-nat” in
the name
•Must disable
source/destination checks
## 54.142.59.121
Elastic IP:
## Private Subnet Route Table
DestinationTa rget
10.0.0.0/16Local
## 0.0.0.0/0nat-instance-id

© Digital Cloud Training | https://digitalcloud.training
NAT Instance vs NAT Gateway
NAT InstanceN AT   G a te way
Managed by you (e.g. software updates)Managed by AWS
Scale up (instance type) manually and use
enhanced networking
Elastic scalability up to 45 Gbps
No high availability – scripted/auto-scaled
HA possible using multiple NATs in multiple
subnets
Provides automatic high availability within an AZ
and can be placed in multiple AZs
Need to assign Security GroupNo Security Groups
Can use as a bastion hostCannot access through SSH
Use an Elastic IP address or a public IP
address with a NAT instance
Choose the Elastic IP address to associate with a
NAT gateway at creation
Can implement port forwarding through
manual customisation
Does not support port forwarding

© Digital Cloud Training | https://digitalcloud.training
NAT Gateway Connectivity Types
There are two connectivity types:
•Public (Default) – Instances in private subnets can connect to the
internet through a public NAT gateway
•Private – Instances in private subnets can connect to other VPCs
or your on-premises network through a private NAT gateway
•You can route traffic from the NAT gateway through a transit gateway or
a virtual private gateway
•You cannot associate an elastic IP address with a private NAT gateway
•You can attach an internet gateway to a VPC with a private NAT
gateway, but if you route traffic from the private NAT gateway to the
internet gateway, the internet gateway drops the traffic

© Digital Cloud Training | https://digitalcloud.training
High Availability for NAT Gateway
## VPC
Public subnet
## Internet
gateway
Private subnet
Public subnet
Private subnet
Public subnet
Private subnet
DestinationTa rget
10.0.0.0/16Local
## 0.0.0.0/0nat-gw-az1
AZ1 Private Route Table
DestinationTa rget
10.0.0.0/16Local
DestinationTa rget
10.0.0.0/16Local
## 0.0.0.0/0nat-gw-az2
AZ2 Private Route Table
DestinationTa rget
10.0.0.0/16Local
DestinationTa rget
10.0.0.0/16Local
## 0.0.0.0/0nat-gw-az3
AZ3 Private Route Table
DestinationTa rget
10.0.0.0/16Local
NAT gateways have redundancy within an AZ

© Digital Cloud Training | https://digitalcloud.training
Private Subnet with
NAT Gateway

© Digital Cloud Training | https://digitalcloud.training
EC2 Instance Lifecycle

© Digital Cloud Training | https://digitalcloud.training
EC2 Instance Lifecycle
pending
runningrebootingstoppingstopped
shutting-down
terminated
## Launch
## Reboot
## Stop
Stop-Hibernate
## Start
## Terminate
## AMI
TerminateRelevant to EBS-backed
volumes only

© Digital Cloud Training | https://digitalcloud.training
EC2 Instance Lifecycle
Stopping EC2 instances
•EBS backed instances only
•No charge for stopped instances
•EBS volumes remain attached (chargeable)
•Data in RAM is lost
•Instance is migrated to a different host
•Private IPv4 addresses and IPv6 addresses
retained; public IPv4 addresses released
•Associated Elastic IPs retained

© Digital Cloud Training | https://digitalcloud.training
EC2 Instance Lifecycle
Hibernating EC2 instances
•Applies to supported AMIs
•Contents of RAM saved to EBS volume
•Must be enabled for hibernation when launched
•Specific prerequisites apply
•When started (after hibernation):
•The EBS root volume is restored to its previous state
•The RAM contents are reloaded
•The processes that were previously running on the
instance are resumed
•Previously attached data volumes are reattached and the
instance retains its instance ID

© Digital Cloud Training | https://digitalcloud.training
EC2 Instance Lifecycle
Rebooting EC2 instances
•Equivalent to an OS reboot
•DNS name and all IPv4 and IPv6 addresses retained
•Does not affect billing
Retiring EC2 instances
•Instances may be retired if AWS detects irreparable
failure of the underlying hardware that hosts the
instance
•When an instance reaches its scheduled retirement
date, it is stopped or terminated by AWS

© Digital Cloud Training | https://digitalcloud.training
EC2 Instance Lifecycle
Terminating EC2 instances
•Means deleting the EC2 instance
•Cannot recover a terminated instance
•By default, root EBS volumes are deleted
Recovering EC2 instances
•CloudWatch can be used to monitor system status
checks and recover instance if needed
•Applies if the instance becomes impaired due to
underlying hardware / platform issues
•Recovered instance is identical to original instance

© Digital Cloud Training | https://digitalcloud.training
Nitro Instances and
## Nitro Enclaves

© Digital Cloud Training | https://digitalcloud.training
AWS Nitro System
•Nitro is the underlying platform for the next
generation of EC2 instances
•Support for many virtualized and bare metal
instance types
•Breaks functions into specialized hardware
with a Nitro Hypervisor
•Specialized hardware includes:
•Nitro cards for VPC
•Nitro cards for EBS
•Nitro for Instance Storage
•Nitro card controller
•Nitro security chip
•Nitro hypervisor
•Nitro Enclaves

© Digital Cloud Training | https://digitalcloud.training
AWS Nitro System
•Improves performance, security and innovation:
•Performance close to bare metal for virtualized
instances
•Elastic Network Adapter and Elastic Fabric Adapter
•More bare metal instance types
•Higher network performance (e.g. 100 Gbps)
•High Performance Computing (HPC) optimizations
•Dense storage instances (e.g. 60 TB)

© Digital Cloud Training | https://digitalcloud.training
AWS Nitro Enclaves
•Isolated compute environments
•Runs on isolated and hardened virtual machines
•No persistent storage, interactive access, or external
networking
•Uses cryptographic attestation to ensure only
authorized code is running
•Integrates with AWS Key Management Service (KMS)
•Protect and securely process highly sensitive data:
•Personally identifiable information (PII)
•Healthcare data
•Financial data
•Intellectual Property data

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Pricing Options

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Pricing Options
## Reserved
Spot InstancesDedicated Instances
## Dedicated Hosts
On-Demand
## Savings Plans
Standard rate -  no discount; no
commitments; dev/test, short-term, or
unpredictable workloads
1 or 3-year commitment; up to 75% discount;
steady-state, predictable workloads and
reserved capacity
Low price for unused capacity; up to 90%
discount; may be terminated by AWS;
workloads with flexible start and end times
Physical isolation at the host hardware level
from instances belonging to other
customers; pay per instance
Flexible pricing with commitment to a set
spend over time
Physical server dedicated for your use;
Socket/core visibility, host affinity; pay per
host; workloads with server-bound software
licenses

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Billing
Billed per hour;
Minimum of 1 hour
Billed per second;
Minimum of 1 minute
Volumes billed per second;
Minimum of 1 minute
Some Linux distros such as SUSE and
Ubuntu use hourly pricing
Per-second billing is for Amazon Linux,
Windows, RHEL and Ubuntu/Ubuntu Pro

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Reserved Instances (RIs)
Standard RIConvertible RI
Change AZ,
instance size,
networking type
Change AZ,
instance size,
networking type
## +
Change family, OS,
tenancy, payment option
Term is 1 or 3 years
Use ModifyReservedInstances API
Can pay All Upfront, Partial
## Upfront, No Upfront
Use ExchangeReservedInstances API

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Reserved Instances (RIs)
When the attributes of a used instance
match the attributes of an RI the
discount is applied
Tenancy: Default or Dedicated
## Availability Zone
## Region

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 On-Demand Capacity Reservations
•Reserve compute capacity for your Amazon EC2 instances in a
specific Availability Zone
•Any duration can be specified
•Mitigates against the risk of being unable to get On-Demand
capacity
•Does not require any term commitments and can be cancelled at
any time
•When you create a Capacity Reservation, you specify:
•The Availability Zone in which to reserve the capacity
•The number of instances for which to reserve capacity
•The instance attributes, including the instance type, tenancy,
and platform/OS

© Digital Cloud Training | https://digitalcloud.training
Capacity Blocks for ML
Use cases for Capacity Blocks:
•ML model training and fine-tuning – Get uninterrupted access to
the GPU instances that you reserved to complete ML model
training and fine-tuning
•ML experiments and prototypes – Run experiments and build
prototypes that require GPU instances for short durations

© Digital Cloud Training | https://digitalcloud.training
AWS Savings Plans
## Compute Savings Plan
EC2 Instance Savings Plans
1 or 3-year; commitment
to usage of EC2, Fargate,
## Lambda
1 or 3-year; commitment
to usage of Amazon EC2
instances on a specific
instance family in a
specific AWS Region
## Machine Learning Savings Plan
1 or 3-year; commitment
to usage of Amazon
SageMaker

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Spot Instances
Spot Fleet: launches and maintains the number of
Spot / On-Demand instances to meet specified
target capacity
EC2 Fleet: launches and maintains specified
number of Spot / On-Demand / Reserved
instances in a single API call
2-  minute warning if AWS
need to reclaim capacity –
available via instance
metadata and CloudWatch
## Events
Spot Instance: One or more EC2 instances
Can define separate OD/Spot capacity
targets, Spot price, instance types, and AZs

© Digital Cloud Training | https://digitalcloud.training
Dedicated Instances and Dedicated Hosts
CharacteristicDedicated InstancesDedicated Hosts
Enables the use of dedicated physical serversXX
Per instance billing (subject to a $2 per region fee)X
Per host billingX
Visibility of sockets, cores, host IDX
Affinity between a host and instanceX
Targeted instance placementX
Automatic instance placementXX
Add capacity using an allocation requestX

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Pricing Use
## Cases

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Pricing Use Cases
Developer working on a small
project for several hours;
cannot be interrupted
## Reserved
## Capacity Reservation
## Spot Instances
## Dedicated Instances
## Dedicated Hosts
On-Demand
Compute-intensive, cost-
sensitive distributed
computing; can withstand
interruption
Steady-state, business critical,
line-of  -business application;
continuous demand

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Pricing Use Cases
Need to Guarantee capacity is
available in a specific AZ
## Reserved
## Spot Instances
## Dedicated Instances
## Dedicated Hosts
On-Demand
Database with per-socket
licensing
Security-sensitive application,
requires dedicated hardware;
per-instance billing
## Capacity Reservation

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns –
Amazon EC2

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – Amazon EC2
Company needs to run a short batch
script to configure Amazon EC2 Linux
instances after they are launched
Add the bash script to the user data of
the EC2 instances
A tightly coupled High Performance
Computing (HPC) workload requires
low-latency between nodes and
optimum network performance
Launch EC2 instances in a single AZ in a
cluster placement group and use an
Elastic Fabric Adapter (EFA)
LoB application receives weekly bursts
of traffic and must scale for short
periods – need the most cost-effective
solution
Use reserved instances for minimum
required workload and then use Spot
instances for the bursts in traffic
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns - Amazon EC2
RequirementSolution
A single instance application uses a
static public IP address. In the event of
failure, the address must be remapped
to a failover instance
Attach an Elastic IP address to the EC2
instance. Remap the EIP in the event of
failure
A fleet of Amazon EC2 instances run in
private subnets across multiple AZs.
Company needs a redundant path to
the internet
Deploy NAT Gateways into multiple AZs
and update route tables
A team of engineers must administer
EC2 instances in private subnets from
remote locations using SSH
Deploy a bastion host in a public subnet
and instruct the engineers to use the
bastion host to “jump” to the instances
in private subnets

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns - Amazon EC2
RequirementSolution
An application uses several EC2
instances. Architect must eliminate the
risk of correlated hardware failures
Launch the instances in a spread
placement group across distinct
underlying hardware
Application requires enhanced
networking capabilities
Choose an instance type that supports
enhanced networking and ensure the
ENA module is installed and ENA
support is enabled
Instance needs close to bare metal
performance, EFA, and high
performance networking
Use an AWS Nitro instance type

© Digital Cloud Training | https://digitalcloud.training
## SECTION 4
Elastic Load Balancing, and Auto Scaling

© Digital Cloud Training | https://digitalcloud.training
Scaling Up vs Scaling Out

© Digital Cloud Training | https://digitalcloud.training
Stateful vs Stateless Applications
StatefulStateless
Person checks a
weather website
No “state” is
recorded about
the user's session
Person browses /
purchases on Amazon
Amazon stores
information
about activity

© Digital Cloud Training | https://digitalcloud.training
Stateful vs Stateless Applications
## Application Server
## Web Server
## Database Server
## User
eCommerce Application
The cart items are
stored in cookies
on the computer
No data is stored on the
web server, it is stateless
When the user purchases, the application
layer processes the order and records the
data in the database. This is stateful

© Digital Cloud Training | https://digitalcloud.training
Stateful vs Stateless Applications
## Application Server
## Web Server
## Database Server
## User
eCommerce Application
The cart items are
stored in cookies
on the computer
No data is stored on the
web server, it is stateless
When the user purchases, the application
layer processes the order and records the
data in the database. This is stateful

© Digital Cloud Training | https://digitalcloud.training
Scalability and Elasticity: Scaling Up
## Operating System
Web service

© Digital Cloud Training | https://digitalcloud.training
Scalability and Elasticity: Scaling Up
## Operating System
Web service
Scaling up means adding
resources to the server

© Digital Cloud Training | https://digitalcloud.training
Scalability and Elasticity: Scaling Out
## Operating System
Web service
## Operating System
Web service
## Operating System
Web service
## Operating System
Web service
## Operating System
Web service
## Operating System
Web service

© Digital Cloud Training | https://digitalcloud.training
Scaling Up vs Out
t2.micro, 1
vCPU, 1 GB
## RAM
c5.xlarge, 4
vCPU, 8 GB
## RAM
Scaling UP
Scaling OUT

© Digital Cloud Training | https://digitalcloud.training
Which scaling model should be used?
EC2 with MySQL DB
Scale UP
EC2 with Static Website
Scale OUT

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Auto Scaling

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Auto Scaling
•Automatically launches and terminates
instances
•Maintain availability and scale capacity
•Works with EC2, ECS, and EKS
•Integrates with many AWS services, including:
•CloudWatch for monitoring and scaling
•Elastic Load Balancing for distributing connections
•EC2 Spot Instances for cost optimization
•Amazon VPC for deploying instances across AZs

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Auto Scaling
## Availability Zone
Public subnet
## Availability Zone
Public subnet
Auto Scaling group
MetricsMetrics
Metric reports
## CPU > 80%
Amazon CloudWatch
CloudWatch notifies
## Auto Scaling
Auto Scaling launches
an extra instance
EC2 Status
Checks fail
ASG replaces
failed instance
1.Automatic scaling
2.Maintaining availability

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Auto Scaling
•Scaling is horizontal (scales out)
•Provides elasticity and scalability
•Responds to EC2 status checks and CloudWatch
metrics
•Can scale based on demand (performance) or on a
schedule
•Scaling policies define how to respond to changes
in demand

© Digital Cloud Training | https://digitalcloud.training
Configuration of an Auto Scaling Group
## Launch Template
AMI and instance type
EBS volumes
Security groups
Key pair
IAM instance profile
User data
Shutdown behavior
Termination protection
Placement group name
Capacity reservation
## Tenancy
Purchasing option (e.g. Spot)
## Launch Config
AMI and instance type
EBS volumes
Security groups
Key pair
Purchasing option (e.g. Spot)
IAM instance profile
User data
## Configure
purchase options
– On-demand vs
## Spot
Configure VPC
and Subnets
## Attach Load
## Balancer
Configure health
checks EC2 & ELB
Group size and
scaling policies
## A Launch Template
specifies the EC2
instance configuration
Launch Configurations are
replaced by launch templates
and have fewer features

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Auto Scaling
•Health checks
•EC2 = EC2 status checks
•ELB = Uses the ELB health checks in addition to EC2
status checks
•Health check grace period
•How long to wait before checking the health status of
the instance
•Auto Scaling does not act on health checks until grace
period expires

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Auto Scaling
Types of Auto Scaling:
•Manual –   make changes to ASG size manually
•Dynamic –   automatically scales based on demand
•Predictive –   uses Machine Learning to predict
•Scheduled –   scales based on a schedule

© Digital Cloud Training | https://digitalcloud.training
Create an Auto Scaling Group

© Digital Cloud Training | https://digitalcloud.training
High Availability and Fault
## Tolerance

© Digital Cloud Training | https://digitalcloud.training
High Availability vs Fault Tolerance
High AvailabilityFault Tolerance
•Minimal service interruption
•Designed with no single
point of failure (redundancy)
•Uptime measured in %, e.g.
## 99.99%
•Synchronous or
asynchronous replication
•Lower cost compared to FT
•Services that create HA:
•Elastic Load Balancing
•EC2 Auto Scaling
•Amazon Route 53
•No service interruption
•Specialized hardware with
instantaneous failover
•No downtime
•Synchronous replication
•Higher cost compared to HA
•Examples of FT:
•Fault tolerant NICs
•Disk mirroring (RAID 1)
•Synchronous DB replication
•Redundant power

© Digital Cloud Training | https://digitalcloud.training
## Fault Tolerance
Memory (RAM)
Processor (CPU)
## Hard Disk Drive
## Network Card
## Hard Disk Drive
Redundant components
allow the system to
continue to operate
The system may fail if there is
no built-in redundancy

© Digital Cloud Training | https://digitalcloud.training
High Availability and Fault Tolerance
## Web Server 1
## Web Server 2
## Web Server 3
## User 3
## User 2
## User 1
Think of an availability zone as
a separate data center
## Availability Zone
## Availability Zone
## Web Server 4
## Cloud
## Load Balancer

© Digital Cloud Training | https://digitalcloud.training
High Availability and Fault Tolerance
## Cloud
## Web Server 1
## Web Server 3
## User 3
## User 2
## User 1
## Availability Zone
## Availability Zone
## Web Server 4
## Auto Scaling
## Web Server 5
Think of an availability zone as
a separate data center
Auto Scaling launches
a new web server
## Load Balancer

© Digital Cloud Training | https://digitalcloud.training
High Availability and Fault Tolerance
## Cloud
## Web Server 1
## User 3
## User 2
## User 1
## Availability Zone
## Web Server 5
## Load Balancer
Think of an availability zone as
a separate data center

© Digital Cloud Training | https://digitalcloud.training
Durability and Availability
If you store 10 million objects in S3,
then you can expect to lose one
object every 10,000 years!
Availability is a measurement
of:
•The amount of time the
data is available to access
•Expressed as a percent of
time per year
•E.g. 99.99%
Durability is protection
against:
•Data loss
•Data corruption
•S3 offers 11 9s durability
## (99.999999999)
DurabilityAvailability

© Digital Cloud Training | https://digitalcloud.training
## Amazon Elastic Load
## Balancing

© Digital Cloud Training | https://digitalcloud.training
## Amazon Elastic Load Balancing
•Provides high availability and fault tolerance
•Targets include:
•Amazon EC2 instances
•Amazon ECS containers
•IP addresses
•Lambda functions
•Other load balancers

© Digital Cloud Training | https://digitalcloud.training
## Amazon Elastic Load Balancing
## Availability Zone
Public subnet
## Elastic Load Balancer
## Availability Zone
Public subnet
## User 3
## User 2
## User 1
## Auto Scaling
ELB takes instance 1
out of service (failed
health check)
EC2 Auto Scaling
terminates
instance 1
## Instance 1
## Instance 2
## Instance 3
## Instance 4
User 1 is connected
to instance 4

© Digital Cloud Training | https://digitalcloud.training
## Amazon Elastic Load Balancing
## Availability Zone
Public subnet
## ELB
## Availability Zone
Public subnet
## User 3
## User 2
## User 1
## Auto Scaling
EC2 Auto Scaling
launches
instance 5
## Instance 5
## Instance 2
## Instance 3
## Instance 4
## User 4

© Digital Cloud Training | https://digitalcloud.training
Types of Elastic Load Balancer (ELB)
## Network Load
## Balancer
## Application Load
## Balancer
## Load Balancer Protocol:
## TCP, TLS, UDP, TCP_UDP
## Instance Protocol:
## TCP, TCP_UDP
## Load Balancer Protocol:
## HTTP, HTTPS
## Instance Protocol:
## HTTP, HTTPS
## Internet Client
## Internet Client
•Operates at the connection level
•Routes connections based on IP protocol data (L4)
•Offers ultra high performance, low latency and TLS
offloading at scale
•Can have a static IP / Elastic IP
•Supports UDP and static IP addresses as targets
•Operates at the request level
•Routes based on the content of the request (L7)
•Supports path-based routing, host-based routing,
query string parameter-based routing, and source
IP address-based routing
•Supports instances, IP addresses, Lambda functions
and containers as targets
## Application Load Balancer
## Network Load Balancer

© Digital Cloud Training | https://digitalcloud.training
Types of Elastic Load Balancer (ELB)
## Gateway Load Balancer
## Load Balancer Protocol:
All packets on all ports
•Used in front of virtual appliances such as firewalls,
IDS/IPS, and deep packet inspection systems
•Operates at Layer 3 – listens for all packets on all
ports
•Forwards traffic to the TG specified in the listener
rules
•Exchanges traffic with appliances using the GENEVE
protocol on port 6081
## Appliance Protocol:
## GENEVE
## Gateway Load Balancer
VPC Endpoint
## Virtual Appliance

© Digital Cloud Training | https://digitalcloud.training
ELB Use Cases
## Application Load Balancer
•Web applications with L7 routing (HTTP/HTTPS)
•Microservices architectures (e.g. Docker containers)
•Lambda targets
## Network Load Balancer
•TCP and UDP based applications
•Ultra-low latency
•Static IP addresses
•VPC endpoint services

© Digital Cloud Training | https://digitalcloud.training
ELB Use Cases
## Gateway Load Balancer
•Deploy, scale and manage 3
rd
party virtual network appliances
•Centralized inspection and monitoring
•Firewalls, intrusion detection and prevention systems, and deep
packet inspection systems

© Digital Cloud Training | https://digitalcloud.training
ALB and NLB Deployments

© Digital Cloud Training | https://digitalcloud.training
ELB Deployments
## Subnet
## Subnet
## Target Group
Network mappings define:
•Availability Zones
•Subnets
Target groups define:
•Target type
•Target protocol / port
## •VPC
•Health checks
•Registered targets
The ELB listener defines:
•Listener protocol /port
•Routing rules
•SSL/TLS certificate
The ELB deploys nodes in
each AZ it is mapped to

© Digital Cloud Training | https://digitalcloud.training
ELB Supported Configurations
Application Load Balancer (ALB)
•Target type can be:
## •instance
## •ip
## •lambda
•Target group protocol must
be HTTP/HTTPS
•Health check protocol must
be HTTP/HTTPS
•Can define rules for
advanced request routing
Network Load Balancer (NLB)
•Target type can be:
## •instance
## •ip
## •alb
•Target group protocol must
be TCP/UDP
•Any health check protocol is
supported
•Can define elastic IP per
subnet

© Digital Cloud Training | https://digitalcloud.training
Routing with Application Load Balancer (ALB)
## Subnet
## Subnet
## Subnet
## TG1
## TG2
## TG3
## Application Load
Balancer (ALB)
https://example.com/orders
https://example.com/specials
https://members.example.com/
Requests can also be routed based on
the host field in the HTTP header
Target groups are used
to route requests to
registered targets
Targets can be EC2
instances, IP addresses,
and Lambda functions
Requests can be
routed based on the
path in the URL
A rule is configured
on the listener.
ALBs listen on
## HTTP/HTTPS
## Path-based
routing
Host-based routing

© Digital Cloud Training | https://digitalcloud.training
Routing with Network Load Balancer (NLB)
## Subnet
## Subnet
## Subnet
## TG1
## TG2
## Network Load
Balancer (NLB)
https://example.com:8080
https://example.com
## 54.22.182.2
## 54.239.28.85
## 54.12.10.212
Requests are routed based
on IP protocol data
NLB nodes can
have elastic IPs in
each subnet
NLBs listen on
TCP, TLS, UDP or
## TCP_UDP
Targets can be EC2
instances, IP addresses,
or ALBs
Targets can be
outside a VPC
(e.g. on-premises)
A separate listener on a
unique port is required
for routing

© Digital Cloud Training | https://digitalcloud.training
What’s the Source IP Address the App sees?
## IP=A
## IP=B
SourceProtocolPort
## IP=BTCP80
## AWS NLB
## AWS ALB
## AWS NLB
## Instance
specified by
Instance ID
## Instance
specified by IP
## Address
SourceProtocolPort
## IP=ATCP80
SourceProtocolPort
## IP=BTCP80
## IP=A
## IP=B
## IP=A
## IP=B
Note: X-forwarded-for can be used with ALB to capture client IPs
CLB and ALB use private IP of
their ENIs as source address
When using an NLB with a VPC Endpoint or
AWS GA source IPs are private IPs of NLB nodes
Applicable to TCP
and TLS – for UDP
and TCP_UDP
should be IP=A
https://
aws.amazon.com/premiumsupport/knowledge-
center/elb-capture-client-ip -addresses/

© Digital Cloud Training | https://digitalcloud.training
Create an Application
## Load Balancer

© Digital Cloud Training | https://digitalcloud.training
Amazon EC2 Scaling Policies

© Digital Cloud Training | https://digitalcloud.training
## Dynamic Scaling – Target Tracking
## Availability Zone
Public subnet
## Availability Zone
Public subnet
Auto Scaling group
MetricsMetrics
Amazon CloudWatch
ASGAverageCPUUtilization = 60%
## 677465
Average CPU = 71.5%
## 80
AWS recommend scaling on metrics
with a 1-  minute frequency
Instance metrics are not
counted until warm-up
time has expired

© Digital Cloud Training | https://digitalcloud.training
## Dynamic Scaling – Simple Scaling
## Auto Scaling
group
## CPU = 70%
Launch 2 instances
Alarm set to CPU >= 60%
Wait 300 seconds before allowing
another scaling activity

© Digital Cloud Training | https://digitalcloud.training
## Dynamic Scaling – Step Scaling
## Auto Scaling
group
## CPU = 70%
Launch 2 instances
Alarm set to CPU >= 60%
## Auto Scaling
group
## CPU = 80%
Launch 4 instances
Alarm set to CPU >= 60%

© Digital Cloud Training | https://digitalcloud.training
## Scheduled Scaling
## Auto Scaling
group
Launch X instances
Schedule set to scale
daily at 08:45

© Digital Cloud Training | https://digitalcloud.training
Create a Scaling Policy

© Digital Cloud Training | https://digitalcloud.training
Cross-Zone Load Balancing

© Digital Cloud Training | https://digitalcloud.training
Cross-Zone Load Balancing
When cross-zone load balancing is enabled:
•Each load balancer node distributes traffic across the registered
targets in all enabled Availability Zones
When cross-zone load balancing is disabled:
•Each load balancer node distributes traffic only across the registered
targets in its Availability Zone
•With Application Load Balancers, cross-zone load balancing is always
enabled
•With Network Load Balancers and Gateway Load Balancers, cross-
zone load balancing is disabled by default

© Digital Cloud Training | https://digitalcloud.training
Cross-Zone Load Balancing - Disabled
## Availability Zone A
Public subnet
ELB Node
## Elastic Load
## Balancer
## Availability Zone B
Public subnet
ELB Node
## 16.6%
## 16.6%
## 16.6%
## 25%
## 25%
If cross-zone load
balancing is disabled:
•Each of the three
targets in Availability
Zone A receives
16.6% of the traffic
•Each of the two
targets in Availability
Zone B receives 25%
of the traffic
## 50%
## 50%

© Digital Cloud Training | https://digitalcloud.training
Cross-Zone Load Balancing - Enabled
If cross-zone load
balancing is enabled:
•Each of the five
targets receives 20%
of the traffic
## Availability Zone A
Public subnet
ELB Node
## Elastic Load
## Balancer
## Availability Zone B
Public subnet
ELB Node
## 20%
## 20%
## 20%
## 20%
## 20%
## 60%
## 40%

© Digital Cloud Training | https://digitalcloud.training
Session State and Session
## Stickiness

© Digital Cloud Training | https://digitalcloud.training
## Storing Session State
## Availability Zone
Public subnet
## Elastic Load Balancer
## Availability Zone
Public subnet
DynamoDB Table
Session data such as
authentication details
stored in DynamoDB Table
Session data retrieved
from DynamoDB Table
ElastiCache is also a popular
solution for storing session-
state data
User does not need to
re-authenticate

© Digital Cloud Training | https://digitalcloud.training
## Sticky Sessions
## Availability Zone
Public subnet
## Elastic Load Balancer
## Availability Zone
Public subnet
Session data such as
authentication details
stored locally
If an instance fails, session
state is lost – use with session
state store for more resiliency
Client is directed to
another instance
Cookie is generated and
client bound to instance
for the cookie lifetime

© Digital Cloud Training | https://digitalcloud.training
Secure Listeners for ELB

© Digital Cloud Training | https://digitalcloud.training
SSL/TLS Termination
## AWS ALB
## SSL/TLS CERT
## Encrypted
## Unencrypted
## AWS ALB
## SSL/TLS CERT
## Encrypted
## SSL/TLS CERT
## Encrypted
ACM certificate or
certificate imported
into ACM or IAM
With a L7 ELB a new connection
is established with the instance
Self-signed certificate can be
used, or a certificate from a
private certificate authority

© Digital Cloud Training | https://digitalcloud.training
SSL/TLS Termination
## AWS NLB
## SSL/TLS CERT
## Encrypted
## AWS NLB
## SSL/TLS CERT
## Encrypted
## SSL/TLS CERT
## Encrypted
Single encrypted
connection
Public certificate
must be used

© Digital Cloud Training | https://digitalcloud.training
Create a Secure Listener

© Digital Cloud Training | https://digitalcloud.training
Network Load Balancer (NLB)

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns –
Auto Scaling and ELB

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns - Auto Scaling and ELB
High availability and elastic scalability
for web servers
Use Amazon EC2 Auto Scaling and an
Application Load Balancer across
multiple AZs
Low-latency connections over UDP to a
pool of instances running a gaming
application
Use a Network Load Balancer with a
UDP listener
Clients need to whitelist static IP
addresses for a highly available load
balanced application in an AWS Region
Use an NLB and create static IP
addresses in each AZ
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns - Auto Scaling and ELB
Application on EC2 in an Auto Scaling
group requires disaster recovery across
## Regions
Create an ASG in a second Region with
the capacity set to 0. Take snapshots
and copy them across Regions (Lambda
or DLM)
Application on EC2 must scale in larger
increments if a big increase in traffic
occurs, compared to small increases in
traffic
Use Auto Scaling with a Step Scaling
policy and configure a larger capacity
increase
Need to scale EC2 instances behind an
ALB based on the number of requests
completed by each instance
Configure a target tracking policy using
the ALBRequestCountPerTarget metric
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns - Auto Scaling and ELB
RequirementSolution
Application runs on EC2 behind an ALB.
Once authenticated users should not
need to reauthenticate if an instance
fails
Use session state store such as
DynamoDB or ElastiCache
Company is deploying an IDS/IPS
system using virtual appliances and
needs to scale horizontally
Deploy a Gateway Load Balancer in
front of the virtual appliances

© Digital Cloud Training | https://digitalcloud.training
## SECTION 5
AWS Organizations

© Digital Cloud Training | https://digitalcloud.training
AWS Organizations and
## Control Tower

© Digital Cloud Training | https://digitalcloud.training
AWS Organizations
•AWS organizations allows you to consolidate multiple AWS accounts into
an organization that you create and centrally manage
•Available in two feature sets:
•Consolidated Billing
•All features
•Includes root accounts and organizational units
•Policies are applied to root accounts or OUs
•Consolidated billing includes:
•Paying Account – independent and cannot access resources of other
accounts
•Linked Accounts – all linked accounts are independent

© Digital Cloud Training | https://digitalcloud.training
AWS Organizations
AWS Organization
## Management Account
Te s tDevelopment
## Production
Enable IAM  Identity Center
Enable CloudTrail in
management account
and apply to members
Receive a
consolidated bill
Create accounts programmatically
using the Organizations API
You can group accounts into
Organizational Units (OUs)
## Service Control Policies
(SCPs) can control
tagging and the available
API actions

© Digital Cloud Training | https://digitalcloud.training
AWS Organizations API
•The AWS Organizations API can be used to automate organization and
account creation
•The following API actions are useful to know:
- CreateOrganization – creates an organization
- CreateAccount – creates an account that is a member of the organization
- CreatePolicy – creates a policy that can be attached to a root, OU, or
individual AWS account
- AttachPolicy - Attaches a policy to a root, an organizational unit (OU), or an
individual account
- InviteAccountToOrganization - Sends an invitation to another account to join
your organization as a member account

© Digital Cloud Training | https://digitalcloud.training
## Service Control Policies
AWS Organization
## Management
## Account
Te s t
## Dev
## Prod
NOTE: SCPs do not grant ANY
permissions, they control the
AVAILABLE permissions
SCPs control the maximum available permissions
Tag policy applied to enforce
tag standardization
Users in the management
account are not restricted
## Root Account
Dev users can only launch
T2.micro instances
Prod users cannot launch any instance other
than t2.micro (denied above)

© Digital Cloud Training | https://digitalcloud.training
SCP Strategies and Inheritance
Deny List StrategyAllow List Strategy
•The FullAWSAccess SCP
is attached to every OU and
account
•Explicitly allows all
permissions to flow down
from the root
•Can explicitly override with
a deny in an SCP
•This is the default setup
•The FullAWSAccess SCP
is
removed from every OU
and account
•To allow a permission, SCPs
with allow statements must
be added to the account
and every OU above it
including root
•Every SCP in the hierarchy
must explicitly allow the
APIs you want to use
Note: An explicit deny overrides any
kind of allow

© Digital Cloud Training | https://digitalcloud.training
## Service Control Policy Strategies
## Root
## OU1
## OU2
## Root
## OU1
## OU2
Deny List StrategyAllow List Strategy
DynamoDB is denied as it’s
not allowed at every level

© Digital Cloud Training | https://digitalcloud.training
AWS Organizations vs Control Tower
AWS Organizations
•Manage multiple accounts
•Consolidated billing
•Organizational Units
•Service Control Policies
•Tag Policies
•Backup Policies
AWS Control Tower
•Extends capabilities of AWS
## Organizations
•Landing Zones (best practices)
•Federated Access (IAM
## Identity Center)
•Centralized Logging
•Account Factory (automation)
•Guardrails (governance rules)

© Digital Cloud Training | https://digitalcloud.training
AWS Control Tower
AWS Organization
AWS Control Tower
Security OUSandbox OU
## Root
Production OU
## Audit
## Log
## Archive
## Mgmt
Dev/Test
## Prod
## Landing Zone
IAM Identity Center
A landing zone is a well-architected
multi-account baseline
Preventive Guardrails disallow API
actions using SCPs
Detective Guardrails are used for
governance and compliance
Directory source can be IAM
Identity Center , SAML 2.0 IdP,
or Microsoft AD

© Digital Cloud Training | https://digitalcloud.training
AWS Control Tower
•Control Tower creates a well-architected multi-
account baseline based on best practices
•This is known as a landing zone
•Guardrails are used for governance and
compliance:
•Preventive guardrails are based on SCPs and disallow
API actions
•Detective guardrails are implemented using AWS
Config rules and Lambda functions and monitor and
govern compliance
•The root user in the management account can
perform actions that guardrails would disallow

© Digital Cloud Training | https://digitalcloud.training
Create AWS Organization and
## Add Account

© Digital Cloud Training | https://digitalcloud.training
## Account Configuration
AWS Organization
## Management Account
## Production
AWS Organizations
Production (OU)
OrganizationAccountAccessRole
Create a Service Control Policy
(SCP) and attach to OU
Role has full permissions
in the account
Role can be assumed by any user with
the sts:AssumeRole permissions

© Digital Cloud Training | https://digitalcloud.training
Service Control Policies (SCPs)

© Digital Cloud Training | https://digitalcloud.training
## Service Control Policies
AWS Organization
## Management
## Account
## Root
Te s t
## Dev
## Prod
Dev users can only
launch T2.micro
instances
Prod users cannot launch
any instance other than
t2.micro (denied above)
Users in the
management
account are
not restricted
Tag policy applied
to enforce tag
standardization
SCPs control the maximum
available permissions
NOTE: SCPs do not grant ANY
permissions, they control the
AVAILABLE permissions

© Digital Cloud Training | https://digitalcloud.training
## Create Service Control
Policy (SCP)

© Digital Cloud Training | https://digitalcloud.training
AWS Control Tower

© Digital Cloud Training | https://digitalcloud.training
AWS Control Tower
AWS Organization
AWS Control Tower
Security OUSandbox OU
## Root
Production OU
## Landing Zone
IAM Identity Center
## Prod
## Mgmt
## Dev/
Te s t
## Audit
## Log
## Archive
A landing zone is a well-architected
multi-account baseline
Preventive Guardrails disallow
API actions using SCPs
Detective Guardrails are used for
governance and compliance
Directory source can be
IAM Identity Center, SAML
2.0 IdP, or Microsoft AD

© Digital Cloud Training | https://digitalcloud.training
AWS Control Tower – Shared Accounts
•Management account – The AWS account used to launch
AWS Control Tower. The root user and IAM administrator
have full access to all resources in the landing zone
•Log archive account – Contains a central Amazon S3 bucket
for storing a copy of all AWS CloudTrail and AWS Config log
files for all other accounts in the landing zone
•Audit account – Aggregates and stores logs collected from
all other accounts in the landing zone. Secure account with
restricted access

© Digital Cloud Training | https://digitalcloud.training
AWS Control Tower - Guardrails
Preventive guardrails
•Purpose: Preventive guardrails are designed to proactively
prevent policy violations before they occur. They enforce
compliance and security best practices by restricting certain
actions or configurations
•How They Work: These guardrails are implemented using AWS
Service Control Policies (SCPs). They effectively limit what
actions users and roles can perform in the AWS accounts
within the organization
•Examples:
•Disallow Deletion of CloudTrail Logs and S3 Logging Buckets
•Disallow Public Read Access to S3 Buckets
•Require Encryption on EBS Volumes
•Disallow RDP/SSH Access from 0.0.0.0/0

© Digital Cloud Training | https://digitalcloud.training
AWS Control Tower - Guardrails
## Detective Guardrails
•Purpose: Detective guardrails are designed to monitor and
report on policy violations or non-compliant activities that have
already occurred. They help in identifying misconfigurations or
activities that do not adhere to the organization's policies
•How They Work: These guardrails are implemented using AWS
Config rules and Lambda functions. They continuously evaluate
the configuration of AWS resources and generate alerts or
reports when non-compliance is detected
•Examples:
•Detecting publicly accessible Amazon S3 buckets
•Detect whether versioning is enabled for Amazon S3 buckets
•Detect whether encryption is enabled for Amazon RDS instances
•Monitoring for IAM policies that grant overly broad permissions

© Digital Cloud Training | https://digitalcloud.training
AWS Organizations vs Control Tower
AWS Organizations
•Manage multiple accounts
•Consolidated billing
•Organizational Units
•Service Control Policies
•Tag Policies
•Backup Policies
AWS Control Tower
•Extends capabilities of AWS
## Organizations
•Landing Zones (best practices)
•Federated Access (IAM
## Identity Center)
•Centralized Logging
•Account Factory (automation)
•Guardrails (governance rules)

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns –
AWS Organizations

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – AWS Organizations
A company needs a method of quickly
creating AWS accounts
programmatically
Use the Organizations API to create the
accounts programmatically
Users in a member account in AWS
Organizations should be restricted
from making changes in IAM
User a Service Control Policy (SCP) to
deny access to IAM actions
An AWS account must be moved
between Organizations
Migrate the account using the AWS
Organizations console
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – AWS Organizations
A solutions architect created a new
account through the Organizations
console and needs to login to launch
resources
The architect should switch roles to
access the new account
Multiple member accounts in AWS
Organizations require the same
permissions to be restricted using SCPs
Create an OU and add the member
accounts then attach the SCP to the OU
The developers in a company each
have their own AWS accounts for
testing. The security team wish to
enable central governance
Create an AWS Organization and send
an invite to each developer’s AWS
account to join the Organization
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## SECTION 6
Amazon Virtual Private Cloud (VPC)

© Digital Cloud Training | https://digitalcloud.training
The AWS Global Infrastructure

© Digital Cloud Training | https://digitalcloud.training
AWS Global Infrastructure
Region – us-east-1
## Availability
## Zone
## Availability
## Zone
## Availability
## Zone
Region – ap-southeast-2
## Availability
## Zone
## Availability
## Zone
## Availability
## Zone
Region – eu-west-1
## Availability
## Zone
## Availability
## Zone
## Availability
## Zone
There are many Regions
around the world
A Region is a separate
physical location in the world
Each region consists of
multiple Availability Zones
An Availability Zone is
composed of one or
more data centers

© Digital Cloud Training | https://digitalcloud.training
AWS Global Infrastructure
## Region
## Availability Zone
## Availability Zone
Corporate data center
AWS Outposts
## Instances
Outpost subnet
AWS Local
## Zone
## VPC
## Subnet
## Servers
Low latency
AWS Wavelength
## Zone
## VPC
## Subnet
## 5G
Low latency

© Digital Cloud Training | https://digitalcloud.training
AWS Global Infrastructure
## Region
## Availability Zone
Private subnet
Public subnet
## Availability Zone
Private subnet
Public subnet
## Redundant
## Power
## Sources
## Redundant
## Power
## Sources
## Redundant
## Networking
## Redundant
## Networking

© Digital Cloud Training | https://digitalcloud.training
Amazon CloudFront
## Edge
location
## Global
## Users
## Regional
## Edge Cache
## Edge
location
## Global
## Users
## Regional
## Edge Cache
## Edge
location
## Global
## Users
## Region
Amazon EC2
## Amazon S3
CloudFront Origins

© Digital Cloud Training | https://digitalcloud.training
## Deploying Services Globally
Region – us-east-1
Region – ap-
southeast-2
Region – eu-west-1
Region – us-west-1
AWS Management
## Console
Launch virtual servers and
databases

© Digital Cloud Training | https://digitalcloud.training
IP Addressing

© Digital Cloud Training | https://digitalcloud.training
Structure of an IPv4 Address
## 192
## ...
## 16801
## 11111111
## 1286432168421
Most significant bitLeast significant bit
## Binary Values
## 11000000
## 10101000
## 00000000
## 00000001
Each part of the address is
a binary octet
IP addresses are written in
dotted decimal notation

© Digital Cloud Training | https://digitalcloud.training
Networks and Hosts
## 192
## ...
## 16801
Network ID
Host ID
## 255
## ...
## 2552550
## Subnet Mask
An IPv4 address has a
network and host ID
The subnet mask is used to
define the network and host
## ID

© Digital Cloud Training | https://digitalcloud.training
Networks and Hosts
## 192
## ...
## 16800
## 255
## ...
## 2552550
## 192.168.0.0/24
## Network
## Subnet Mask
24 bits
## 192.168.0.1
## 192.168.0.2
## 192.168.0.3
## 192.168.0.4
## 192.168.0.5
## 192.168.0.6
All computers share the
same network ID and
have a unique host ID
A network and subnet
mask can also be
written in this format

© Digital Cloud Training | https://digitalcloud.training
Private IP Address Ranges
## 10000
## 10255255255
## 1721600
## 17231255255
## 19216800
## 192168255255
These addresses are reserved
for private use according to
## IETF RFC-1918

© Digital Cloud Training | https://digitalcloud.training
## Amazon Virtual Private Cloud
## (VPC)

© Digital Cloud Training | https://digitalcloud.training
Private subnet
Amazon VPC
## Region
## VPC
## Availability Zone
## Availability Zone
Public subnet
## Router
## Internet
gateway
## Main Route Table
EC2 Instance
EC2 Instance
DestinationTa rget
10.0.0.0/16Local
## 0.0.0.0/0igw-id
A VPC is a logically isolated portion
of the AWS cloud within a region
Subnets are
created within AZs
The route table is used
to configure the VPC
router
An Internet Gateway is
used to connect to the
## Internet
You can launch EC2 instances
into your VPC subnets

© Digital Cloud Training | https://digitalcloud.training
Amazon VPC
## Region
## VPC
## Availability Zone
Private subnet
Public subnet
## Availability Zone
Private subnet
Public subnet
## VPC
## Availability Zone
Private subnet
Public subnet
## Availability Zone
Private subnet
Public subnet
## CIDR 10.0.0.0/16
## CIDR 10.1.0.0/16
## 10.1.1.0/2410.1.2.0/24
## 10.1.3.0/2410.1.4.0/24
## 10.0.1.0/2410.0.2.0/24
## 10.0.3.0/2410.0.4.0/24
Each VPC has a different
block of IP addresses
You can create multiple VPCs
within each region
CIDR stands for Classless
## Interdomain Routing
Each subnet has a block of IP addresses
from the CIDR block

© Digital Cloud Training | https://digitalcloud.training
VPC CIDR Blocks and Subnets
## 10000
VPC CIDR Block
## 25525500
## /16 Subnet Mask
## 10.0.0.0/16
## 10.0.1.0/24
## 10.0.2.0/24
## 10.0.3.0/24
## Subnets:
## 2552552550
VPC subnets have a longer subnet
mask than the CIDR block by using
additional bits from the host portion

© Digital Cloud Training | https://digitalcloud.training
AWS Public and Private Services
## VPC
## Availability Zone
Private subnet
Public subnet
EC2 Instance
## Internet
gateway
EC2 Instance
AWS Cloud
Amazon RDS
## Amazon Elastic File System
## Amazon S3
Amazon DynamoDB
## Amazon Route 53
Amazon CloudFront
## Public Internet
Public services have public
IP addresses / endpoints
Private services can have
public IP addresses but
exist within the VPC

© Digital Cloud Training | https://digitalcloud.training
Defining VPC CIDR Blocks

© Digital Cloud Training | https://digitalcloud.training
Rules and Guidelines
•CIDR block size can be between /16 and /28
•The CIDR block must not overlap with any existing CIDR block
that's associated with the VPC
•You cannot increase or decrease the size of an existing CIDR
block
•The first four and last IP address are not available for use
•AWS recommend you use CIDR blocks from the RFC 1918
ranges:
RFC 1918 RangeExample CIDR Block
10.0.0.0 - 10.255.255.255 (10/8 prefix)Your VPC must be /16 or smaller, for example, 10.0.0.0/16
172.16.0.0 - 172.31.255.255 (172.16/12 prefix)Your VPC must be /16 or smaller, for example, 172.31.0.0/16
192.168.0.0 - 192.168.255.255 (192.168/16 prefix)Your VPC can be smaller, for example 192.168.0.0/20

© Digital Cloud Training | https://digitalcloud.training
VPC CIDR Blocks and Subnets
## 10000
VPC CIDR Block
## 25525500
## /16 Subnet Mask
## 10.0.0.0/16
## 10.0.1.0/24
## 10.0.2.0/24
## 10.0.3.0/24
## Subnets:
## 2552552550
VPC subnets have a longer
subnet mask than the CIDR
block by using additional bits
from the host portion

© Digital Cloud Training | https://digitalcloud.training
## Additional Considerations
•Ensure you have enough networks and hosts
•Bigger CIDR blocks are typically better (more
flexibility)
•Smaller subnets are OK for most use cases
•Consider deploying application tiers per subnet
•Split your HA resources across subnets in different
AZs
•VPC Peering requires non-overlapping CIDR blocks
•This is across all VPCs in all Regions / accounts you want
to connect
•Avoid overlapping CIDR blocks as much as possible!

© Digital Cloud Training | https://digitalcloud.training
Example VPC CIDR Block and Subnets
Subnet NameIPv4 CIDR blockAvailability ZoneRoute TableAuto-assign Public IP v4
private-1a10.0.0.0/24us-east-1aPrivate-RTNo
private-1b10.0.1.0/24us-east-1bPrivate-RTNo
private-1c10.0.2.0/24us-east-1cPrivate-RTNo
public-1a10.0.3.0/24us-east-1aMAINYe s
public-1b10.0.4.0/24us-east-1bMAINYe s
public-1c10.0.5.0/24us-east-1cMAINYe s
## 10000
VPC CIDR Block
## 25525500
## /16 Subnet Mask

© Digital Cloud Training | https://digitalcloud.training
Create a Custom VPC

© Digital Cloud Training | https://digitalcloud.training
Custom VPC
MyVPC
us-east-1a
Private-1A
Public-1A
## CIDR 10.0.0.0/16
## 10.0.1.0/24
## 10.0.3.0/24
MyIGW
## Main Route Table
DestinationTa rget
10.0.0.0/16Local
## 0.0.0.0/0igw-id
us-east-1b
Private-1B
Public-1B
## 10.0.2.0/24
## 10.0.4.0/24
Private-RT Route Table
DestinationTa rget
10.0.0.0/16Local

© Digital Cloud Training | https://digitalcloud.training
Security Groups and Network
ACLs

© Digital Cloud Training | https://digitalcloud.training
Stateful vs Stateless Firewalls
## Web Server (10.2.1.10)
## Dest Port: 80
A stateful firewall
allows the return
traffic automatically
## Firewall
## Src Port: 65188
Src Port: 80Dest Port: 65188
## PROTOCOLSOURCE IPDESTINATION IPSOURCE PORTDESTINATION PORT
## HTTP10.1.1.110.2.1.106518880
## HTTP10.2.1.1010.1.1.18065188
A stateless firewall
checks for an allow
rule for both
connections
## Client
## (10.1.1.1)

© Digital Cloud Training | https://digitalcloud.training
Security Groups and Network ACLs
## VPC
## Availability Zone
Public subnet
Private subnet
## Security
## Group A
## Availability Zone
Public subnet
Private subnet
## Security
## Group A
Network ACL
## Security
## Group B
## Security
## Group B
## Security
## Group A
## Router
Network ACL
Network ACL
Network ACL
## Security Groups
can be applied
to instances in
any subnet
NACLs apply at the
subnet level
NACLs apply only to
traffic entering /
exiting the subnet
Security Groups apply at the Instance level

© Digital Cloud Training | https://digitalcloud.training
Security Groups & Network Access Control Lists (NACLs)
Security GroupNetwork ACL
Operates at the instance (interface) levelOperates at the subnet level
Supports allow rules onlySupports allow and deny rules
StatefulStateless
Evaluates all rulesProcesses rules in order
Applies to an instance only if associated
with a group
Automatically applies to all instances in
the subnets its associated with

© Digital Cloud Training | https://digitalcloud.training
## Using Security Groups
and NACLs

© Digital Cloud Training | https://digitalcloud.training
VPC Peering

© Digital Cloud Training | https://digitalcloud.training
What is VPC Peering?
•A private network connection between two Amazon Virtual Private
Clouds (VPCs)
•Allows VPCs to communicate as if they were on the same network
•Uses AWS’s internal network, providing low-latency, high-bandwidth
connectivity
## VPC AVPC B
## 10.0.1.0/24
## 10.0.2.0/24
Traffic uses private networking and private IP addresses
A peering connection is created between the VPCs

© Digital Cloud Training | https://digitalcloud.training
Key Features of VPC Peering
•No Single Point of Failure –   VPC peering is highly available
and does not depend on a central gateway
•No Bandwidth Bottlenecks –   Traffic stays within AWS
infrastructure, avoiding internet-based congestion
•Works Across Accounts & Regions – Supports same-account
and cross-account peering, as well as inter-region VPC
peering
•Full IP Address Control –   Peered VPCs must have non-
overlapping CIDR blocks to avoid conflicts
•Supports All AWS Services –   Works with EC2, RDS, Lambda,
etc.

© Digital Cloud Training | https://digitalcloud.training
VPC Peering Deployment
## VPC AVPC B
## VPC C
## VPC D
## 10.0.1.0/24
## 10.0.2.0/24
## 10.0.3.0/24
## 10.0.4.0/24
•For fully meshed connectivity
this architecture requires:
•6 peering connections
•3 route table entries (min) per VPC
or 12 entries total
•With 8 VPCs there would need
to be:
•28 peering connections
•7 route table entries (min) per VPC
or 56 entries in total
Transitive routing is NOT supported

© Digital Cloud Training | https://digitalcloud.training
VPC Peering Deployment
## VPC AVPC B
## VPC D
## 10.0.1.0/24
## 10.0.2.0/24
## 10.0.4.0/24
Transitive routing is NOT supported
•VPC A and VPC B have direct
connectivity
•VPC B and VPC D have direct
connectivity
•Connectivity is not possible
between VPC A and VPC D via VPC B
VPC A must peer with VPC D

© Digital Cloud Training | https://digitalcloud.training
Limitations of VPC peering
No Transitive Routing – Traffic from VPC A cannot flow to VPC C via
## VPC B
Manual Route Table Updates Required – You must explicitly add
routes in each VPC for communication
No DNS Resolution by Default – For inter-region peering, you must
enable DNS resolution manually
FeatureVPC PeeringTransit GatewayVPNDirect Connect
Transitive routing?NoYe sNoNo
Multi-VPC scaling?LimitedScalableNoNo
Best for?1:1 private VPC
links
Multi-VPC
networks
Hybrid cloud Hybrid cloud

© Digital Cloud Training | https://digitalcloud.training
Routing with VPC Peering
## VPC
Public subnet
## Route Table
## CIDR: 10.0.2.0/24
## Management Account
## Production Account
EC2 Instance
## CIDR: 10.0.1.0/24
## VPC
Public subnet
EC2 Instance
Security group (VPCPEER-PROD)Security group  (VPCPEER-MGMT)
DestinationTa r ge t
## 10.0.1.0/24peering-id
ProtocolPortSource
ICMPAll10.0.2.0/24
## TCP220.0.0.0/0
ProtocolPortSource
ICMPAll10.0.1.0/24
## TCP220.0.0.0/0
DestinationTa r ge t
## 10.0.2.0/24peering-id
## Route Table

© Digital Cloud Training | https://digitalcloud.training
Routing with VPC Peering
## VPC AVPC B
## VPC C
## VPC D
## 10.0.1.0/24
## 10.0.2.0/24
## 10.0.3.0/24
## 10.0.4.0/24
DestinationTa r ge t
## 10.0.2.0/24peering-id -1
## 10.0.3.0/24peering-id -4
## 10.0.4.0/24peering-id -5
## PID 1
## PID 2
## PID 3
## PID 4
## PID 5
## PID 6
DestinationTa r ge t
## 10.0.1.0/24peering-id -4
## 10.0.2.0/24peering-id -6
## 10.0.4.0/24peering-id -3
DestinationTa r ge t
## 10.0.1.0/24peering-id -1
## 10.0.3.0/24peering-id -6
## 10.0.4.0/24peering-id -2
DestinationTa r ge t
## 10.0.1.0/24peering-id -5
## 10.0.2.0/24peering-id -2
## 10.0.3.0/24peering-id -3

© Digital Cloud Training | https://digitalcloud.training
Configure VPC Peering

© Digital Cloud Training | https://digitalcloud.training
VPC Peering
## VPC
Public subnet
## Route Table
## CIDR: 10.1.0.0/16
## US-EAST-1US-WEST-1
## CIDR: 10.0.0.0/16
## VPC
Public subnet
Security groupSecurity group
DestinationTa r ge t
## 10.0.0.0/16peering-id
ProtocolPortSource
ICMPAll10.1.0.0/16
## TCP220.0.0.0/0
ProtocolPortSource
ICMPAll10.0.0.0/16
## TCP220.0.0.0/0
DestinationTa r ge t
## 10.1.0.0/16peering-id
## Route Table

© Digital Cloud Training | https://digitalcloud.training
VPC Endpoints

© Digital Cloud Training | https://digitalcloud.training
VPC Endpoints
## VPC
Private subnet
EC2 Instance
AWS CloudFormation
Endpoint ENI
AWS PrivateLink
## VPC
Private subnet
## S3 Gateway
## Endpoint
## Amazon S3
EC2 Instance
Interface VPC Endpoint:
•Supports many services
•Uses an ENI
•Can use security groups
Gateway VPC Endpoint:
•Supports S3/DynamoDB
•Must add route to the
route table
•Can use endpoint policies
Keep traffic private and avoid the internet
AWS CodeDeploy

© Digital Cloud Training | https://digitalcloud.training
VPC Endpoints
Interface EndpointGateway Endpoint
Elastic Network Interface with a
private IP
A gateway that is a target for a
specific route
Uses DNS entries to redirect
traffic
Uses prefix lists in the route table
to redirect traffic
Many AWS servicesAmazon S3, DynamoDB
Use Security GroupsApply VPC Endpoint Policies

© Digital Cloud Training | https://digitalcloud.training
Create VPC Endpoint

© Digital Cloud Training | https://digitalcloud.training
VPC Gateway Endpoints
## VPC
Private subnet
DestinationTarget
pl-6ca54005 (com.amazonaws.ap-southeast-2.s3,  54.231.248.0/22, 54.231.252.0/24, 52.95.128.0/21)vpce-ID
## Route Table
## S3 Gateway
## Endpoint
## Amazon S3
EC2 Instance
EC2 instance connects to S3 using a private IP
IAM policies can
be applied to
endpoints
Bucket policies can limit
access to endpoint source
A route table entry is required with the
prefix list for S3 and the gateway ID

© Digital Cloud Training | https://digitalcloud.training
AWS Client VPN

© Digital Cloud Training | https://digitalcloud.training
AWS Client VPN
•AWS Client VPN is an OpenVPN-based VPN for connecting
remote end-user devices to AWS VPCs
•It is a fully managed solution that uses OpenVPN/SSL for
tunneling
•Authentication options inclue:
•Active Directory authentication
•Mutual authentication using certificates
•Federated authentication with SAML-based identity providers
•You can define which users/groups can access specific network
ranges
•Automatically scales to handle thousands of concurrent
connections
•Works with Windows, macOS, and Linux clients using
OpenVPN-based clients

© Digital Cloud Training | https://digitalcloud.training
AWS Client VPN
## Region
## VPC – CIDR 10.0.0.0/16
Private subnet – 10.0.5.0/24
Public subnet – 10.0.1.0/24
EC2 Instance
## VPN
## Endpoint
## VPN
## Assoc.
## Assoc.
## 10.0.5.12
## 10.0.1.15
VPN client connects over
## SSL/TLS (443)
CIDR 10.1.0.0/22 – performs
SNAT to 10.0.0.0/16
Client VPN network
interfaces created in
subnet
Local route of associated subnet
is added to client route table
DestinationGateway
## 10.0.0.0/1610.1.1.X

© Digital Cloud Training | https://digitalcloud.training
AWS Client VPN Deployment
## Deployment:
•You create a Client VPN endpoint in AWS
•Associate the endpoint with one or more VPC subnets
•This gives the VPN a presence inside your VPC
## Client Configuration:
•End users install an OpenVPN-based client and download the
VPN configuration file generated from AWS
•Users authenticate using the method you configured (e.g., AD,
SAML, or certificates)
## Authentication & Authorization:
•When a client connects, AWS Client VPN checks the credentials
•Based on authorization rules, it decides which VPC networks or
resources the client can access

© Digital Cloud Training | https://digitalcloud.training
AWS Site-to-Site VPN

© Digital Cloud Training | https://digitalcloud.training
AWS Virtual Private Network (VPN) Options
You can connect a VPC to remote networks and users
using the following VPN connectivity options:
•AWS Site-to-Site VPN –   an IPSec VPN connection
•AWS Client VPN – A managed client-based VPN
•AWS VPN CloudHub –   Multiple S2S VPNs
•Third party software VPN appliance –   EC2 instance
with 3rd party software

© Digital Cloud Training | https://digitalcloud.training
AWS Site-to-Site VPN
VPN connection
DestinationTa rget
## 192.168.0.0/16vgw-id
## Route Table
## VPC
Private subnet
Public subnet
Corporate data center
## CIDR: 10.0.0.0/16
## CIDR: 192.168.0.0/16
AWS S2S VPN is a managed IPSec VPN
A VGW is deployed on
the AWS site
Supports static routes or
BGP peering/routing
A CGW is deployed on the
customer side
Route table points
to the VGW
## Customer
Gateway (CGW)
## Virtual Private
Gateway (VGW)

© Digital Cloud Training | https://digitalcloud.training
AWS Site-to-Site VPN Key Features
Uses IPSec Tunnels –   Creates a secure IPSec VPN tunnel
between AWS and your network
Dual VPN Tunnels for High Availability –   AWS provides
two VPN tunnels to each AWS VPN endpoint for redundancy
Works with Any VPN Device –   Supports third-party VPN
routers that use IKEv1 or IKEv2
Encryption & Security –   Uses AES-256 encryption and
SHA-2 hashing for data protection
Can Connect to AWS Transit Gateway –   Allows multiple
VPCs to share the same VPN connection
Supports BGP or Static Routing – Can use BGP (dynamic
routing) or static routes for routing traffic

© Digital Cloud Training | https://digitalcloud.training
AWS Site-to-Site VPN Limitations
Depends on Internet Latency –   Performance varies
based on internet conditions
Limited Bandwidth –   Maximum bandwidth is 1.25 Gbps
per VPN tunnel
Single TCP Session Limit –   AWS throttles single TCP flows
to 250 Mbps, affecting high-bandwidth applications
Manual Failover Between Tunnels –   If one VPN tunnel
fails, your router must switch to the second tunnel manually
(unless using BGP)
https://docs.aws.amazon.com/vpn/latest/s2svpn/VPC_VPN.html

© Digital Cloud Training | https://digitalcloud.training
AWS VPN CloudHub

© Digital Cloud Training | https://digitalcloud.training
AWS VPN CloudHub
## VPC
Private subnet
Public subnet
## Virtual Private
Gateway (VGW)
Customer office
Customer office
Customer office
Customer gateway
## ASN: 6500
Network traffic
Network traffic
Customer gateway
## ASN: 6501
Customer gateway
## ASN: 6502
A VGW is deployed
on the AWS site
Network traffic may go between a
VPC and a remote office
Network traffic between offices can
also be routed over the IPSec VPN
Each office must use a
unique BGP ASN
Remote offices connect
to the VGW in a hub-
and-spoke model

© Digital Cloud Training | https://digitalcloud.training
AWS Direct Connect (DX)
## Deep Dive

© Digital Cloud Training | https://digitalcloud.training
AWS Direct Connect (DX)
Corporate data center
AWS Direct Connect location
AWS Cloud
AWS cageCustomer /
partner cage
AWS Direct
## Connect
endpoint
## Customer /
partner router
## Region
## Customer
## Router
## VPC
Private subnet
Public subnet
A cross-connect between the AWS DX router
and the customer/partner DX router
DX is a physical fiber
connection to AWS running at
1Gbps, 10Gbps, 100Gbps, or
400Gbps
A DX port must be
allocated in a DX location
The customer router is
connected to the DX
router in the DX location

© Digital Cloud Training | https://digitalcloud.training
AWS Direct Connect Benefits
•Private connectivity between AWS and your
data center / office
•Consistent network experience:
•Increased speed
•Lower latency
•High bandwidth/throughput
•Lower costs for organizations that transfer
large volumes of data

© Digital Cloud Training | https://digitalcloud.training
AWS Direct Connect (DX)
## VPC
Corporate data center
AWS Direct Connect location
AWS Cloud
AWS cageCustomer /
partner cage
## Region
Amazon S3Amazon DynamoDBAmazon CloudFront
Private subnet
Public subnet
AWS Direct
## Connect
endpoint
## Customer /
partner router
## VGW
Private VIF
Public VIF
## Customer
## Router
A VIF is a virtual interface (802.1Q VLAN)
and a BGP session
A Private VIF connects to a
single VPC in the same AWS
Region using a VGW
A Public VIF can be used to connect to AWS Public
services in any Region (but not the Internet)

© Digital Cloud Training | https://digitalcloud.training
AWS Direct Connect (DX)
## VPC
Corporate data center
AWS Direct Connect location
AWS Cloud
AWS cageCustomer /
partner cage
## Region
AWS Direct
## Connect
endpoint
## Customer /
partner router
## VGW
## VPC
## VPC
## VGW
## VGW
## Customer
## Router
Multiple Private VIFs can be used to
connect to multiple VPCs in the Region
VIFs can also be shared with other AWS
accounts – known as hosted VIFs

© Digital Cloud Training | https://digitalcloud.training
AWS Direct Connect (DX)
•Speeds from 50Mbps to 25Gbps can also be
accessed via an APN partner (uses hosted VIFs or
hosted connections):
•A hosted VIF is a single VIF that is shared with other
customers (shared bandwidth)
•A hosted connection is a DX connection with a single
VIF dedicated to you
•DX Connections are NOT encrypted by default
•Use an IPSec S2S VPN connection over a public VIF
or MACsec to add encryption in transit
•Link aggregation groups (LAGs) can be used to
combine multiple physical connections into a
single logical connection using LACP – provides
improved speed

© Digital Cloud Training | https://digitalcloud.training
DX - Native High Availability
Corporate data center
AWS Direct Connect location
## Region
Corporate data center
AWS Direct Connect location
## =
Single Point of Failure
DX Locations are connected
by redundant connections
Multiple DX Locations exist in metropolitan
areas where AWS has Regions
Cables may share the
same pathways

© Digital Cloud Training | https://digitalcloud.training
VPN Backup for Direct Connect
Corporate data center
AWS Direct Connect location
## Region
## Internet
## DX
## VGW
## Requirements:
•Use the same VGW for both DX and the VPN connection to the VPC
•For a BGP VPN, advertise the same prefix for Direct Connect and the VPN
•For a static VPN, add the same static prefixes to the VPN connection that you are
announcing with the DX virtual interface
This architecture is NOT
recommended for speeds
above 1Gbps
Multiple SPOFs exist in this
architecture, add
redundancy to eliminate
The DX connection is the
primary active path
An IPSec S2S VPN is
the backup path

© Digital Cloud Training | https://digitalcloud.training
VPN Backup for Direct Connect
•If the same prefixes are being advertised for DX and
the S2S VPN, the VGW makes routing decisions as
follows (most preferred to least preferred):
•BGP propagated routes from an AWS Direct Connect
connection
•Manually added static routes for a Site-to-Site VPN
connection
•BGP propagated routes from a Site-to-Site VPN
connection
•For matching prefixes where each Site-to-Site VPN
connection uses BGP, the AS PATH is compared and the
prefix with the shortest AS PATH is preferred
•When the AS PATHs are the same length and if the first AS
in the AS_SEQUENCE is the same across multiple paths,
multi-exit discriminators (MEDs) are compared. The path
with the lowest MED value is preferred

© Digital Cloud Training | https://digitalcloud.training
MACsec for Encrypting Direct Connect
•MACsec is the IEEE 802.1AE MAC Security Standard
•MACsec can be used for encrypting part of the AWS
Direct Connect connection
•MACsec runs at L2 and uses GCM-AES-128 to offer
integrity and confidentiality
•MACsec can be used to enable encryption for DX
connections
•Offers near line-rate encryption for high throughput
•MACsec protects links between your customer
router/switch and the DX device

© Digital Cloud Training | https://digitalcloud.training
MACsec for Encrypting Direct Connect
Corporate data center
## Region
## DX
MACsec
## VGW
AWS Direct Connect location
AWS cage
## Customer /
partner cage
AWS Direct
## Connect
endpoint
## Customer /
partner router
MACsec
MACsec provides near line-rate
encryption for maximum throughput
AWS provide a MACsec enabled
port on the DX router
Layer 2 traffic that travels over the
dedicated connection to or from the
data center is encrypted
MACsec is configured between the
customer router or switch and the DX
device

© Digital Cloud Training | https://digitalcloud.training
IPSec VPN for Encrypting Direct Connect
Corporate data center
AWS Direct Connect location
## Region
## DX
## VGW
This solution encrypts from the
data center to the VGW
An IPSec S2S VPN is established over a
public VIF across the DX connection
A VGW is required for
terminating the VPN

© Digital Cloud Training | https://digitalcloud.training
Virtual Interfaces (VIFs)
There are three types of virtual interface (VIF):
•Private virtual interface - used to access an Amazon VPC
using private IP addresses
•Public virtual interface - can access all AWS public services
using public IP addresses
•Transit virtual interface - used to access one or more Amazon
VPC Transit Gateways associated with Direct Connect
gateways
•For public VIFs you can access all AWS prefixes through the
connection such as Amazon EC2, Amazon S3, and
## Amazon.com

© Digital Cloud Training | https://digitalcloud.training
## Network Requirements
•Customer routers must meet specific requirements:
•Use single-mode fiber with compatible optical transceivers
•Support for BGP for routing
•Support for 802.1Q VLAN encapsulation
•Use the correct transceiver for your port speed:
•1 Gbps: 1000BASE-LX (1310 nm)
•10 Gbps: 10GBASE-LR (1310 nm)
•100 Gbps: 100GBASE-LR4
•400 Gbps: 400GBASE-LR4
•For connections with speeds greater than 1 Gbps, auto-
negotiation must be disabled

© Digital Cloud Training | https://digitalcloud.training
## Network Requirements
Routing and BGP requirements:
•BGP support: Your router must support Border Gateway
Protocol (BGP) and BGP MD5 authentication
•ASN: You must have an Autonomous System Number (ASN) to
establish a BGP session. If using a private ASN, it must be in
the 64512 to 65535 range
•Public IP prefixes: For public virtual interfaces, you must own
and advertise the public IP prefixes you intend to use
•BFD: Bidirectional Forwarding Detection (BFD) is optional but
recommended. It is automatically enabled on the virtual
interface side.

© Digital Cloud Training | https://digitalcloud.training
Bidirectional Forwarding Detection (BFD)
•BFD is a detection protocol that provides fast forwarding path
failure detection times for faster reconvergence times
•Without BFD, BGP waits for three keep-alives to fail at a hold-
down time of 90 seconds
•Asynchronous BFD is automatically enabled for Direct
Connect virtual interfaces on the AWS side
•You must configure your router to enable asynchronous BFD
for your connection
•The default AWS BFD liveness detection minimum interval is
300 ms. The default BFD liveness detection multiplier is three

© Digital Cloud Training | https://digitalcloud.training
AWS Direct Connect Gateway

© Digital Cloud Training | https://digitalcloud.training
## Direct Connect Gateway
•Use AWS Direct Connect gateway to connect your VPCs
•A Direct Connect gateway is a globally available resource
•You can create the Direct Connect gateway in any Region
and access it from all other Regions
•You associate an AWS Direct Connect gateway with
either of the following gateways:
•A transit gateway when you have multiple VPCs in
the same Region
•A virtual private gateway

© Digital Cloud Training | https://digitalcloud.training
## Direct Connect - Multiple Regions
Region – us-west-1
DX Location - Europe
Corporate data center
DX Location - US
Region eu-central-1
AWS Cloud
Private VIF
Private VIF
## VGW
## VGW
Example architecture without AWS
## Direct Connect Gateway
A Private VIF connects to a
single VPC in the same AWS
Region using a VGW
DX is a regional service so multiple
DX locations must be used
Requires regional offices
or long distance
(expensive) links

© Digital Cloud Training | https://digitalcloud.training
## Direct Connect - Multiple Regions
Region – us-west-1
Corporate data center
DX Location - US
Region eu-central-1
AWS Cloud
Private VIF
## VGW
## VGW
DX Gateway
Example architecture with AWS Direct
## Connect Gateway
The DX Gateway is
associated with a VGW
A Private VIF is associated
with the DX Gateway
BGP advertises a route to all
VPCs via the DX Gateway

© Digital Cloud Training | https://digitalcloud.training
## Direct Connect - Multiple Regions
Region – us-west-1
Corporate data center
DX Location - US
Region eu-central-1
AWS Cloud
Private VIF
## VGW
## VGW
DX Gateway
Example architecture with AWS Direct
## Connect Gateway
Network traffic
DX Gateway does not
allow VGWs to send
traffic to each other
Network traffic can be routed from on-
premises to any VPC

© Digital Cloud Training | https://digitalcloud.training
## Virtual Private Gateway Associations
•The Direct Connect gateway is associated with the virtual
private gateway (VGW) for the VPC
•Private virtual interfaces (VIFs) are then used to connect
to the Direct Connect gateway
•You can attach multiple private virtual interfaces to your
Direct Connect gateway
•VPCs must not have overlapping CIDR blocks
•Yo u   cannot create a public virtual interface to a Direct
Connect gateway

© Digital Cloud Training | https://digitalcloud.training
## Virtual Private Gateway Associations
The following traffic flows are not supported:
•Direct communication between the VPCs that are
associated with a single DX gateway
•Direct communication between the virtual interfaces
that are attached to a single DX gateway
•Direct communication between the virtual interfaces
that are attached to a single DX gateway and a VPN
connection on a virtual private gateway that's associated
with the same DX gateway
•You cannot associate a virtual private gateway with more
than one DX gateway, and you cannot attach a private
virtual interface to more than one DX gateway

© Digital Cloud Training | https://digitalcloud.training
AWS Transit Gateway Deep Dive

© Digital Cloud Training | https://digitalcloud.training
AWS Transit Gateway
•Simplified connectivity: Transit Gateway simplifies network management
by acting as a central hub that connects VPCs and on-premises networks
•Scalability: It supports thousands of connections, making it more scalable
than VPC peering, which requires individual peering connections
between each pair of VPCs
•Transitive routing: Unlike VPC peering, Transit Gateway allows for
transitive routing, enabling VPCs to communicate with each other
through a single central hub
•Integrated VPN and Direct Connect support: Transit Gateway can be
used with both AWS VPN and AWS Direct Connect, providing a unified
gateway for both cloud and on-premises networks
•Efficient use of route tables: Reduces the number of route table entries
required in each VPC, as VPCs only need to know how to reach the Transit
Gateway, not each other
•Cross-account access: Transit gateways can be shared across accounts
using AWS RAM

© Digital Cloud Training | https://digitalcloud.training
AWS Transit Gateway
## VPC AVPC B
## VPC C
## VPC D
## CGW
Corporate office
## Subnet
## Subnet
## Subnet
## Subnet
## Subnet
## Subnet
## Subnet
## Subnet
TGWs can be attached to VPNs, Direct
## Connect Gateways, 3
rd
party appliances
and TGWs in other Regions/accounts
Specify one subnet
from each AZ to enable
routing within the AZ
VPCs are attached to
## Transit Gateway

© Digital Cloud Training | https://digitalcloud.training
AWS Transit Gateway
## VPC AVPC B
## VPC C
## VPC D
Example full mesh architecture without
AWS Transit Gateway
IPSec VPN
IPSec VPN
IPSec VPN
IPSec VPN
## CGW
## VGW
## VGW
## VGW
## VGW
Corporate office
6 VPC Peering
connections
## 4 S2S VPN
connections
To make this architecture
redundant add another CGW
and double the number of
S2S VPN connections!

© Digital Cloud Training | https://digitalcloud.training
AWS Transit Gateway
## VPC AVPC B
## VPC C
## VPC D
Example full mesh architecture with
AWS Transit Gateway
## CGW
Corporate office
## Subnet
## Subnet
## Subnet
## Subnet
## Subnet
## Subnet
## Subnet
## Subnet
Specify one subnet from
each AZ to enable
routing within the AZ
Transit Gateway is a network
transit hub that interconnects
VPCs and on-premises
networks
VPCs are attached to
## Transit Gateway
TGWs can be attached to VPNs,
## Direct Connect Gateways, 3
rd
party
appliances and TGWs in other
## Regions/accounts

© Digital Cloud Training | https://digitalcloud.training
AWS TGW + DX Gateway
## VPC AVPC B
## VPC C
## VPC D
This architecture supports full transitive
routing between on-premises, TGW and VPCs
Corporate office
## Subnet
## Subnet
## Subnet
## Subnet
## Subnet
## Subnet
## Subnet
## Subnet
AWS cage
## Customer /
partner cage
AWS Direct
## Connect
endpoint
## Customer /
partner router
Transit VIF
## Customer
## Router
DX Gateway
DX Gateway is
associated with the TGW
A Transit VIF is used when attaching
via a DX Gateway to a TGW

© Digital Cloud Training | https://digitalcloud.training
Isolated VPCs and Shared Services Architecture
## VPC A
## Data Center
## Customer
## Gateway
## VPC B
## VPC C
## VPC D
(shared services)
## 10.1.0.0/16
## 10.2.0.0/16
## 10.3.0.0/16
## 10.4.0.0/16
## S2S VPN
## 10.99.99.0/24
DestinationTa rgetRoute type
10.99.99.0/24VPN attachmentpropagated
10.4.0.0/16VPC D attachmentpropagated
DestinationTa rget
## 10.1.0.0/16local
## 0.0.0.0/0tgw-id
TGW RT1 – Associated with VPC A, B, and C
VPC A Route Table
DestinationTa rgetRoute type
10.1.0.0/16VPC A attachmentpropagated
10.2.0.0/16VPC B attachmentpropagated
10.3.0.0/16VPC C attachmentpropagated
10.4.0.0/16VPC D attachmentpropagated
TGW RT2 - Associated with VPN and VPC D
The route tables for VPC
A, B, C, and D will have
similar routes
VPC A, B, C, can
communicate with VPC
D but not with each
other
Transit GW functions as
multiple isolated routers

© Digital Cloud Training | https://digitalcloud.training
Isolated VPCs and Shared Services Architecture
## VPC A
## Data Center
## Customer
## Gateway
## VPC B
## VPC C
## VPC D
(shared services)
## 10.1.0.0/16
## 10.2.0.0/16
## 10.3.0.0/16
## 10.4.0.0/16
## S2S VPN
## 10.99.99.0/24
DestinationTa rgetRoute type
10.99.99.0/24VPN attachmentpropagated
10.4.0.0/16VPC D attachmentpropagated
DestinationTa rget
## 10.1.0.0/16local
## 0.0.0.0/0tgw-id
TGW RT1 – Associated with VPC A, B, and C
VPC A Route Table
TGW RT2 - Associated with VPN and VPC D
Attachments associated with one isolated router can route
packets to each other, but cannot route packets to or receive
packets from the attachments for another isolated router
Transit GW functions as
multiple isolated routers
VPC A, B, C, can
communicate with VPC
D but not with each
other
DestinationTa rgetRoute type
10.1.0.0/16VPC A attachmentpropagated
10.2.0.0/16VPC B attachmentpropagated
10.3.0.0/16VPC C attachmentpropagated
10.4.0.0/16VPC D attachmentpropagated

© Digital Cloud Training | https://digitalcloud.training
Transit Gateway Connect and SD-WAN
•SD-WAN is a system that connects branch sites over
the internet using smart routing, picking the best
path based on performance
•It replaces or supplements MPLS by using multiple
links (internet, LTE, fiber) with automatic failover
•SD-WAN appliances apply traffic policies, monitor link
health, and steer apps over the best path
•In AWS, you deploy a virtual SD-WAN appliance inside
a VPC to act as the cloud endpoint
•That appliance connects to AWS Transit Gateway
Connect using GRE tunnels and BGP
•Transit Gateway then shares routes between SD-WAN
branches and all connected AWS VPCs

© Digital Cloud Training | https://digitalcloud.training
## Multicast Routing
•Transit gateway supports multicast routing between
subnets of attached VPCs
•TGW routes traffic for instances sending to multiple
receiving instances
•Multicast domain membership is defined at the subnet
level
•Multicast groups identify hosts that send and receive
multicast traffic by groups of IP addresses
•Multicast group membership is defined by individual ENI
•Internet Group Management Protocol (IGMP) is used for
managing multicast group membership
•Multicast routing is not supported over AWS Direct
Connect, Site-to -Site VPN, or peering attachments

© Digital Cloud Training | https://digitalcloud.training
•You can monitor with Amazon CloudWatch:
•Transit gateway metrics (AWS/TransitGateway)
•Attachment-level metrics
•Amazon VPC Flow Logs to capture information on
the IP traffic routed through the TGW
•AWS Transit Gateway Network Manager enables
global monitoring for AWS and on-premises
•Centralized Network Monitoring – including alerting on
changes to topology, routing, and connection status
•Global Network Visibility – visualize your entire global
network
•SD-WAN Integration – seamless integration with SD-WAN
solutions from from Cisco, Aruba, Silver Peak, Aviatrix,
and Versa Networks
## Transit Gateway Monitoring

© Digital Cloud Training | https://digitalcloud.training
•Use a separate subnet for each transit gateway VPC
attachment
•Create one network ACL and associate it with all the
subnets that are associated with the transit gateway
•Associate the same VPC route table with all subnets
that are associated with the transit gateway, unless your
network design requires multiple VPC route tables
•Enable route propagation for AWS Direct Connect
gateway attachments and BGP Site-to-Site VPN
attachments
•More here:
https://docs.aws.amazon.com/vpc/latest/tgw/tgw-best-
design-practices.html
## Transit Gateway Best Practices

© Digital Cloud Training | https://digitalcloud.training
Using IPv6 in a VPC

© Digital Cloud Training | https://digitalcloud.training
Using IPv6 in a VPC
## 192
## ...
## 16801
## 11000000
## 10101000
Public IPv4 addresses are
close to being exhausted
and N AT must be used
extensively
IPv4 provides approximately 4.3 billon addresses
## 00000000
## 00000001
An IPv4 address is 32 bits long

© Digital Cloud Training | https://digitalcloud.training
Using IPv6 in a VPC
## 202000015bc21c4832c1b12ca93b9d32:::::::
IPv6 provides 340,282,366,920,938,463,463,374,607,431,768,211,456
addresses
## Network Part
## Node Part
That’s enough to assign more than
100 IPv6 addresses to every atom
on earth!!!
An IPv6 address is 128 bits long
An IPv6 addresses use
hexadecimal whereas IPv4
addresses use dotted decimal

© Digital Cloud Training | https://digitalcloud.training
Using IPv6 in a VPC
## VPC
Public subnet
Public subnet
IPv4 CIDR 10.0.0.0/16
## 10.0.0.0/20
## 10.0.16.0/20
DestinationTa rget
10.0.0.0/16Local
2406:da1c:f7b:ae00::/56Local
## 0.0.0.0/0igw-id
## ::/0igw-id
## Route Table
IPv6 CIDR 2406:da1c:f7b:ae00::/56
## 2406:da1c:f7b:ae11::/64
## 2406:da1c:f7b:ae10::/64
AWS assign a /56 IPv6
address range to your VPC
Subnets receive a /64
address range allowing 18
million trillion addresses
All IPv6 addresses are
publicly routable (no NAT)
A hexadecimal pair is  assigned for
each subnet – values from 00 – FF =
256 /64 subnets
Route table has an entry to
send all external IPv6
traffic to the IGW

© Digital Cloud Training | https://digitalcloud.training
Using IPv6 in a VPC
## VPC
Public subnet
Public subnet
IPv4 CIDR 10.0.0.0/16
## 10.0.0.0/20
## 10.0.16.0/20
IPv6 CIDR 2406:da1c:f7b:ae00::/56
## 2406:da1c:f7b:ae11::/64
## 2406:da1c:f7b:ae10::/64
An Egress-only Internet Gateway allows
IPv6 traffic outbound but not inbound
DestinationTa rget
172.31.0.0/16Local
## 0.0.0.0/0igw-id
## ::/0eo-igw-id
## Route Table
An Egress-only is    necessary only
if you want outbound-only IPv6
(similar to NAT gateway)

© Digital Cloud Training | https://digitalcloud.training
VPC Flow Logs

© Digital Cloud Training | https://digitalcloud.training
VPC Flow Logs
## VPC
Private subnet
Public subnet
Flow logs
Flow logs
EC2 Instance
Flow logs
•Flow Logs capture information about the
IP traffic going to and from network
interfaces in a VPC
•Flow log data is stored using Amazon
CloudWatch Logs or S3
•Flow logs can be created at the following
levels:
## •VPC
•Subnet
•Network interface

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns –
Amazon VPC

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – Amazon VPC
An Amazon S3 bucket must only allow
access from EC2 instances in a private
subnet using private IPs
Create a VPC endpoint and configure a
bucket policy that restricts access to the
VPC endpoint ID using the Condition
element
Malicious traffic is reaching some EC2
instances in a public subnet from a few
identified public IP addresses
Use a Network ACL to deny access
based on the source IP addresses
A company wants to connect their on-
premises data center to AWS and
requires consistent performance and
encryption
Create an AWS Direct Connect
connection and run an AWS S2S VPN
over the DX connection to enable
encryption
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – Amazon VPC
A company requires private
connectivity between VPCs in different
Regions will full redundancy
Create VPC peering connections
between the VPCs
Several remote office locations should
be connected to an Amazon VPC and
to each other over the internet with
full encryption
Create VPG and attach multiple remote
locations in a hub and spoke topology
using AWS CloudHub
Microservices app requires instance-
level firewall with different rules per
application component
Create separate security groups for
each application component and
configure the appropriate rules
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – Amazon VPC
A company is using IPv6 addresses with
Amazon EC2 and needs to enable
outbound internet connectivity
Configure an egress-only Internet
## Gateway
Subnet must be configured that allows
internet connectivity using IPv4 with
auto-address assignment
Attach an internet gateway to the VPC
and update the route table for the new
subnet. Enable the auto-assign public
IPv4 setting for the subnet
An on-premises data center needs to
establish S2S VPN connections to
several VPCs in a full mesh architecture
Deploy an AWS Transit Gateway and
attach the VPN connection from on-
premises and each VPC
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## SECTION 7
Amazon Simple Storage Service (S3)

© Digital Cloud Training | https://digitalcloud.training
## Amazon Simple Storage
Service (S3)

© Digital Cloud Training | https://digitalcloud.training
Amazon Simple Storage Service (S3)
## S3 Bucket
## Object
## Object
## Object
https://bucket.s3.aws-region.amazonaws.com/key
https://s3.aws-region.amazonaws.com/bucket/key
Accessing objects in a bucket:
A bucket is a
container for
objects
An object is a
file you upload
You can store
millions of objects
in a bucket
The HTTP protocol is used with a
REST API (e.g. GET, PUT, POST,
## SELECT, DELETE)

© Digital Cloud Training | https://digitalcloud.training
Amazon Simple Storage Service (S3)
## VPC
Private subnet
Public subnet
EC2 Instance
## S3 Gateway Endpoint
## Amazon S3
## Internet
gateway
## Internet Client
## Public Internet
http://bucket.s3.aws  -region.amazonaws.com
## Bucket
## Object
An objects consists of:
•Key (name of objects)
•Version ID
•Value (actual data)
•Metadata
•Subresources
•Access control information
http://s3.aws  -region.amazonaws.com/bucket
EC2 Instance
A bucket is a container
for objects
EC2 instances
connect using
public addresses
EC2 instances connect using
private addresses

© Digital Cloud Training | https://digitalcloud.training
File Storage vs Object Storage
## File Share
•Data stored in directories
•A hierarchy of directories can be formed
•File systems are mounted to an operating system
•Function like local storage
•Network connection is maintained
•Example is Amazon EFS
## Object Store
•Data stored in buckets
•Flat namespace (no hierarchy)
•Hierarchy can be mimicked with prefixes
•Accessed by REST API and cannot be mounted
•Network connection is completed after each
request
•Example is Amazon S3
http://bucket.s3.aws-region.amazonaws.com

© Digital Cloud Training | https://digitalcloud.training
## Amazon S3 Storage Classes

© Digital Cloud Training | https://digitalcloud.training
Durability and Availability in S3
If you store 10 million objects, then
you expect to lose one object every
10,000 years!
Availability is a measurement
of:
•The amount of time the
data is available to you
•Expressed as a percent of
time per year
•E.g. 99.99%
Durability is protection
against:
•Data loss
•Data corruption
•S3 offers 11 9s durability
## (99.999999999)
DurabilityAvailability

© Digital Cloud Training | https://digitalcloud.training
## S3 Storage Classes
S3 StandardS3 Intelligent
## Tiering
S3 Standard-IAS3 One Zone-IAS3 Glacier
## Instant Retrieval
## S3 Glacier Flexible
## Retrieval
## S3 Glacier Deep
## Archive
Designed for
durability
99.999999999%99.999999999%99.999999999%99.999999999%99.999999999%99.999999999%99.999999999%
Designed for
availability
## 99.99%99.9%99.9%99.5%99.9%99.99%99.99%
Availability SLA99.9%99%99%99%99%99.9%99.9%
## Availability Zones≥3≥3≥31≥3≥3≥3
Minimum capacity
charge per object
## N/AN/A128KB128KB128KB40KB40KB
Minimum storage
duration charge
N/AN/A30 days30 days90 days90 days180 days
Retrieval feeN/AN/APer GB retrievedPer GB retrievedPer GB retrievedPer GB retrievedPer GB retrieved
First byte latencymillisecondsmillisecondsmillisecondsmillisecondsmillisecondsminutes or hourshours
Storage typeObjectObjectObjectObjectObjectObjectObject
Lifecycle transitionsYe sYe sYe sYe sYe sYe sYe s

© Digital Cloud Training | https://digitalcloud.training
Working with S3 Buckets
and Objects

© Digital Cloud Training | https://digitalcloud.training
IAM Policies, Bucket Policies
and ACLs

© Digital Cloud Training | https://digitalcloud.training
IAM Policies
•IAM Policies are identity-based policies
•Specify what actions are allowed on what
AWS resources
## User
## Group
## Role
IAM Policies are attached
to IAM users, groups, or
roles
The Principal element is
not required in the policy
IAM Policies are written
in JSON using the AWS
access policy language

© Digital Cloud Training | https://digitalcloud.training
## Bucket Policies
•Bucket Policies are resource-based policies
•Can only be attached to Amazon S3 buckets
•Also use the AWS access policy language
## S3 Bucket
## Paul
s3:PutObject

© Digital Cloud Training | https://digitalcloud.training
S3 Access Control Lists (ACLs)
•Legacy access control mechanism that predates
## IAM
•AWS generally recommends using S3 bucket
policies or IAM policies rather than ACLs
•Can be attached to a bucket or directly to an
object
•Limited options for grantees and permissions

© Digital Cloud Training | https://digitalcloud.training
When to use each access control mechanism
•Use IAM policies if:
•You need to control access to AWS services other than S3
•You have numerous S3 buckets each with different
permissions requirements (IAM policies will be easier to
manage)
•You prefer to keep access control policies in the IAM
environment
•Use S3 bucket policies if:
•You want a simple way to grant cross-account access to
your S3 environment, without using IAM roles
•Your IAM policies are reaching the size limits
•You prefer to keep access control policies in the S3
environment

© Digital Cloud Training | https://digitalcloud.training
## Authorization Process
## Decision
starts at
deny
## Evaluate
all
policies
## Explicit
deny?
Is there
an
allow?
Final decision =
allow (explicit
allow)
Final decision
= deny
(explicit deny)
Final decision
= deny
(default deny)
Ye sYe s
## No
## No

© Digital Cloud Training | https://digitalcloud.training
S3 Permissions and Bucket
## Policies

© Digital Cloud Training | https://digitalcloud.training
## S3 Versioning, Replication
and Lifecycle Rules

© Digital Cloud Training | https://digitalcloud.training
## Amazon S3 Versioning
•Versioning is a means of keeping multiple variants
of an object in the same bucket
•Use versioning to preserve, retrieve, and restore
every version of every object stored in your
Amazon S3 bucket
•Versioning-enabled buckets enable you to recover
objects from accidental deletion or overwrite

© Digital Cloud Training | https://digitalcloud.training
## Amazon S3 Replication
## Region
## Region
## Region
BucketBucket
BucketBucket
Cross-Region Replication (CRR)
Same-Region Replication (SRR)
Buckets must have versioning enabled

© Digital Cloud Training | https://digitalcloud.training
## S3 Lifecycle Management
There are two types of actions:
•Transition actions - Define when objects transition
to another storage class
•Expiration actions - Define when objects expire
(deleted by S3)

© Digital Cloud Training | https://digitalcloud.training
S3 LM: Supported Transitions
https://docs.aws.amazon.com/AmazonS3/latest/userguide/lifecycle-transition-
general-considerations.html

© Digital Cloud Training | https://digitalcloud.training
Configure Replication and
## Lifecycle

© Digital Cloud Training | https://digitalcloud.training
MFA with Amazon S3

© Digital Cloud Training | https://digitalcloud.training
S3 Multi-Factor Authentication Delete (MFA Delete)
•Adds MFA requirement for bucket owners to the
following operations:
•Changing the versioning state of a bucket
•Permanently deleting an object version
•The x-amz-mfa request header must be included in the
above requests
•The second factor is a token generated by a hardware
device or software program
•Requires versioning to be enabled on the bucket

© Digital Cloud Training | https://digitalcloud.training
S3 Multi-Factor Authentication Delete (MFA Delete)
•Versioning can be enabled by:
•Bucket owners (root account)
•AWS account that created the bucket
•Authorized IAM users
•MFA delete can be enabled by:
•Bucket owner (root account)

© Digital Cloud Training | https://digitalcloud.training
MFA-Protected API Access
•Used to enforce another authentication factor (MFA code) when
accessing AWS resources (not just S3)
•Enforced using the aws:MultiFactorAuthAge key in a bucket policy:
Denies any API operation
that is not authenticated
using MFA

© Digital Cloud Training | https://digitalcloud.training
## Amazon S3 Encryption

© Digital Cloud Training | https://digitalcloud.training
## Amazon S3 Encryption
Server-side encryption with S3
managed keys (SSE-S3)
Server-side encryption with AWS
KMS managed keys (SSE-KMS)
## Encryption /
decryption
## Encryption /
decryption
•S3 managed keys
•Unique object keys
•Master key
## •AES 256
•KMS managed keys
•Can be AWS managed keys
•Or customer managed KMS
keys
## User
## User

© Digital Cloud Training | https://digitalcloud.training
## Amazon S3 Encryption
Server-side encryption with
client provided keys (SSE-C)
Client-side encryption
## Encryption /
decryption
•Client managed keys
•Not stored on AWS
•Client managed keys
•Not stored on AWS
•Or you can use a KMS Key
## User
## User
## Encryption /
decryption

© Digital Cloud Training | https://digitalcloud.training
## Amazon S3 Default Encryption
•All Amazon S3 buckets have encryption configured by default
•All new object uploads to Amazon S3 are automatically
encrypted
•There is no additional cost and no impact on performance
•Objects are automatically encrypted by using server-side
encryption with Amazon S3 managed keys (SSE-S3)
•To encrypt existing unencrypted Amazon S3 objects, you can use
## Amazon S3 Batch Operations
•You can also encrypt existing objects by using the CopyObject API
operation or the copy-object AWS CLI command

© Digital Cloud Training | https://digitalcloud.training
Enforce Encryption with Bucket Policy
Example PUT request
Enforces encryption
using SSE-KMS

© Digital Cloud Training | https://digitalcloud.training
## Enforce Encryption
with AWS KMS

© Digital Cloud Training | https://digitalcloud.training
Enforce Encryption with Bucket Policy
Example PUT request
Enforces encryption
using SSE-KMS

© Digital Cloud Training | https://digitalcloud.training
## S3 Event Notifications

© Digital Cloud Training | https://digitalcloud.training
## S3 Event Notifications
•Sends notifications when events happen in
buckets
•Destinations include:
•Amazon Simple Notification Service (SNS)
topics
•Amazon Simple Queue Service (SQS) queues
•AWS Lambda functions

© Digital Cloud Training | https://digitalcloud.training
S3 Presigned URLs

© Digital Cloud Training | https://digitalcloud.training
S3 Presigned URLs
aws s3 presign s3://dct-data-bucket/presigned_index.html
https://mywebsite-3eqd2a.s3.us-east-1.amazonaws.com/index.html?X-Amz-
Algorithm=AWS4-HMAC-SHA256&X-Amz-
Credential=ASIA6GBMFBGVJIKXMWWK%2F20240322%2Fus-east-
1%2Fs3%2Faws4_request&X-Amz-

© Digital Cloud Training | https://digitalcloud.training
## Multipart Upload &
## Transfer Acceleration

© Digital Cloud Training | https://digitalcloud.training
## S3 Multipart Upload
•Multipart upload uploads objects in parts
independently, in parallel and in any order
•Performed using the S3 Multipart upload API
•It is recommended for objects of 100 MB or larger
•Can be used for objects from 5 MB up to 5 TB
•Must be used for objects larger than 5 GB

© Digital Cloud Training | https://digitalcloud.training
S3 Multipart Upload with the AWS CLI
You can use the AWS CLI to perform a multipart upload to S3:
Then, upload each part of the file using the following command:
Upload additional parts using the same command with different part numbers,
and then complete the multipart upload using the following command:
Use the list-parts command to list the parts uploaded for a specific multipart upload:

© Digital Cloud Training | https://digitalcloud.training
S3 Multipart Upload with Boto3
This example uses the boto3
library for Python

© Digital Cloud Training | https://digitalcloud.training
S3 Transfer Acceleration (S3TA)
•Uses CloudFront edge locations to improve
performance of transfers from client to S3 bucket
## Bucket
http://bucketname.s3  -accelerate.amazonaws.com
http://bucketname.s3  -accelerate.dualstack.amazonaws.com
CloudFront Edge location
## Application
Transfer Acceleration is
enabled at the bucket level
AWS only charges if there’s a
performance improvement

© Digital Cloud Training | https://digitalcloud.training
S3 Transfer Acceleration (S3TA)
•Speeds transfers by 50-500%
•Moves data faster over long distances
•Must be enabled in the bucket properties

© Digital Cloud Training | https://digitalcloud.training
S3 Transfer Acceleration (S3TA)
•Use the speed comparison tool to check if it’s
worth the cost:

© Digital Cloud Training | https://digitalcloud.training
S3 Select and Glacier Select

© Digital Cloud Training | https://digitalcloud.training
S3 Select and Glacier Select
## S3 Bucket
AWS Lambda
Expression= "select * from s3object s where ... "
AWS Lambda
"Expression": "SELECT * FROM archive"
## Archive
SQL expression to retrieve
individual file from zip archive
Single file is retrieved
Single file is retrieved

© Digital Cloud Training | https://digitalcloud.training
## Server Access Logging

© Digital Cloud Training | https://digitalcloud.training
## Server Access Logging
•Provides detailed records for the requests that are made to a
bucket
•Details include the requester, bucket name, request time,
request action, response status, and error code (if applicable)
•Disabled by default
•Only pay for the storage space used
•Must configure a separate bucket as the destination (can specify
a prefix)
•Must grant write permissions to the Amazon S3 Log Delivery
group on destination bucket

© Digital Cloud Training | https://digitalcloud.training
Create an Amazon S3
## Static Website

© Digital Cloud Training | https://digitalcloud.training
Cross-Origin Resource
Sharing (CORS)

© Digital Cloud Training | https://digitalcloud.training
CORS with Amazon S3
•Allows requests from an origin to another origin
•Origin is defined by DNS name, protocol, and port
## Browser
S3 BucketS3 Bucket
Bucket configured
as a website for
mycompany.com
Connect to http://mycompany.com
(the origin)
Bucket holding web
font assets
Connect to S3 endpoint
Preflight request checks
if allowed to make a
request
JavaScript web
client loaded
CORS configuration
must be added to
allow requests from
the other origin

© Digital Cloud Training | https://digitalcloud.training
CORS with Amazon S3
•Enabled through setting:
•Access-Control-Allow-Origin
•Access-Control-Allow-Methods
•Access-Control-Allow-Headers
•These settings are defined using rules
•Rules are added using JSON files in S3

© Digital Cloud Training | https://digitalcloud.training
Example CORS Rule

© Digital Cloud Training | https://digitalcloud.training
Cross-Account Access

© Digital Cloud Training | https://digitalcloud.training
Cross Account Access (IAM Role)
## S3 Bucket
## Account A
## Role
## Account B
sts:AssumeRole
with external ID
## User
## Permissions
## Policy
## Trust
## Policy
The trust policy condition
requires the external ID
Allows access to
the bucket
CLI command will include
the external ID

© Digital Cloud Training | https://digitalcloud.training
## S3 Object Lambda

© Digital Cloud Training | https://digitalcloud.training
## S3 Object Lambda
## Amazon S3
## S3 Object Lambda
## Access Point
Lambda FunctionS3 Access Point
GetObject requests trigger Lambda to process and modify
data before returning it to the application
•S3 Object Lambda uses Lambda functions to process
the output of S3 GET requests
•You can use your own functions or use the AWS pre-
built functions
GetObject

© Digital Cloud Training | https://digitalcloud.training
## S3 Object Lambda – Prebuilt Functions
•Prebuilt Lambda functions that detect personally identifiable
information (PII)
•PII includes names, addresses, dates, credit card numbers, and social
security numbers
•Prebuilt functions include:
•PII Access Control – detects PII and restricts access
•PII Redaction – detects PII and returns documents with the PII
redacted
•Decompression – decrypts objects compressed with bzip2, gzip,
snappy, zlib,  zstandard and ZIP

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns –
## Amazon S3

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns – Amazon S3
Company is concerned about
accidental deletion of Amazon S3
objects
Enable S3 versioning
Data stored in S3 is frequently
accessed for 30 days then is rarely
accessed but must be immediately
retrievable
Use a lifecycle policy to transition
objects from S3 standard to S3
Standard-IA after 30 days
A backup of S3 objects within a specific
folder in a bucket must be replicated to
another Region
Configure cross-region replication and
specify the folder name as a prefix
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns – Amazon S3
Previous versions of objects in a
versioning-enabled S3 bucket must be
stored long term at the lowest cost
Create a lifecycle rule that transitions
previous versions to S3 Glacier Deep
## Archive
A company wishes to manage all
encryption of S3 objects through their
application with their own encryption
keys
Use client-side encryption with client
managed keys
Unencrypted objects in an Amazon S3
bucket must be encrypted
Re-upload the objects and specify the
encryption an encryption key
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns – Amazon S3
An administrator requires a notification
when objects are deleted from an
Amazon S3 bucket
Configure an event notification that
uses the SNS service
A group of customers without AWS
credentials must be granted time-
limited access to a software update
that is stored in an Amazon S3 bucket
Generate a presigned URL
Solutions architects require both
programmatic and console access
across AWS accounts
Configure cross-account access using
IAM roles
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## SECTION 8
DNS, Caching, and Performance
## Optimization

© Digital Cloud Training | https://digitalcloud.training
DNS and Amazon Route 53

© Digital Cloud Training | https://digitalcloud.training
The Domain Name System (DNS)
User enters website
address in browser
DNS Server
NameTypeValue
mycompany.localA192.168.0.1
emailserver.localA192.168.0.2
## Web Server
Computer connects to
## 192.168.0.1
Domain name is resolved to the
IP address of the webserver

© Digital Cloud Training | https://digitalcloud.training
## Amazon Route 53
## Amazon Route 53
example.com
## Availability Zone
Public subnet
## Region
## VPC
## Web Server
## (8.1.2.1)
What’s the IP address
for example.com?
Address is 8.1.2.1
HTTP GET to IP address (8.1.2.1)
A hosted zone represents a set of
records belonging to a domain

© Digital Cloud Training | https://digitalcloud.training
## Amazon Route 53 Routing Policies
Routing PolicyWhat it does
SimpleSimple DNS response providing the IP address associated with a name
FailoverIf primary is down (based on health checks), routes to secondary destination
GeolocationUses geographic location you’re in (e.g. Europe) to route you to the closest
region
GeoproximityRoutes you to the closest region within a geographic area
LatencyDirects you based on the lowest latency route to resources
Multivalue answerReturns several IP addresses and functions as a basic load balancer
WeightedUses the relative weights assigned to resources to determine which to route to
IP-BasedUses the IP addresses of clients to make routing decisions

© Digital Cloud Training | https://digitalcloud.training
## Amazon Route Features
## Amazon Route 53
Hosted zone
example.com
dctlabs.com
EC2 Instances
## Health
## Checks
## Domain
## Registration
## .net
## .com
## .org
## Traffic Flow

© Digital Cloud Training | https://digitalcloud.training
Register Domain with Route
53 (Optional)

© Digital Cloud Training | https://digitalcloud.training
DNS and Amazon Route 53

© Digital Cloud Training | https://digitalcloud.training
## The Domain Name System
## Web Server
## 52.134.26.12
http://dctlabs.com
DNS Server
NameTypeValue
dctlabs.comA52.134.26.12
www.dctlabs.comA52.134.26.12
DNS Zone File
IP addresses are the
addresses computers
use to communicate
Connection is made
using IP address
What’s the IP address
for dctlabs.com?

© Digital Cloud Training | https://digitalcloud.training
Fully Qualified Domain Names (FQDNs)
www
## .
example
## .
com
## .
The root domain is represented by a
“.” And is not usually visible in a DNS
name
com is an example of
a   To p-Level Domain
www is a hostname within
the example subdomain
Example is a subdomain

© Digital Cloud Training | https://digitalcloud.training
## Subdomains
support
## .
amazon
## .
com
## .
support is a subdomain
of amazon.com
mail
## .
google
## .
com
## .
mail is a subdomain
of google.com
A subdomain is subdivision of a
domain name for organizing a set
of related resources or services

© Digital Cloud Training | https://digitalcloud.training
DNS Zones and Records
Record TypeDescription
AMaps a domain name to an IP address (e.g. dctlabs.com to 52.23.21.43)
CNAMEMaps a domain name to another domain name (e.g. mail.dctlabs.com to mailserver1.net)
MXReturns the mail servers for a domain name
TXT Associates text with a domain name (used for verification, authorization etc.)
SRVMaps a domain name to a specific service or protocol (e.g. a Kerberos server)
NS Specifies the authoritative DNS servers for a particular domain
SOAStart of Authority record stores important information about the domain

© Digital Cloud Training | https://digitalcloud.training
## Amazon Route 53
## Amazon Route 53
Hosted zone
example.com
dctlabs.com
EC2 Instances
## Health Checks
## Domain Registration
## .net
## .com
## .org
## Traffic Flow

© Digital Cloud Training | https://digitalcloud.training
DNS Resolution with Route 53
## Amazon Route 53
example.com
## Availability Zone
Public subnet
## Region
## VPC
## Web Server:
## 8.1.2.1
What’s the address
for example.com?
Address is 8.1.2.1
HTTP GET to 8.1.2.1
A hosted zone represents a set of
records belonging to a domain

© Digital Cloud Training | https://digitalcloud.training
## Route 53 Routing Policies
Routing PolicyWhat it does
SimpleSimple DNS response providing the IP address associated with a name
FailoverIf primary is down (based on health checks), routes to secondary destination
GeolocationUses geographic location client is in (e.g. Europe) to route to the closest region
GeoproximityRoutes to the closest region within a geographic area
LatencyDirects based on the lowest latency route to resources
Multivalue answerReturns several IP addresses and functions as a basic load balancer
WeightedUses the relative weights assigned to resources
IP BasedRoute based on the originating IP address of the traffic

© Digital Cloud Training | https://digitalcloud.training
## Route 53 Routing Policies

© Digital Cloud Training | https://digitalcloud.training
## Amazon Route 53 Routing Policies
Routing PolicyWhat it does
SimpleSimple DNS response providing the IP address associated with a name
FailoverIf primary is down (based on health checks), routes to secondary destination
GeolocationUses geographic location you’re in (e.g. Europe) to route you to the closest
region
GeoproximityRoutes you to the closest region within a geographic area
LatencyDirects you based on the lowest latency route to resources
Multivalue answerReturns several IP addresses and functions as a basic load balancer
WeightedUses the relative weights assigned to resources to determine which to route to
IP-BasedUses the IP addresses of clients to make routing decisions

© Digital Cloud Training | https://digitalcloud.training
## Amazon Route 53 – Simple Routing Policy
## Amazon Route 53
DNS query
NameTypeValueTTL
simple.dctlabs.comA1.1.1.1
## 2.2.2.2
## 60
simple2.dctlabs.comA3.3.3.360
## Region
## 1
## 2
## 3

© Digital Cloud Training | https://digitalcloud.training
## Amazon Route 53 – Weighted Routing Policy
## Amazon Route 53
DNS query
NameTypeValueHealthWeight
weighted.dctlabs.comA1.1.1.1ID60
weighted.dctlabs.comA2.2.2.2ID20
weighted.dctlabs.comA3.3.3.3ID20
## Region
## 1
## 2
## 3
## Region
## 1.1.1.1
## 2.2.2.2
## 3.3.3.3
## 60%
## 20%
## 20%
## Optional
## Health Checks
Simplified values - actually
uses an integer between 0
and 255

© Digital Cloud Training | https://digitalcloud.training
## Amazon Route 53 – Latency Routing Policy
## Amazon Route 53
DNS query
NameTypeValueHealthRegion
latency.dctlabs.comA1.1.1.1IDap-southeast-1
latency.dctlabs.comA2.2.2.2IDus-east-1
latency.dctlabs.comAalb-idIDap-southeast-2
Region – ap-
southeast-2
Region – us-east-1
## Optional
## Health Checks
Region – ap-
southeast-1
## 1.1.1.1
## 2.2.2.2
## Singapore
N ew   Yo r k
## Sydney
DNS query
DNS query
## ALB

© Digital Cloud Training | https://digitalcloud.training
## Amazon Route 53 – Failover Routing Policy
## Amazon Route 53
NameTypeValueHealthRecord Type
failover.dctlabs.comA1.1.1.1IDPrimary
failover.dctlabs.comAalb-idSecondary
Region – ap-
southeast-2
Region – us-east-1
## 1.1.1.1
DNS query
## ALB
Health check is
required on Primary
ap-southeast-2 is the
secondary Region

© Digital Cloud Training | https://digitalcloud.training
## Amazon Route 53 – Geolocation Routing Policy
## Amazon Route 53
NameTypeValueHealthGeolocation
geolocation.dctlabs.comA1.1.1.1IDSingapore
geolocation.dctlabs.comA2.2.2.2IDDefault
geolocation.dctlabs.comAalb-idIDOceania
Region – ap-southeast-2
Region – us-east-1
## Optional Health
## Checks
## 2.2.2.2
## Mexico
## New Zealand
DNS query
DNS query
## ALB

© Digital Cloud Training | https://digitalcloud.training
## Amazon Route 53 – Multivalue Routing Policy
## Amazon Route 53
DNS query
## Region
## 1
## 2
## 3
NameTypeValueHealthMulti Value
multivalue.dctlabs.comA1.1.1.1IDYes
multivalue.dctlabs.comA2.2.2.2IDYes
multivalue.dctlabs.comA3.3.3.3IDYes
Health Checks: returns
healthy records only

© Digital Cloud Training | https://digitalcloud.training
## Amazon Route 53 – Geoproximity Routing Policy
Must create a policy in Traffic Flow
Endpoints include
CloudFront, Elastic
Beanstalk, ELB, S3, and
IP addresses

© Digital Cloud Training | https://digitalcloud.training
Amazon Route 53 – IP-Based Routing Policy
CIDR collections are used to
define IP addresses and
CIDR blocks
Routing rules can then be created
to route based on a CIDR collection

© Digital Cloud Training | https://digitalcloud.training
## Failover Routing Policy
with ALB

© Digital Cloud Training | https://digitalcloud.training
## Amazon Route 53 Resolver

© Digital Cloud Training | https://digitalcloud.training
## Data Center
Private subnet
## Route 53 Resolver – Endpoints
## VPC
## Customer
gateway
VPN connection
VPN gateway
DNS Server
## Amazon Route 53
## Outbound
## Endpoint
## App Instance 1
DB Instance 1
What’s the IP for app1.org.local?
## Inbound
## Endpoint
## App1
NameTypeValue
app1.org.localA192.168.100
What’s the IP for DB Instance 1?
Resolver conditionally forwards DNS
queries for org.local names to the
on-premises DNS server
The on-premises DNS server
conditionally forwards to the
inbound endpoint

© Digital Cloud Training | https://digitalcloud.training
## Route 53 Resolver
•Route 53 Resolver answers DNS queries for:
•Local VPC domain names for EC2 instances (e.g. ec2-192-0-2-
## 44.compute-1.amazonaws.com)
•Records in private hosted zones (e.g. mydomain.com)
•Public domain names through recursive lookups against public name
servers on the internet
•Resolver endpoints are created for on-premises resources:
•Inbound Resolver endpoints allow DNS queries to your VPC from your
on-premises network or another VPC
•Outbound Resolver endpoints allow DNS queries from your VPC to
your on-premises network or another VPC
•Rules are created for forwarding queries based on domain names

© Digital Cloud Training | https://digitalcloud.training
## Route 53 Resolver Rules
rslvr-rr  -6345432e2ae344584
Association with one or more VPCs
The outbound resolver endpoint
The IP addresses of the DNS servers to forward queries
to for the specified domain name
The domain for which queries are forwarded
Rules are created in Route 53 for
forwarding outbound DNS queries
Options are Forward or System (use System to get Resolver to
process queries for a subdomain of a domain it forwards to)

© Digital Cloud Training | https://digitalcloud.training
Amazon CloudFront Origins
and Distributions

© Digital Cloud Training | https://digitalcloud.training
Amazon CloudFront
Users (US)
Edge location
## Region
Amazon EC2
## Amazon S3
CloudFront Origins
Edge location
Edge location
Edge location
Edge location
Edge location
Edge location
## Users
(Europe)
Users (UK)
## Users
(India)
## Users
(Asia)
## Users
(Australia)
Users (NZ)
Content is pushed
from the origin and
cached
Edge locations
are distributed
around the world
Users are directed
to the nearest
edge location

© Digital Cloud Training | https://digitalcloud.training
CloudFront Origins and Distributions
CloudFront Distribution
## Beach.jpg
## Behaviors
## S3 Origin
## Custom Origin
## Path Pattern
## Viewer Protocol Policy
## Cache Policy
## Origin Request Policy
RTMP distributions were discontinued
so only web distributions are currently
available
CloudFront Web Distribution:
•Speed up distribution of static and dynamic content, for
example, .html, .css, .php, and graphics files
•Distribute media files using HTTP or HTTPS
•Add, update, or delete objects, and submit data from web
forms
•Use live streaming to stream an event in real time
Name: d1schtd9zdwrm1.cloudfront.net
doc.html
## Manual.pdf
S3 static websites
can also be origins

© Digital Cloud Training | https://digitalcloud.training
Amazon CloudFront Caching
and Behaviors

© Digital Cloud Training | https://digitalcloud.training
Amazon CloudFront Caching
Edge location
## Global
## Users
## Regional
## Edge Cache
Edge location
## Global
## Users
## Regional
## Edge Cache
Edge location
## Global
## Users
## Region
Amazon EC2
## Amazon S3
CloudFront Origins
There are 12 Regional
## Edge Caches
There are 210
Edge locations

© Digital Cloud Training | https://digitalcloud.training
Amazon CloudFront Caching
Edge location
## (POP)
## Regional
## Edge Cache
## Region
CloudFront Origin
AWS Global
## Network
## HTTP GET
## Image
Cache MISS
Cache MISS
Object is cached for
TTL (default 24hrs)
Cache HIT
When the TTL expires
the file is removed
Decreasing the TTL is best for
Dynamic content, increasing TTL
is better for performance (and
reduces load on origin)

© Digital Cloud Training | https://digitalcloud.training
Amazon CloudFront Caching
•You can define a maximum Time To Live (TTL) and a
default TTL
•TTL is defined at the behavior level
•This can be used to define different TTLs for different
file types (e.g. png vs jpg)
•After expiration, CloudFront checks the origin for any
new requests (check the file is the latest version)
•Headers can be used to control the cache:
•Cache-Control max-age=(seconds) - specify how long before
CloudFront gets the object again from the origin server
•Expires – specify an expiration date and time

© Digital Cloud Training | https://digitalcloud.training
CloudFront Path Patterns
CloudFront Distribution
HTTP GET beach.jpg
## Beach.jpg
The path pattern determines
where to send the request
## Clip.mp4
## Behaviors
## Origin 1
## Origin 2
## *.jpg = Origin 1
## *.mp4 = Origin 2
## Default = Origin 1
HTTP GET clip.mp4
The default origin is used
for any requests that don’t
match a path pattern
## Origin 1
## Origin 1
## Origin 2

© Digital Cloud Training | https://digitalcloud.training
Caching Based on Request Headers
•You can configure CloudFront to forward headers
in the viewer request to the origin
•CloudFront can then cache multiple versions of an
object based on the values in one or more request
headers
•Controlled in a behavior to do one of the
following:
•Forward all headers to your origin (objects are not
cached)
•Forward a whitelist of headers that you specify
•Forward only the default headers (doesn’t cache
objects based on values in request headers)

© Digital Cloud Training | https://digitalcloud.training
CloudFront Signed URLs
and OAI/OAC

© Digital Cloud Training | https://digitalcloud.training
CloudFront Signed URLs
•Signed URLs provide more control
over access to content
•Can specify beginning and
expiration date and time, IP
addresses
## Serverless
## Application
Amazon CloudFront
## 1
## 2
## 3
## 4
Mobile app uses signed URL to
access distribution
Signed URL
returned
Mobile app authenticates to
application and requests signed URL
Signed URLs should be used for
individual files and clients that
don’t support cookies

© Digital Cloud Training | https://digitalcloud.training
CloudFront Signed Cookies
•Similar to Signed URLs
•Use signed cookies when you don’t want to change URLs
•Can also be used when you want to provide access to multiple
restricted files (Signed URLs are for individual files)

© Digital Cloud Training | https://digitalcloud.training
CloudFront Origin Access Identity (OAI)
Amazon CloudFront
S3 Bucket configured
as static website
## Custom Origin
## Bucket Policy
Origin Access Identity (OAI)
## Users
HTTP GET https://d1schtd9zdwrm1.cloudfront.net
GET https://mybucket.s3.amazonaws.com/beach.jpg
The policy restricts
access to the OAI
Access is blocked by
bucket policy

© Digital Cloud Training | https://digitalcloud.training
CloudFront Origin Access Control (OAC)
•Like a OAI but supports additional use cases
•AWS recommend using the OAC instead of an OAI
•Requires an S3 bucket policy that allows the CloudFront service principal

© Digital Cloud Training | https://digitalcloud.training
CloudFront Cache and
## Behavior Settings

© Digital Cloud Training | https://digitalcloud.training
CloudFront SSL/TLS and SNI

© Digital Cloud Training | https://digitalcloud.training
CloudFront SSL/TLS
## S3 Origin
## Custom Origin
AWS Certificate
## Manager
For CloudFront
certificate must be
issued in us-east-1
Certificate can be ACM or a
trusted third-party CA
## Viewer Protocol
## Origin Protocol
S3 has its own certificate
(can’t be changed)
Certificate can be ACM
(ALB) or third-party (EC2)
Default CF domain
name can be
changed using
## CNAMES
Origin certificates
must be public
certificates

© Digital Cloud Training | https://digitalcloud.training
CloudFront Server Name Indication (SNI)
## S3 Origin
## Custom Origin
Request URL includes
domain name which
matches certificate
Name: myotherdomain.com
HTTP GET: https://mypublicdomain.com
Multiple certificates
share the same IP
with SNI
HTTP GET: https://myotherdomain.com
Name: mypublicdomain.com
Note: SNI works with
browsers/clients released
after 2010 – otherwise
need dedicated IP

© Digital Cloud Training | https://digitalcloud.training
Lambda@Edge

© Digital Cloud Training | https://digitalcloud.training
Lambda@Edge
•Run Node.js and Python Lambda functions to customize the content
CloudFront delivers
•Executes functions closer to the viewer
•Can be run at the following points
•After CloudFront receives a request from a viewer (viewer request)
•Before CloudFront forwards the request to the origin (origin request)
•After CloudFront receives the response from the origin (origin response)
•Before CloudFront forwards the response to the viewer (viewer response)
CloudFront Cache
## S3 Origin
Viewer response
Origin response
Viewer request
Origin request

© Digital Cloud Training | https://digitalcloud.training
AWS Global Accelerator

© Digital Cloud Training | https://digitalcloud.training
AWS Global Accelerator
## Amazon Route 53
Users in US
Resolve dctlabs.com
## Answer:
## 51.45.2.12
## 53.58.31.89
Edge location
## Addresses:
## 51.45.2.12
## 53.58.31.89
us-east-1eu-west-1
AWS Global Network
## Global Accelerator
Connect via Edge Location
User traffic ingresses using
the closest Edge Location
Static anycast
IP addresses
Users are redirected
to another endpoint
Traffic traverses
the AWS global
network
Requests are
routed to the
optimal endpoint

© Digital Cloud Training | https://digitalcloud.training
AWS Global Accelerator
•Network Layer: Operates at the network layer (Layer 4 of
the OSI model)
•IP Address: Provides static IP addresses as a fixed entry
point to your applications
•Performance: Improves performance by leveraging the AWS
global network backbone, reducing internet latency and
jitter
•Health Checks: Performs health checks and automatically
reroutes traffic to healthy endpoints
•Application Protocols: Supports TCP and UDP traffic,
making it suitable for a wide range of applications, including
those requiring non-HTTP protocols
•Use Cases: Ideal for non-HTTP use cases such as gaming
(UDP traffic), IoT, VoIP, or for services where having a static
IP address is beneficial

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns –
DNS, Caching and Performance
## Optimization

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – DNS, Caching and Performance Optimization
An Elastic Load Balancer must be
resolvable using a company’s public
domain name. A Route 53 hosted zone
exists
Create an Alias record that maps the
domain name to the ELB
A website runs across two AWS
Regions. All traffic goes to one Region
and should be redirected only if the
website is unavailable
Create a failover routing policy in AWS
Route 53 and configure health checks
on the primary
Websites run in several countries and
distribution rights require restricting
access to content based on the
geographic source of the connection
Use AWS Route 53 geolocation routing
and restrict distribution based on
geographic location
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – DNS, Caching and Performance Optimization
A CloudFront distribution has multiple
S3 origins. Requests should be served
from different origins based on file
type being requested
Modify the CloudFront behavior and
configure a path pattern
Content is accessed using an application
and CloudFront distribution. Need to
control access to multiple files on the
distribution
Configure signed cookies and update
the application
Application runs behind an Application
Load Balancer in multiple Regions.
Need to intelligently route traffic based
on latency and availability
Create an AWS Global Accelerator and
add the ALBs
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## SECTION 9
Block and File Storage

© Digital Cloud Training | https://digitalcloud.training
Block vs File vs Object
## Storage

© Digital Cloud Training | https://digitalcloud.training
## Block Storage
Hard Disk Drive (HDD)
Solid State Drive (SSD)
•Also known as magnetic drives
•Older technology
•Much slower than SSD
•Much cheaper than SSD
•Uses flash memory
•Newer technology
•MUCH faster than HDD
•More expensive than HDD

© Digital Cloud Training | https://digitalcloud.training
## Block Storage
## Hard Disk
Drive (HDD)
## The Operating System
(OS) sees a volume. A
volume can be
partitioned and
formatted
## Disk Management
## C:
## 800 GB
## D:
## 200 GB
## Volume
## 1000 GB
Hard drives are
block-based
storage systems
Hard drives are block-based storage systems

© Digital Cloud Training | https://digitalcloud.training
## File Storage
## NIC
## Network Switch
## Network Attached
Storage Server (NAS)
The Operating System (OS) sees a file system that
is mapped to a local drive letter
The NAS “shares” file systems
over the network

© Digital Cloud Training | https://digitalcloud.training
## Object Storage Systems
## Object Storage
## Container
User uploads objects
using a web browser
Objects can be files,
videos, images etc.
The HTTP protocol is
used with a REST API
(e.g. GET, PUT, POST,
## SELECT, DELETE)
There is no hierarchy
of objects in the
container

© Digital Cloud Training | https://digitalcloud.training
Block vs File vs Object Storage
## Object Storage
## Container
There is no hierarchy of
objects in the container
## Disk Management
## C:
## 800 GB
## D:
## 200 GB
## Volume
## 1000 GB
The OS reads/writes at
the block level. Disks
can be internal, or
network attached
The OS sees volumes
that can be partitioned
and formatted
A filesystem is “mounted” to
the OS using a network share
Massively scalable
and low cost
A filesystem can be
shared by many users
## Block Storage
File StorageObject Storage
Cannot be mounted but can be
accessed programmatically
using the REST API

© Digital Cloud Training | https://digitalcloud.training
Amazon EBS Deployment and
## Volume Types

© Digital Cloud Training | https://digitalcloud.training
Amazon EBS Deployment
EC2 Instance
EBS Volume
## Amazon Elastic Block
Store (EBS)
## Availability Zone
EC2 Instance
## Availability Zone
EC2 Instance
EBS Volume
EBS Volume
EBS Volume
Limited support for
attaching multiple
instances*
EBS volumes are
replicated within
an AZ
EC2 instances
must be in the
same AZ as the
EBS volume

© Digital Cloud Training | https://digitalcloud.training
Amazon EBS Multi-Attach
EC2 Instance
## Availability Zone
EC2 Instance
EBS Volume
Available for Nitro
system-based
EC2 instances
EC2 Instance
Up to 16 instances
can be attached to a
single volume
Must be a
## Provisioned
IOPS io1 volume
Must be within
a single AZ
May not be on the
exam yet

© Digital Cloud Training | https://digitalcloud.training
Amazon EBS SSD-Backed Volumes
New and may
not be on the
exam yet
New and may
not be on the
exam yet
## Supported

© Digital Cloud Training | https://digitalcloud.training
Amazon EBS HDD-Backed Volumes

© Digital Cloud Training | https://digitalcloud.training
Amazon EBS
•EBS volume data persists independently of the life of
the instance
•EBS volumes do not need to be attached to an instance
•You can attach multiple EBS volumes to an instance
•You can use multi-attach to attach a volume to multiple
instances but with some constraints
•EBS volumes must be in the same AZ as the instances
they are attached to
•Root EBS volumes are deleted on termination by
default
•Extra non-boot volumes are not deleted on
termination by default

© Digital Cloud Training | https://digitalcloud.training
Amazon EBS Copying, Sharing
and Encryption

© Digital Cloud Training | https://digitalcloud.training
Amazon EBS Copying, Sharing and Encryption
EC2 Instance
## Volume
## Availability Zone A
EC2 Instance
## Availability Zone B
Snap ASnap B
## Amazon S3
## Region
## Volume
## Snap C

© Digital Cloud Training | https://digitalcloud.training
Take Snapshot, Create AMI, Launch New Instance
EC2 Instance
## Availability Zone A
## Availability Zone B
## Snapshot
## Amazon S3
## Region
## Volume
## AMI
EC2 Instance
## Volume

© Digital Cloud Training | https://digitalcloud.training
Copying and Sharing AMIs and Snapshots
## Snapshot
•Encryption state retained
•Same region
## Encrypted
## Snapshot
•Can be encrypted
•Can change regions
## Copy
## Unencrypted
## Snapshot
## Encrypted
## Volume
•Can be encrypted
•Can change AZ
## AMI
## Unencrypted
## Snapshot
•Cannot be encrypted
•Can be shared with other accounts
•Can be shared publicly
•Can change encryption key
•Can change regions
## Copy
## Volume
## Snapshot
## Snapshot
## Snapshot

© Digital Cloud Training | https://digitalcloud.training
Copying and Sharing AMIs and Snapshots
•Can change encryption key
•Can change region
## Encrypted
## Volume
## Encrypted
## Snapshot
Encrypted AMI
## Encrypted
## Snapshot
Encrypted AMI
## Encrypted
## AMI
## Copy
## Encrypted
## AMI
•Can change encryption key
•Can change AZ
EC2 Instance
## Unencrypted
## AMI
•Can change encryption state
•Can change AZ
EC2 Instance
•Can be shared with other accounts
(custom key only)
•Cannot be shared publicly
•Can be encrypted
•Can change AZ

© Digital Cloud Training | https://digitalcloud.training
Amazon EBS Snapshots and
## DLM

© Digital Cloud Training | https://digitalcloud.training
Amazon EBS Snapshots
EC2 Instance
## Volume
## Availability Zone A
EC2 Instance
## Availability Zone B
Snap ASnap B
## Region
## Volume
## Snap C
Snapshot taken to
capture a point-in-time
state of an instance
Snapshots are stored
on Amazon S3
Snapshots are
incremental
You can create an EBS
volume in another AZ
from a snapshot
## AMI
A snapshot can
be used to create
an AMI

© Digital Cloud Training | https://digitalcloud.training
Amazon Data Lifecycle Manager (DLM)
•DLM automates the creation, retention, and deletion
of EBS snapshots and EBS-backed AMIs
•DLM helps with the following:
•Protects valuable data by enforcing a regular backup
schedule
•Create standardized AMIs that can be refreshed at regular
intervals
•Retain backups as required by auditors or internal
compliance
•Reduce storage costs by deleting outdated backups
•Create disaster recovery backup policies that back up data
to isolated accounts

© Digital Cloud Training | https://digitalcloud.training
EC2 Instance Store Volumes

© Digital Cloud Training | https://digitalcloud.training
EBS vs instance store
## Amazon Elastic Block
Store (EBS)
## Availability Zone
EBS Volume
EC2 Host Server
EBS Volume
Instance Store volumes
are physically attached
to the host
EBS volumes are
attached over the
network
Instance Stores are
ephemeral - data is lost
when the instance is
powered down

© Digital Cloud Training | https://digitalcloud.training
EBS vs instance store
•Instance store volumes are high performance local disks that are
physically attached to the host computer on which an EC2 instance runs
•Instance stores are ephemeral which means the data is lost when
powered off (non-persistent)
•Instance stores are ideal for temporary storage of information that
changes frequently, such as buffers, caches, or  scratch data
•Instance store volume root devices are created from AMI templates
stored on S3
•Instance store volumes cannot be detached/reattached

© Digital Cloud Training | https://digitalcloud.training
Create and Attach
an EBS Volume

© Digital Cloud Training | https://digitalcloud.training
EBS Snapshots and
AMIs

© Digital Cloud Training | https://digitalcloud.training
Using RAID with EBS

© Digital Cloud Training | https://digitalcloud.training
Using RAID with EBS
•RAID stands for Redundant Array of
Independent disks
•Not provided by AWS, you must configure
through your operating system
•RAID 0 and RAID 1 are potential options on EBS
•RAID 5 and RAID 6 are not recommended by
## AWS

© Digital Cloud Training | https://digitalcloud.training
Using RAID with EBS
•RAID 0 is used for striping data across disks
## (performance):
•Use 2 or more disks
•If one disk fails, the entire RAID set fails
Data writes
EBS Volume
EBS Volume
## Block 1
## Block 3
## Block 5
## Block 7
## Block 2
## Block 4
## Block 6
## Block 8

© Digital Cloud Training | https://digitalcloud.training
Using RAID with EBS
•RAID 1 is used for mirroring data across disks
(redundancy / fault tolerance):
•If one disk fails, the other disk is still working
•Data gets sent to 2 EBS volumes at the same time
Data writes
EBS Volume
EBS Volume
## Block 1
## Block 2
## Block 3
## Block 4
## Block 1
## Block 2
## Block 3
## Block 4

© Digital Cloud Training | https://digitalcloud.training
Amazon Elastic File System (EFS)

© Digital Cloud Training | https://digitalcloud.training
Amazon Elastic File System (EFS)
EFS File system
(Regional)
## /efs-mnt
The connection protocol is NFS
EC2 InstanceEC2 Instance
## /efs-mnt
Regional file systems
have mount targets in
multiple AZs
Instances connect
to a mount point
in the local AZ
Instances can connect to
mount points in other
AZs in the Region
Note: EFS supports Linux only
EC2 Instance
## Availability Zone
One Zone file systems have
mount targets in a single AZ
## /efs-mnt

© Digital Cloud Training | https://digitalcloud.training
Amazon ElasticFileSystem (EFS)
•Data consistency – write operations for Regional file
systems are durably stored across Availability Zones
•File locking – NFS client applications can use NFS v4
file locking for read and write operations on EFS files
•Storage classes – there are three options:
•EFS Standard – uses SSDs for low latency performance
•EFS Infrequent Access (IA) – cost effective option
•EFS Archive – even cheaper for less active data (archival)
•Durability – all storage classes offer 11 9s of
durability

© Digital Cloud Training | https://digitalcloud.training
Amazon Elastic File System (EFS)
EFS File system
Corporate data center
## On-premises
client
EFS File system
EC2 Instance
## Region
## Region
EFS file systems can be
replicated across Regions
Mount points can be
created but the file
system is read-only
On-premises computers
can also mount EFS file
systems

© Digital Cloud Training | https://digitalcloud.training
Amazon ElasticFileSystem (EFS)
•EFS Replication – data is replicated across Regions
for disaster recovery purposes with RPO/RTO in the
minutes
•Automatic Backup – EFS integrates with AWS
Backup for automatic file system backups
•Performance options – there are two options:
•Provisioned throughput – Specify a level of throughput
that the file system can drive independent of the file
system's size
•Bursting throughput – Throughput scales with the
amount of storage and supports bursting to higher levels

© Digital Cloud Training | https://digitalcloud.training
Create an Amazon EFS
## File System

© Digital Cloud Training | https://digitalcloud.training
Amazon FSx

© Digital Cloud Training | https://digitalcloud.training
Amazon FSx
•Amazon FSx provides fully managed third-
party file systems
•Amazon FSx provides you with two file
systems to choose from:
•Amazon FSx for Windows File Server for
Windows-based applications
•Amazon FSx for Lustre for compute-intensive
workloads

© Digital Cloud Training | https://digitalcloud.training
Amazon FSx for Windows File Server
•Provides a fully managed native Microsoft Windows
file system
•Full support for the SMB protocol, Windows NTFS,
and Microsoft Active Directory (AD) integration
•Supports Windows-native file system features:
•Access Control Lists (ACLs), shadow copies, and user
quotas.
•NTFS file systems that can be accessed from up to
thousands of compute instances using the SMB protocol
•High availability: replicates data within an Availability
Zone (AZ)
•Multi-AZ: file systems include an active and standby
file server in separate AZs

© Digital Cloud Training | https://digitalcloud.training
Public subnet
Public subnet
Amazon FSx for Windows File Server
EC2 Instance
(Windows)
EC2 Instance
(Windows)
## VPC
Corporate data center
## On-premises
client (Windows)
VPN or Direct
Connect connection
## Availability Zone
## Availability Zone
Amazon FSx
AWS Managed
Microsoft AD
With multi-AZ a
standby can be
created in another AZ

© Digital Cloud Training | https://digitalcloud.training
Amazon FSx for Lustre
•High-performance file system optimized for fast
processing of workloads such as:
•Machine learning
•High performance computing (HPC)
•Video processing
•Financial modeling
•Electronic design automation (EDA)
•Works natively with S3, letting you transparently access
your S3 objects as files
•Your S3 objects are presented as files in your file
system, and you can write your results back to S3
•Provides a POSIX-compliant file system interface

© Digital Cloud Training | https://digitalcloud.training
Public subnet
Public subnet
Amazon FSx for Lustre
EC2 Instance
EC2 Instance
## VPC
Corporate data center
## On-premises
client
VPN or Direct
Connect connection
## Availability Zone
## Availability Zone
## S3 Bucket
Amazon FSx for Lustre
Use for cloud bursting
and data migration
S3 objects can be viewed as
files in FSx; result data can
be written back to S3

© Digital Cloud Training | https://digitalcloud.training
AWS Storage Gateway

© Digital Cloud Training | https://digitalcloud.training
AWS Storage Gateway

© Digital Cloud Training | https://digitalcloud.training
AWS Storage Gateway – File Gateway
AWS Storage Gateway
## S3 Standard
S3 Standard IA
S3 One Zone IA
AWS CloudCorporate
data center
## Server
## CACHE
The file system is
mounted using
NFS or SMB
A virtual gateway
appliance runs on
Hyper-V, VMware,
or EC2
A local cache provides
low latency access to
recently used data
Files are stored
as objects in S3
Can store data
in multiple S3
storage classes

© Digital Cloud Training | https://digitalcloud.training
AWS Storage Gateway – File Gateway
•File gateway provides a virtual on-premises file
server
•Store and retrieve files as objects in Amazon S3
•Use with on-premises applications, and EC2-based
applications that need file storage in S3 for object-
based workloads
•File gateway offers SMB or NFS-based access to data
in Amazon S3 with local caching

© Digital Cloud Training | https://digitalcloud.training
AWS Storage Gateway - Volume Gateway
AWS Storage Gateway
## S3 Standard
AWS CloudCorporate
data center
## CACHE
## Server
AWS Storage Gateway
## S3 Standard
## Server
iSCSI
iSCSI
## CACHED VOLUME MODE
## STORED VOLUME MODE
Asynchronous replication
A cache of the most
recently used data
on-premise
Entire data set is
stored on-premise
Entire data set is
stored in S3
Data backed up as
point-in -time
snapshots

© Digital Cloud Training | https://digitalcloud.training
AWS Storage Gateway - Volume Gateway
•The volume gateway supports block-based volumes
•Block storage – iSCSI protocol
- Cached Volume mode – the entire dataset is stored on S3 and a
cache of the most frequently accessed data is cached on-site
- Stored Volume mode – the entire dataset is stored on-site and is
asynchronously backed up to S3 (EBS point-in-time snapshots).
Snapshots are incremental and compressed

© Digital Cloud Training | https://digitalcloud.training
AWS Storage Gateway - Tape Gateway
AWS Storage Gateway
## S3 Glacier
## S3 Glacier
## Deep Archive
## S3 Standard
AWS CloudCorporate
data center
## Backup Server
## VTL
iSCSI
Backup server can
use many common
backup applications
Once tapes are
ejected from the
backup app, they
are stored in one
of these classes
S3 standard is
used when
writing to tapes

© Digital Cloud Training | https://digitalcloud.training
AWS Storage Gateway - Tape Gateway
•Used for backup with popular backup software
•Each gateway is preconfigured with a media changer and tape drives. Supported by
NetBackup, Backup Exec, Veeam etc.
•When creating virtual tapes, you select one of the following sizes: 100 GB, 200 GB, 400
GB, 800 GB, 1.5 TB, and 2.5 TB
•A tape gateway can have up to 1,500 virtual tapes with a maximum aggregate capacity of
## 1 PB
•All data transferred between the gateway and AWS storage is encrypted using SSL
•All data stored by tape gateway in S3 is encrypted server-side with Amazon S3-Managed
Encryption Keys (SSE-S3)

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns –
Block and File Storage

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – Block and File Storage
Simple method of backing up Amazon
EBS volumes is required that is fully
automated
Use Data Lifecycle Manager to create a
backup schedule
A distributed application has many
nodes that each hold a copy of data
that is synchronized between them.
Need the best performance
Use instance stores for storing the data
with the best performance
RequirementSolution
Application must startup quickly when
launched by ASG but requires app
dependencies and code to be installed
Create an AMI that includes the
application dependencies and code

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – Block and File Storage
Many Linux instances must be attached
to a shared filesystem that scales
elastically
Create an Amazon EFS file system and
mount from each instance
Company requires a managed file
system that uses the NTFS file system
Use Amazon FSx for Windows File
## Server
On-premises servers must be able to
attach a block storage system locally.
Data should be backed up to S3 as
snapshots
Deploy an AWS Storage Gateway
volume gateway in stored volume mode
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – Block and File Storage
An Amazon EBS volume must be
moved between Regions
Take a snapshot and copy the snapshot
between Regions
Root EBS volumes for a critical
application must not be deleted on
termination
Modify the delete on termination
attribute when launching the EC2
instances
On-premises servers use NFS to attach
a file system. The file system should be
replaced with an AWS service that uses
Amazon S3 with a local cache
Deploy an AWS Storage Gateway file
gateway
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## SECTION 10
Docker Containers and ECS

© Digital Cloud Training | https://digitalcloud.training
Docker Containers and
## Microservices

© Digital Cloud Training | https://digitalcloud.training
Server Virtualization vs Containers
Windows OS
## Website
## Server
## Hypervisor
## Server
## Docker Engine
Windows OS
Every VM/instance needs an operating
system which uses significant resources

© Digital Cloud Training | https://digitalcloud.training
## Docker Containers
## Server
## Docker Engine
Windows OS
A container includes all the code,
settings, and dependencies for
running the application
Containers start
up very quickly
Each container is isolated
from other containers
Containers are very
resource efficient

© Digital Cloud Training | https://digitalcloud.training
## Docker Containers
•Docker utilizes containerization to package an application
and its dependencies into a single container image
•Docker provides Docker Hub, a cloud-based registry
service for sharing container images and automating
workflows
•Containers are lightweight because they share the host
system's kernel
•Docker is ideal for microservices architectures and
building cloud-native applications

© Digital Cloud Training | https://digitalcloud.training
Cloud-Native Applications
## Order Processing
## S3 Static Website
SQS Queue
## Order Table
## REST API
## Notification
AuthenticationCognito User Pool
## Shopping Cart
## Customer Service
## Payment Gateway
## Microservices
## Shipping
## REST API
Microservices architecture:
Applications are structured as a
collection of loosely coupled,
independently deployable services,
each running its own process
Containers and Functions: Code
runs in Docker containers and
Lambda functions for isolation,
elasticity, and cost-efficiency
Programmable, API-based: Inter-
service communication through APIs
## REST API
## Payment
## Processor

© Digital Cloud Training | https://digitalcloud.training
Microservices: Attributes and Benefits
Microservices AttributeMicroservices Benefit
Business-oriented architectureDevelopment organized around business capabilities;
teams may be cross-functional and services may be reused
Independently deployable blocks of codeCan be scaled and maintained independently
Flexible use of technologiesEach microservice can be written using different
technologies (e.g. programming languages)
Speed and agilityFast to deploy and update. Easy to include high availability
and fault tolerance for each microservice
Use of Application Programming Interfaces (APIs)Easier integrations between application components;
assists with loose coupling

© Digital Cloud Training | https://digitalcloud.training
## Amazon Elastic
Container Service (ECS)

© Digital Cloud Training | https://digitalcloud.training
Amazon ECS
## Availability Zone
## Availability Zone
ECS Container
instance
ECS Container
instance
Ta s kTa s kTa s kTa s k
## Image
## Image
## {
"containerDefinitions": [
## {
## "name": "wordpress",
## "links": [
## "mysql"
## ],
## "image":  "wordpress",
"essential": true  ,
"portMappings": [
## {
"containerPort": 80,
"hostPort":  80
## }
## ],
## "memory":  500  ,
## "cpu":  10
## }
## Task Definition
## Registry
ECS Services are used to maintain
a desired count of tasks
An ECS Ta s k is created
from a Task Definition
An ECS Task is a running
Docker container
## Amazon Elastic Container Service
## Amazon Elastic Container
## Registry
ECS Cluster
ECS Service
An AmazonECS Clusteris a logical
grouping of tasks or services
Docker images can be
stored in Amazon ECR

© Digital Cloud Training | https://digitalcloud.training
Amazon ECS Key Features
•Serverless with AWS Fargate – managed for you and fully
scalable
•Fully managed container orchestration – control plane is
managed for you
•Docker support – run and manage Docker containers
with integration into the Docker Compose CLI
•Windows container support – ECS supports management
of Windows containers
•Elastic Load Balancing integration – distribute traffic
across containers using ALB or NLB
•Amazon ECS Anywhere – enables the use of Amazon ECS
control plane to manage on-premises implementations

© Digital Cloud Training | https://digitalcloud.training
Amazon ECS Components
Elastic Container Service (ECS)Description
ClusterLogical grouping of tasks or services
Container instanceEC2 instance running the the ECS agent
Task DefinitionBlueprint that describes how a docker container should
launch
Ta s kA running container using settings in a task definition
ImageA Docker image referenced in the task definition
ServiceDefines long running tasks – can control task count with
Auto Scaling and attach an ELB

© Digital Cloud Training | https://digitalcloud.training
Amazon ECS Images
•Containers are created from a read-only template called an
image which has the instructions for creating a Docker
container
•Images are built from a Dockerfile
•Only Docker containers are supported on ECS
•Images are stored in a registry such as DockerHub or Amazon
Elastic Container Registry (ECR)
•ECR is a managed AWS Docker registry service that is secure,
scalable and reliable
•ECR supports private Docker repositories with resource-based
permissions using AWS IAM in order to access repositories and
images
•You can use the Docker CLI to push, pull and manage images
ImageImage
## Amazon Elastic
## Container Registry
## Registry

© Digital Cloud Training | https://digitalcloud.training
Amazon ECS Tasks and Task Definitions
•A task definition is required to run
Docker containers in Amazon ECS
•A task definition is a text file in JSON
format that describes one or more
containers, up to a maximum of 10
•Task definitions use Docker images to
launch containers
ECS Container
instance
Ta s kTa s k
## {
"containerDefinitions": [
## {
## "name": "wordpress",
## "links": [
## "mysql"
## ],
## "image":  "wordpress",
"essential": true  ,
"portMappings": [
## {
"containerPort": 80,
"hostPort":  80
## }
## ],
## "memory":  500  ,
## "cpu":  10
## }
## Task Definition
ECS Cluster

© Digital Cloud Training | https://digitalcloud.training
Launch Types – EC2 and Fargate
## Registry:
ECR, Docker Hub, Self-hosted
## Registry:
ECR, Docker Hub
EC2 Launch Type:
•You explicitly provision EC2 instances
•You’re responsible for managing EC2 instances
•Charged per running EC2 instance
•EFS, FSx, and EBS integration
•You handle cluster optimization
•More granular control over infrastructure
## Fargate Launch Type:
•Fargate automatically provisions resources
•Fargate provisions and manages compute
•Charged for running tasks
•EFS integration only
•Fargate handles cluster optimization
•Limited control
ECS Service
ECS Container
instance
ECS Container
instance
Ta s kTa s kTa s kTa s k
ECS EC2 Cluster
ECS Service
Ta s k
Ta s kTa s kTa s k
ECS Fargate Cluster

© Digital Cloud Training | https://digitalcloud.training
ECS and IAM Roles
ECS Service
ECS   Container instance
ECS EC2 Cluster
Task IAM Role
## Task
Instance IAM Role
AmazonEC2ContainerServiceforEC2Role
The container instance IAM
role provides permissions to
the host
The ECS task IAM role provides
permissions to the container
NOTE: With the Fargate launch type the container
instance role is replaced with the Task Execution Role

© Digital Cloud Training | https://digitalcloud.training
Amazon ECS and IAM Roles

© Digital Cloud Training | https://digitalcloud.training
ECS and IAM Roles
There are several roles used with ECS:
•Amazon ECS container instance IAM role – used by EC2
and external instances to provide permissions to the
container agent to call AWS APIs
•Task IAM role – the permissions granted in the IAM role
are assumed by the containers running in the task
•Amazon ECS task execution IAM role – the task
execution role grants the Amazon ECS container and
Fargate agents permissions to make AWS API calls on
your behalf
•Amazon ECS infrastructure IAM role – allows Amazon
ECS to manage infrastructure resources in your clusters
on your behalf (e.g. EBS volumes)

© Digital Cloud Training | https://digitalcloud.training
ECS and IAM Roles
There are several roles used with ECS:
•ECS Anywhere IAM role – On-premises servers or virtual
machines (VM) require an IAM role to communicate with
AWS APIs
•Amazon ECS CodeDeploy IAM Role – the CodeDeploy
service needs permissions to update ECS when
performing blue/green deployments
•Amazon ECS EventBridge IAM Role – to use Amazon ECS
scheduled tasks with EventBridge rules and targets, the
EventBridge service needs permissions

© Digital Cloud Training | https://digitalcloud.training
ECS and IAM Roles
ECS Service
ECS Container instance
ECS EC2 Cluster
IAM Task Role
## Task
IAM Instance Role
AmazonEC2ContainerServiceforEC2Role
The container instance
IAM role provides
permissions to the host
The ECS task IAM role
provides permissions to
the container

© Digital Cloud Training | https://digitalcloud.training
ECS and IAM Roles
ECS Service
ECS Fargate Cluster
IAM Task Role
## Task
With the Fargate launch type only
IAM task roles can be applied

© Digital Cloud Training | https://digitalcloud.training
ECS and IAM Roles
•A container can only retrieve credentials for the IAM
role that is defined in the task definition to which it
belongs
•A container never has access to credentials that are
intended for another container that belongs to
another task
•When using EC2 instances, tasks are not prevented
from accessing credentials supplied to the IAM
instance role

© Digital Cloud Training | https://digitalcloud.training
Scaling Amazon ECS

© Digital Cloud Training | https://digitalcloud.training
Auto Scaling for ECS
Two types of scaling:
1.Service auto scaling
2.Cluster auto scaling
•Service auto scaling automatically adjusts the desired task
count up or down using the Application Auto Scaling service
•Service auto scaling supports target tracking, step, and
scheduled scaling policies
•Cluster auto scaling uses a Capacity Provider to scale the
number of EC2 cluster instances using EC2 Auto Scaling

© Digital Cloud Training | https://digitalcloud.training
## Service Auto Scaling
ECS Service
ECS Container
instance
ECS Container
instance
Ta s kTa s kTa s k
ECS Cluster
MetricsMetrics
Amazon CloudWatch
Ta s k
•1. Metric reports CPU > 80%
•2. CloudWatch notifies
## Application Auto Scaling
•3. ECS launches additional task
## Application Auto Scaling

© Digital Cloud Training | https://digitalcloud.training
## Service Auto Scaling
•Amazon ECS Service Auto Scaling supports the following types of scaling
policies:
•Target Tracking Scaling Policies—Increase or decrease the number of
tasks that your service runs based on a target value for a specific
CloudWatch metric
•Step Scaling Policies—Increase or decrease the number of tasks that
your service runs in response to CloudWatch alarms. Step scaling is
based on a set of scaling adjustments, known as step adjustments,
which vary based on the size of the alarm breach
•Scheduled Scaling—Increase or decrease the number of tasks that
your service runs based on the date and time

© Digital Cloud Training | https://digitalcloud.training
## Cluster Auto Scaling
Auto Scaling group
ECS Service
ECS Container
instance
ECS Container
instance
Ta s kTa s kTa s k
ECS Cluster
## Metrics
## Metrics
Amazon CloudWatch
Ta s k
•1. Metric reports target
capacity > 80%
•2. CloudWatch notifies ASG
•3. AWS launches additional
container instance
ECS Container
instance
## Amazon Elastic Container Service
A Capacity provider reservation
metric measures the total
percentage of cluster resources
needed by allECSworkloads in the
cluster
ASG is linked to ECS
using a Capacity
## Provider

© Digital Cloud Training | https://digitalcloud.training
## Cluster Auto Scaling
•Uses an ECS resource type called a Capacity Provider
•A Capacity Provider can be associated with an EC2 Auto Scaling Group
## (ASG)
•ASG can automatically scale using:
•Managed scaling -  with an automatically-created scaling policy on
your ASG
•Managed instance termination protection -  which enables container-
aware termination of instances in the ASG when scale-in happens

© Digital Cloud Training | https://digitalcloud.training
Amazon ECS with ALB

© Digital Cloud Training | https://digitalcloud.training
Private subnet
Private subnet
Amazon ECS with ALB
ECS Service
## Application Load Balancer
Host port: 32600
Listener: HTTP (80)
Container port: 80
## Apache
Public subnet
NAT gateway
Public subnet
nginx
Container port: 80
Host port: 32612
Container port: 80
## Apache
nginx
Host port: 32668
Container port: 80
Host port: 32669
ECS Service
N AT  gateway
required for tasks in
private subnets to
access the internet
All connections to
web services coming
into HTTP listener
## (port 80)
Each task is running a
web service on port 80
A dynamic port is
allocated on the host

© Digital Cloud Training | https://digitalcloud.training
## Launch Docker Containers
on AWS Fargate

© Digital Cloud Training | https://digitalcloud.training
## Amazon Elastic Kubernetes
Service (EKS)

© Digital Cloud Training | https://digitalcloud.training
Amazon EKS
•Amazon Elastic Kubernetes Service (Amazon EKS) is a managed service for
running Kubernetes applications in the cloud or on-premises
•Kubernetes is an open-source system for automating deployment, scaling,
and management of containerized applications
•Use when you need to standardize container orchestration across multiple
environments using a managed Kubernetes implementation
•Features:
•Hybrid Deployment - manage Kubernetes clusters and applications across hybrid
environments (AWS + On-premises)
•Batch Processing - run sequential or parallel batch workloads on your EKS cluster
using the Kubernetes Jobs API. Plan, schedule and execute batch workloads
•Machine Learning - use Kubeflow with EKS to model your machine learning
workflows and efficiently run distributed training jobs using the latest EC2 GPU-
powered instances, including Inferentia
•Web Applications - build web applications that automatically scale up and down and
run in a highly available configuration across multiple Availability Zones

© Digital Cloud Training | https://digitalcloud.training
Amazon EKS
## Region
## VPC
## Availability Zone
Public subnet
Private subnet
## Availability Zone
Public subnet
## Availability Zone
EKS Cluster
## Amazon Kubernetes
## Service
## Worker Nodes
EKS Control Plane
Managed Kubernetes service
– runs on EC2 / Fargate and
also AWS Outposts
Groups of containers are known
as Pods in Kubernetes
EKS supports load balancing
with ALB, NLB, CLB

© Digital Cloud Training | https://digitalcloud.training
Amazon EKS Auto Scaling
## Workload Auto Scaling:
•Vertical Pod Autoscaler -  automatically adjusts the CPU and memory
reservations for your pods to help "right size" your applications
•Horizontal Pod Autoscaler -  automatically scales the number of pods in a
deployment, replication controller, or replica set based on that
resource's CPU utilization
## Cluster Auto Scaling:
•Amazon EKS supports two autoscaling products:
•Kubernetes Cluster Autoscaler
•Karpenter open source autoscaling project
•The cluster autoscaler uses AWS scaling groups, while Karpenter works
directly with the Amazon EC2 fleet

© Digital Cloud Training | https://digitalcloud.training
Amazon EKS and Elastic Load Balancing
•Amazon EKS supports Network Load Balancers and Application Load
## Balancers
•The AWS Load Balancer Controller manages AWS Elastic Load Balancers
for a Kubernetes cluster
•Install the AWS Load Balancer Controller using Helm V3 or later or by
applying a Kubernetes manifest
•The controller provisions the following resources:
•An AWS Application Load Balancer (ALB) when you create a
## Kubernetes Ingress
•An AWS Network Load Balancer (NLB) when you create a
Kubernetes service of type
LoadBalancer
•In the past, the Kubernetes network load balancer was used for instance
targets, but the AWS Load balancer Controller was used for IP targets
•With the AWS Load Balancer Controller version 2.3.0 or later, you can
create NLBs using either target type

© Digital Cloud Training | https://digitalcloud.training
Amazon EKS Distro
•Amazon EKS Distro is a distribution of Kubernetes with the same
dependencies as Amazon EKS
•Allows you to manually run Kubernetes clusters anywhere
•EKS Distro includes binaries and containers of open-source Kubernetes,
etcd, networking, and storage plugins, tested for compatibility
•You can securely access EKS Distro releases as open source on GitHub or
within AWS via Amazon S3 and Amazon ECR
•Amazon EKS Distro alleviates the need to track updates, determine
compatibility, and standardize on a common Kubernetes version across
distributed teams
•You can create Amazon EKS Distro clusters in AWS on Amazon EC2 and
on your own on-premises hardware using the tooling of your choice

© Digital Cloud Training | https://digitalcloud.training
Amazon ECS and EKS Anywhere
•Run ECS or EKS on customer-managed infrastructure, supported by AWS
•Customers can run Amazon ECS/EKS Anywhere on their own on-
premises infrastructure on bare metal servers
•You can also deploy ECS/EKS Anywhere using VMware vSphere

© Digital Cloud Training | https://digitalcloud.training
## Amazon Elastic
Container Registry (ECR)

© Digital Cloud Training | https://digitalcloud.training
Amazon Elastic Container Registry (ECR)
•Amazon ECR is a fully-managed container
registry
•Integrated with Amazon ECS and Amazon EKS
•Supports Open Container Initiative (OCI) and
Docker Registry HTTP API V2 standards
•You can use Docker tools and Docker CLI
commands such as
push, pull, list, and tag
•Can be accessed from any Docker environment –
in the cloud, on-premises, or on you machine

© Digital Cloud Training | https://digitalcloud.training
Amazon Elastic Container Registry (ECR)
•Container images and artifacts are stored in S3
•You can use namespaces to organize repositories
•Public repositories allow everyone to access
container images
•Access control applies to private repositories:
•IAM access control - Set policies to define access to
container images in private repositories
•Resource-based policies - Access control down to
the individual API action such as
create, list, describe,
delete, and get

© Digital Cloud Training | https://digitalcloud.training
Amazon ECR Components
ECR ComponentDescription
RegistryAn Amazon ECR private registry is provided to each AWS account; you can create
one or more repositories in your registry and store images in them
Authorization tokenYour client must authenticate to Amazon ECR registries as an AWS user before it
can push and pull images
RepositoryAn Amazon ECR repository contains your Docker images, OCI images, and OCI
compatible artifacts
Repository policyYou can control access to your repositories and the images within them with
repository policies
ImageYou can push and pull container images to your repositories

© Digital Cloud Training | https://digitalcloud.training
Amazon Elastic Container Registry (ECR)
•Lifecycle policies - manage the lifecycle of the
images in your repositories
•Image scanning - identify software vulnerabilities
in your container images
•Cross-Region and cross-account replication –
replicate images across accounts/Region
•Pull through cache rules - cache repositories in
remote public registries in your private Amazon
ECR registry

© Digital Cloud Training | https://digitalcloud.training
Amazon Elastic Container Registry (ECR)
Ta s k
## Image
## Amazon Elastic Container
## Registry
## Registry
ECS Fargate Cluster
Public subnet
## Amazon Elastic Container Service
EC2 Instance with Docker
## Ubuntu
## Image
Download and
customize image
Upload image
Run task using
image

© Digital Cloud Training | https://digitalcloud.training
Pushing an Image to a Private Repository
•Users must have the following IAM permissions:
The Resource element can
also be used to scope to a
specific repository ARN

© Digital Cloud Training | https://digitalcloud.training
Pushing an Image to a Private Repository
•First, authenticate the Docker client to ECR:
•Tag your image with the Amazon ECR registry, repository, and
image tag name to use:
•Push the image using the docker push command:

© Digital Cloud Training | https://digitalcloud.training
AWS App Runner

© Digital Cloud Training | https://digitalcloud.training
AWS App Runner
AWS App Runner
## Image
ECR Registry
## Create Service
•Source
•Auto Scaling
•Load Balancing
•Health Check
•Networking
•Observability
GitHub Repo
## Code
https://u66ymnfyst.us-east-1.awsapprunner.com
Fully managed service for
deploying containerized web
apps and APIs
PaaS solution with all
components managed
– just bring your code
and container image!

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns –
Amazon ECS

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – Amazon ECS
Application will be deployed on
Amazon ECS and must scale based on
memory
Use service auto-scaling and use the
memory utilization
Application will run on Amazon ECS
tasks across multiple hosts and needs
access to an Amazon S3 bucket
Use a task execution IAM role to
provide permissions to S3 bucket.
Company requires standard Docker
container automation and
management service to be used across
multiple environments
Deploy Amazon EKS
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – Amazon ECS
Company plans to deploy Docker
containers on AWS at the lowest cost
Use Amazon ECS with a cluster of Spot
instances and enable Spot instance
draining
Company plans to migrate Docker
containers to AWS and does not want
to manage operating systems
Migrate to Amazon ECS using the
Fargate launch type
RequirementSolution
Multiple microservices applications
running on Amazon ECS. Need to route
based on information in the HTTP
header
Deploy an Application Load Balancer in
front of ECS and use query string
parameter based routing

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – Amazon ECS
Containerized app runs on Amazon
EKS. Need to collect and centrally view
metrics and logs including EKS
namespaces and EKS services
Configure CloudWatch Container
Insights and view data in CloudWatch
console
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## SECTION 11
## Serverless Applications

© Digital Cloud Training | https://digitalcloud.training
Serverless Services and
Event-Driven Architecture

© Digital Cloud Training | https://digitalcloud.training
## Serverless Services
•With serverless there are no instances to manage
•You don’t need to provision hardware
•There is no management of operating systems or
software
•Capacity provisioning and patching is handled
automatically
•Provides automatic scaling and high availability
•Can be very cheap!

© Digital Cloud Training | https://digitalcloud.training
Serverless Services and Event-Driven Architecture
Lambda FunctionS3 Static WebsiteSQS Queue
DynamoDB Table
## Lambda Function
## S3 Bucket
SNS Topic
User uploads a
file through a
static website
Serverless function
processes file
A notification is sent using
SNS and email
Function processes the
message and stores
information in a database
Processed file is
stored in a bucket

© Digital Cloud Training | https://digitalcloud.training
AWS Lambda

© Digital Cloud Training | https://digitalcloud.training
AWS Lambda
Lambda function
## Developer
Code can be uploaded
using zip or war formats
Functions are invocated based on events
and the code is then executed
Code is executed
Event is written to
CloudWatch Logs
Pricing is based on memory assigned and
the duration of function execution

© Digital Cloud Training | https://digitalcloud.training
AWS Lambda
•Languages –   Lambda natively supports Java, Go,
PowerShell, Node.js, C#, Python, and Ruby code
•Execution Role (IAM Role) – this role grants the function
permissions to access AWS services and resources
•Monitoring and Logging –   integrates with Amazon
CloudWatch
•Memory and Timeout – you can specify the amount of
memory allocated to a function and the maximum
execution time
•Note: The maximum execution time is 15 minutes

© Digital Cloud Training | https://digitalcloud.training
## Lambda Function Invocation
•Lambda functions run in response to events from various AWS
services or direct invocation from the AWS SDKs or API
•Functions can be invoked synchronously or asynchronously:
•With synchronous invocation, applications wait for the function to
process the event and return a response
•With asynchronous invocation, Lambda queues the event for
processing and returns a response immediately
•Lambda scales horizontally by running multiple instances of a
function in parallel, up to the concurrency limit
## Lambda
Function invocation
Function is
executed

© Digital Cloud Training | https://digitalcloud.training
Connecting Lambda to an Amazon VPC
## VPC
## Availability Zone
Public subnet
Private subnet
## Lambda Function
## ENI
## Internet
## Gateway
NAT GatewayInstance
## Availability Zone
Public subnet
Private subnet
ENIInstance
Lambda functions are
Regional and do not have
VPC access by default
Lambda functions can be
connected to a VPC
Must select the VPC, subnets,
and security group
The function execution role must have
permissions create the ENIs
A NAT gateway is required
for internet connectivity

© Digital Cloud Training | https://digitalcloud.training
Create Function to Resize
## Instance

© Digital Cloud Training | https://digitalcloud.training
## Application Integration
## Services Overview

© Digital Cloud Training | https://digitalcloud.training
## Application Integration Services Overview
ServiceWhat it doesExample use cases
## Simple Queue Service
Messaging queue; store and forward
patterns
Building distributed / decoupled applications
## Simple Notification Service
Set up, operate, and send notifications
from the cloud
Send email notification when CloudWatch alarm is
triggered
## Step Functions
Out-of-the-box coordination of AWS
service components with visual
workflow
Order processing workflow
## Simple Workflow Service
Need to support external processes or
specialized execution logic
Human-enabled workflows like an order fulfilment
system or for procedural requests
Note: AWS recommends that for new applications
customers consider Step Functions instead of SWF
Amazon MQ
Message broker service for Apache
Active MQ and RabbitMQ
Need a message queue that supports industry
standard APIs and protocols; migrate queues to AWS
## Amazon Kinesis
Collect, process, and analyze streaming
data.
Collect data from IoT devices for later processing

© Digital Cloud Training | https://digitalcloud.training
Kinesis vs SQS vs SNS
Amazon KinesisAmazon SQSAmazon SNS
Consumers pull dataConsumers pull dataPush data to many subscribers
As many consumers as you needData is deleted after being consumed
Publisher / subscriber model
Routes related records to same record
processor
Can have as many workers (consumers) as
you need
Integrates with SQS for fan-out
architecture pattern
Multiple applications can access stream
concurrently
No ordering guarantee (except with FIFO
queues)
Up to 10,000,000 subscribers
Ordering at the shard levelProvides messaging semanticsUp to 100,000 topics
Can consume records in correct order at
later time
Individual message delayData is not persisted
Must provision throughputDynamically scalesNo need to provision throughput

© Digital Cloud Training | https://digitalcloud.training
Amazon SQS

© Digital Cloud Training | https://digitalcloud.training
Decoupling with SQS Queues
SQS Queue
## Web Tier
Direct integration
## Auto Scaling Group
## App Tier
## Auto Scaling Group
## Web Tier
## Auto Scaling Group
## App Tier
## Auto Scaling Group
Decoupled integration
EC2 instance polls
## SQS
Web tier connects
directly to app tier
App tier must keep
up with workload or
failure will occur

© Digital Cloud Training | https://digitalcloud.training
SQS Queue Types
## Standard Queue
## 1
## 5
## 3
## 2
## 6
## 7
## 4
## 8
## 7654321
FIFO Queue
## First-in, First-out
## Delivery
Best-effort ordering

© Digital Cloud Training | https://digitalcloud.training
SQS Queue Types
Standard QueueFIFO Queue
Unlimited Throughput: Standard queues support a
nearly unlimited number of transactions per second
(TPS) per API action.
High Throughput: FIFO queues support up to 300
messages per second (300 send, receive, or delete
operations per second). When you batch 10 messages per
operation (maximum), FIFO queues can support up to
3,000 messages per second
Best-Effort Ordering: Occasionally, messages might be
delivered in an order different from which they were
sent
First-ln-First-out Delivery: The order in which messages are
sent and received is strictly preserved
At-Least-Once Delivery: A message is delivered at
least once, but occasionally more than one copy of a
message is delivered
Exactly-Once Processing: A message is delivered once and
remains available until a consumer processes and deletes
it. Duplicates are not introduced into the queue

© Digital Cloud Training | https://digitalcloud.training
SQS Queue Types
•FIFO queues require the Message Group ID and Message
Deduplication ID parameters to be added to messages
•Message Group ID:
•The tag that specifies that a message belongs to a specific
message group Messages that belong to the same message
group are guaranteed to be processed in a FIFO manner
•Message Deduplication ID:
•The token used for deduplication of messages within the
deduplication interval

© Digital Cloud Training | https://digitalcloud.training
SQS – Dead Letter Queue
SQS Queue
## 1
## 5
## 3
## 2
## 6
## 7
## 4
## 8
## Web Tier
## Auto Scaling Group
## Application Tier
## Auto Scaling Group
Dead-Letter Queue
## Analyze Failures
## 4
Message not processed successfully
(ReceiveCount exceeds
maxReceiveCount for queue)
Dead-letter queue is a standard or
FIFO queue that has been specified
as a dead-letter queue

© Digital Cloud Training | https://digitalcloud.training
SQS – Dead Letter Queue
•The main task of a dead-letter queue is handling message failure
•A dead-letter queue lets you set aside and isolate messages that can’t be
processed correctly to determine why their processing didn’t succeed
•It is not a queue type, it is a standard or FIFO queue that has been specified
as a dead-letter queue in the configuration of another standard or FIFO
queue
## Enable Redrive Policy
Specify the queue to use as a dead-letter queue
Specify the maximum receives before a message
is sent to the dead-letter queue

© Digital Cloud Training | https://digitalcloud.training
SQS – Delay Queue
SQS Queue
## 1
## Timeline
## Delay Seconds
## 1
Lambda function
## Producer
Message cannot be
returned
Message is visible
Message is
received
Default 0s, max 15mins

© Digital Cloud Training | https://digitalcloud.training
SQS Long Polling vs Short Polling
SQS Queue
## Consumer
## Producer
## 1
## 5
## 3
## 2
Long polling waits for the
WaitTimeSeconds and
eliminates empty
responses
Short polling checks a
subset of servers and may
not return all messages

© Digital Cloud Training | https://digitalcloud.training
SQS Long Polling vs Short Polling
•SQS Long polling is a way to retrieve messages from SQS queues – waits for
messages to arrive
•SQS Short polling returns immediately (even if the message queue is empty)
•SQS Long polling can lower costs
•SQS Long polling can be enabled at the queue level or at the API level using
WaitTimeSeconds
•SQS Long polling is in effect when the Receive Message Wait Time is a value
greater than 0 seconds and up to 20 seconds
The maximum amount of time that a long
polling receive call will wait for a message to
become available before returning an empty
response.

© Digital Cloud Training | https://digitalcloud.training
Amazon SNS

© Digital Cloud Training | https://digitalcloud.training
Amazon SNS Notifications
## Publisher
Amazon SNS Topic
## Subscribers
## Lambda
## Amazon Simple
## Queue Service
## Web Application
## Email
Te x t
## SMS
Email/Email
## -JSON
## HTTP/HTTPS
## Transport
## Protocols
Event producer sends
one message to one SNS
topic
## Many
subscribers
listen for
notifications
Each subscriber will
get all the messages

© Digital Cloud Training | https://digitalcloud.training
Amazon SNS
•Amazon SNS is a highly available, durable, secure, fully managed pub/sub
messaging service
•Amazon SNS provides topics for high-throughput, push-based, many-to-many
messaging
•Publisher systems can fan out messages to a large number of subscriber
endpoints:
•Endpoints include:
•Amazon SQS queues
•AWS Lambda functions
•HTTP/S webhooks
•Mobile push
## •SMS
•Email

© Digital Cloud Training | https://digitalcloud.training
Amazon SNS
•Multiple recipients can be grouped using Topics
•A topic is an “access point” for allowing recipients to dynamically
subscribe for identical copies of the same notification
•One topic can support deliveries to multiple endpoint types
•Simple APIs and easy integration with applications
•Flexible message delivery over multiple transport protocols

© Digital Cloud Training | https://digitalcloud.training
Amazon SNS + Amazon SQS Fan-Out
•You can subscribe one or more Amazon SQS queues to an Amazon SNS
topic
•Amazon SQS manages the subscription and any necessary permissions
•When you publish a message to a topic, Amazon SNS sends the message
to every subscribed queue
## Queue
## Queue
## Queue
## Topic

© Digital Cloud Training | https://digitalcloud.training
Simple Event-Driven App

© Digital Cloud Training | https://digitalcloud.training
Simple Event-Driven App
Simple-App-Function
SQS Queue
DynamoDB Table
CW Logs
Manually add message to
queue with AWS CLI
Item is written to
DynamoDB table
SQS triggers Lambda
This is the
message body

© Digital Cloud Training | https://digitalcloud.training
AWS Step Functions

© Digital Cloud Training | https://digitalcloud.training
AWS Step Functions
•AWS Step Functions is used to build distributed applications as a series of
steps in a visual workflow
•You can quickly build and run state machines to execute the steps of your
application
How it works:
1.Define the steps of your workflow in the JSON-based Amazon States Language.
The visual console automatically graphs each step in the order of execution
2.Start an execution to visualize and verify the steps of your application are
operating as intended. AWS Step Functions operates and scales the steps of
your application and underlying compute for you to help ensure your
application executes reliably under increasing
demand

© Digital Cloud Training | https://digitalcloud.training
AWS Step Functions
## Do Something
Check Yes/No
Create something
## Wait
## Completed?
Send notification
Check result

© Digital Cloud Training | https://digitalcloud.training
Create a State Machine

© Digital Cloud Training | https://digitalcloud.training
Amazon EventBridge

© Digital Cloud Training | https://digitalcloud.training
Amazon EventBridge
AWS Services
## Custom Apps
SaaS Apps
## Event Sources
## Events
EventBridge
event bus
## Rules
Ta rge t s
Amazon EventBridge is a serverless event bus for
building event-driven applications
EventBridge ingests, filters, transforms, and delivers
events to build loosely-coupled applications

© Digital Cloud Training | https://digitalcloud.training
Amazon EventBridge
•Event Sources – supports events from AWS services,
SaaS applications, and custom applications
•Default and Custom Event Buses – Offers a default
bus for AWS events and supports creating custom
buses for personal or third-party app events
•Event Filtering and Routing – Events can be filtered
and routed to different targets based on content-
based filtering rules
•Scalability and Reliability – scales automatically with
the number of events, handling millions of events
per second

© Digital Cloud Training | https://digitalcloud.training
Amazon EventBridge with Amazon EC2
## Event Source
## Event
## Event Bus
## Rule
Ta rge t
EC2 instance
terminated event
Send SNS
notification

© Digital Cloud Training | https://digitalcloud.training
Amazon EventBridge with AWS CloudTrail
## Event Source
## Event
## Event Bus
## Rule
Ta rge t
S3:PutBucketPolicy
API used
Secure S3 bucket

© Digital Cloud Training | https://digitalcloud.training
Create Event Bus and Rule

© Digital Cloud Training | https://digitalcloud.training
Amazon EventBridge Example 1

© Digital Cloud Training | https://digitalcloud.training
Amazon API Gateway

© Digital Cloud Training | https://digitalcloud.training
REST API with Amazon API Gateway
REST API over HTTPS
Single application
entry point
## Microservices
## Booking Service
## Payment Service
## Account Service
Amazon API Gateway

© Digital Cloud Training | https://digitalcloud.training
REST API with Amazon API Gateway
A resource represents a path in your API
Methods are created within resources and
represent client-facing interfaces by which the
client calls the API to access back-end resources

© Digital Cloud Training | https://digitalcloud.training
REST API with Amazon API Gateway
## Support Email
## Support Ticket
## S3 Website
## Notification
DynamoDB Table
Amazon API Gateway

© Digital Cloud Training | https://digitalcloud.training
Simple HTTP API

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns -
## Serverless

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns - Serverless
Application includes EC2 and RDS.
Spikes in traffic causing writes to be
dropped by RDS
Decouple EC2 and RDS database with
an SQS queue; use Lambda to process
records in the queue
Web app includes a web tier and
processing tier. Must be decoupled and
processing tier should dynamically
scale based on number of jobs
Decouple the web tier and processing
tier with SQS and scale with Auto
Scaling based on the queue length
Lambda function execution time has
increased significantly as the payload
size increased.
Optimize execution time by increasing
memory available to the function which
will proportionally increase CPU
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns - Serverless
Statistical data is stored in RDS and will
be accessed using a REST API. Demand
will range from no traffic to sudden
bursts of traffic and is unpredictable
Create a REST API using Amazon API
Gateway and integrate with an AWS
Lambda function for connecting to RDS
New application processes customer
orders and consists of multiple
decoupled tiers. Orders must be
processed in the order they are received
Implement an Amazon SQS FIFO queue
to preserve the record order
RequirementSolution
App uses API Gateway and Lambda.
During busy periods, many requests fail
multiple times before succeeding. No
errors reported in Lambda
Throttle limit could be configured with
a value that is too low. Increase the
throttle limit

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns - Serverless
EC2 instance processes images using
JavaScript code and stores results in S3.
Load is highly variable. Need a more
cost-effective solution
Replace EC2 with AWS Lambda function
RequirementSolution
App uses API Gateway regional REST
API. Just gone global and performance
has suffered
Convert API to an edge-optimized API to
optimize for the global user base
Legacy application uses many batch
scripts that process data and pass on to
next script. Complex and difficult to
maintain
Migrate scripts to AWS Lambda
functions and use AWS Step Functions
to coordinate components

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns - Serverless
Objects uploaded to an S3 bucket must
be processed by AWS Lambda
Create an event source notification to
notify Lambda function to process new
objects
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## SECTION 12
Databases and Analytics

© Digital Cloud Training | https://digitalcloud.training
Database Types and
## Use Cases

© Digital Cloud Training | https://digitalcloud.training
Relational vs Non-Relational
RelationalNon-Relational
Organized by tables, rows and columnsVaried data storage models
Rigid schema (SQL)Flexible schema (NoSQL) – data stored in key-value
pairs, columns, documents or graphs
Rules enforced within databaseRules can be defined in application code (outside
database)
Typically scaled verticallyScales horizontally
Supports complex queries and joinsUnstructured, simple language that supports any kind
of schema
Amazon RDS, Oracle, MySQL,  IBM DB2,  PostgreSQLAmazon DynamoDB, MongoDB, Redis, Neo4j
Key differences are how data are managed and how data are stored

© Digital Cloud Training | https://digitalcloud.training
## Relational Databases
SELECT FirstName
FROM employees
WHERE Location = Atlanta
Example Structured Query Language (SQL) query:
SQL is used for defining the
structure of the database
and its elements
SQL provides the tools for inserting, updating, deleting,
and querying data within the database table
EmployeeIDFirstNameLastNameJobRoleLocation
00001PaulPetersonSenior DeveloperAtlanta
00002KaleighAnnetteAssistant ManagerMiami
00003CarlWoodSales SupportNew York
00004VinniJonesCustomer ServiceDallas
00005StefanieHowardIT ArchitectLos Angeles

© Digital Cloud Training | https://digitalcloud.training
Non-Relational Databases
clientid
created
skucategorysize
john@example.com
## 1583975308
## SKU-S523
## SKU-J091
## SKU-R873
## SKU-I019
T-Shirt
## Chair
color
## SKU-A234
## Small
## Pen
## Red
## Blue
## Mug
## 30
## Attributes
## Sort  Key
## Partition Key
## Primary Key
## 4011
weight
## Light
## 1583975613
## 1583975449
## 1583976311
## 1583976323
chris@example.com
chris@example.com
sarah@example.com
jenny@example.com
## Plate
NoSQL databases can be key/value and
document stores
This is an example of a key/value store
There is no rigid schema so attributes
can be missing or have different data
types

© Digital Cloud Training | https://digitalcloud.training
## Graph Databases
Graph databases like Amazon Neptune are
designed to store, manage, and navigate
relationships in data
Graph databases use:
•Nodes to represent entities
•Edges to represent
relationships
•Properties to store information
about nodes and edges

© Digital Cloud Training | https://digitalcloud.training
Operational vs Analytical
Operational / transactionalAnalytical
Online Transaction Processing (OLTP)Online Analytics Processing (OLAP) – the source data
comes from OLTP DBs
Production DBs that process transactions. E.g. adding
customer records, checking stock availability (INSERT,
## UPDATE, DELETE)
Data warehouse. Typically, separated from the customer
facing DBs. Data is extracted for decision making
Short transactions and simple queriesLong transactions and complex queries
Relational examples: Amazon RDS, Oracle, IBM DB2,
MySQL
Relational examples: Amazon RedShift, Teradata, HP
## Vertica
Non-relational examples: MongoDB, Cassandra,
Neo4j,  HBase
Non-relational examples: Amazon EMR, MapReduce
Key differences are use cases and how the database is optimized

© Digital Cloud Training | https://digitalcloud.training
Operational vs Analytical
Amazon RDS
Amazon RDS
Amazon RDS
## Amazon Redshift
## COPY
## COPY
## COPY
Operational DBs receive
data from applications
Data Warehouse is
used for analytics

© Digital Cloud Training | https://digitalcloud.training
AWS Databases
Data StoreUse Case
Database on EC2
•Need full control over instance and database
•Third-party database engine (not available in RDS)
Amazon RDS
•Need traditional relational database
•e.g. Oracle, PostgreSQL, Microsoft SQL, MariaDB, MySQL
•Data is well-formed and structured
Amazon DynamoDB
•NoSQL database
•In -memory performance
•High I/O needs
•Dynamic scaling
Amazon RedShift
•Data warehouse for large volumes of aggregated data
Amazon ElastiCache
•Fast temporary storage for small amounts of data
•In -memory database

© Digital Cloud Training | https://digitalcloud.training
## Amazon Relational Database
Service (RDS)

© Digital Cloud Training | https://digitalcloud.training
Amazon RDS
•Managed relational database service
•Used for online transaction processing (OLTP)
use cases
•Runs on Amazon EC2 instances
You must choose the
DB instance type
A DB instance can contain
multiple user-created databases
RDS uses Amazon EBS volumes
for storage
Backups can be taken using
EBS snapshots

© Digital Cloud Training | https://digitalcloud.training
Amazon RDS
Amazon RDS offers a choice of database engines:
•Amazon Aurora – (MySQL and PostgreSQL compatible)
•MySQL –   One of the most popular open-source relational
database management systems
•PostgreSQL – An advanced open-source relational database that
supports both SQL (relational) and JSON (non-relational) querying
•Oracle – Offers support for Oracle Database under two licensing
models: "License Included" and "Bring Your Own License (BYOL)"
•Microsoft SQL Server – Supports several editions of Microsoft SQL
## Server
•MariaDB – A community-developed fork of MySQL intended to
remain free under the GNU GPL

© Digital Cloud Training | https://digitalcloud.training
Amazon RDS – Scaling up (vertically)
M4 instance
## M4 Instance
db.m4.2xlarge 4
vCPUs, 32 GiB RAM
db.m4.large 2 vCPUs,
8 GiB RAM
RDS scales up by changing
the instance type
Scaling up is required for
better write performance
The database must shut
down and restart

© Digital Cloud Training | https://digitalcloud.training
Amazon RDS – Scaling out (horizontally)
RDS scales reads horizontally
with Read Replicas
Applications write to
the primary
Reads can be directed
to the Read Replica
RDS PrimaryRDS Read Replica

© Digital Cloud Training | https://digitalcloud.training
Amazon RDS Multi AZ
## VPC
## Availability Zone
## Availability Zone
Synchronous replication
Asynchronous replication
## Application
## Application
Read Replicas can be in the
same or a different AZ
Multi-AZ standby instances are
in a different AZ to the primary
## .
DB writes
DB reads
Multi-AZ deployments enable
automatic disaster recovery (DR)
RDS Standby
RDS PrimaryRDS Read Replica

© Digital Cloud Training | https://digitalcloud.training
Amazon RDS Backup
and Recovery

© Digital Cloud Training | https://digitalcloud.training
Amazon RDS Automated Backups
## Amazon S3
New DB Instance
## Restore
## Backup
DB Instance
Restore can be to any point in time
during the retention period
Retention is 0–35 days
The DB instance must be in the
available
state for backups to occur
Restored DB instances are
associated with the default DB
parameter and option groups
RDS uploads transaction logs
for DB instances to Amazon
S3 every five minutes
Automated backups can be
replicated to any AWS Region

© Digital Cloud Training | https://digitalcloud.training
Amazon RDS Manual Backups (Snapshot)
•Backs up the entire DB instance, not just individual
databases
•For single-AZ DB instances there is a brief suspension of I/O
•For Multi-AZ SQL Server, I/O activity is briefly suspended on
primary
•For Multi-AZ MariaDB, MySQL, Oracle and PostgreSQL the
snapshot is taken from the standby
•Snapshots do not expire (no retention period)

© Digital Cloud Training | https://digitalcloud.training
Amazon RDS Maintenance Windows
•Operating system and DB patching can require taking the database offline
•These tasks take place during a maintenance window
•By default, a weekly maintenance window is configured
•You can choose your own maintenance window

© Digital Cloud Training | https://digitalcloud.training
## Amazon Aurora Backups
•Aurora backups are continuous and incremental so you can quickly restore to any point
within the backup retention period
•For Amazon Aurora DB clusters, the default backup retention period is one day regardless
of how the DB cluster is created
•You can't disable automated backups on Aurora. The backup retention period for Aurora is
managed by the DB cluster
•You can also use AWS Backup to manage backups of Amazon Aurora DB clusters
•You can also take DB cluster snapshots which capture a snapshot of the entire DB cluster
•Manual snapshots aren't subject to the backup retention period and do not expire
•For very long-term backups, you can export snapshot data to Amazon S3

© Digital Cloud Training | https://digitalcloud.training
## Amazon Aurora Backups
•With Amazon Aurora, you can copy automated backups or manual DB
cluster snapshots
•You can copy a snapshot within the same AWS Region, you can copy a
snapshot across AWS Regions, and you can copy shared snapshots
•Amazon RDS deletes automated backups in several situations:
•At the end of their retention period
•When you disable automated backups for a DB cluster
•When you delete a DB cluster
•If you want to keep an automated backup for a longer period, copy it to
create a manual snapshot

© Digital Cloud Training | https://digitalcloud.training
Create an Amazon RDS
## Database

© Digital Cloud Training | https://digitalcloud.training
Create a Read Replica

© Digital Cloud Training | https://digitalcloud.training
Amazon RDS Security

© Digital Cloud Training | https://digitalcloud.training
Amazon RDS Security
## VPC
## RDS SG
SSL/TLS encryption
## APP SG
<- Allow APP SG port 3306
## Encryption
in-transit
RDS encryption at
rest (AES 256)
## IP
DB Volume
DB Snapshot
Optionally,   a public
IP can enable access
from the Internet

© Digital Cloud Training | https://digitalcloud.training
Amazon RDS Security
•Encryption at rest can be enabled – includes DB storage, backups, read
replicas and snapshots
•You can only enable encryption for an Amazon RDS DB instance when you
create it, not after the DB instance is created
•DB instances that are encrypted can't be modified to disable encryption
•Uses AES 256 encryption and encryption is transparent with minimal
performance impact
•RDS for Oracle and SQL Server is also supported using Transparent Data
Encryption (TDE) (may have performance impact)
•AWS KMS is used for managing encryption keys

© Digital Cloud Training | https://digitalcloud.training
Amazon RDS Security
•You can't have:
•An encrypted read replica of an unencrypted DB instance
•An unencrypted read replica of an encrypted DB instance
•Read replicas of encrypted primary instances are encrypted
•The same KMS key is used if in the same Region as the primary
•If the read replica is in a different Region, a different KMS key is
used
•You can't restore an unencrypted backup or snapshot to an
encrypted DB instance

© Digital Cloud Training | https://digitalcloud.training
Amazon RDS Security
## Snapshot
## (unencrypted)
EBS Volume
## (unencrypted)
RDS (unencrypted)
## Snapshot
## (encrypted)
## COPY
EBS Volume
## (encrypted)
RDS (encrypted)
New instance with
new endpoint
Restore from
snapshot

© Digital Cloud Training | https://digitalcloud.training
Create Encrypted Copy of
RDS Database

© Digital Cloud Training | https://digitalcloud.training
Amazon RDS Security
## Snapshot
## (unencrypted)
EBS Volume
## (unencrypted)
RDS (unencrypted)
## Snapshot
## (encrypted)
## COPY
EBS Volume
## (encrypted)
RDS (encrypted)
New instance with
new endpoint
Restore from
snapshot

© Digital Cloud Training | https://digitalcloud.training
## Amazon Aurora

© Digital Cloud Training | https://digitalcloud.training
## Amazon Aurora
•Amazon Aurora is an AWS database offering in the RDS family
•Amazon Aurora is a MySQL and PostgreSQL-compatiblerelational
databasebuilt for the cloud
•Amazon Aurora is up to five times faster than
standardMySQLdatabases and three times faster than standard
PostgreSQL databases
•Amazon Aurora features a distributed, fault-tolerant, self-healing
storage system that auto-scales up to 128TB per database
instance

© Digital Cloud Training | https://digitalcloud.training
Aurora Fault Tolerance and Aurora Replicas
Availability ZoneAvailability ZoneAvailability Zone
## Primary
## Data Copies
## Data Copies
## Data Copies
## Replica
ReplicaReplica
## Writes
## Writes
## Writes
## Reads
## Reads
## Reads
## Reads
## Region
## Single Logical Volume
## Aurora Fault Tolerance
•Fault tolerance across 3 AZs
•Single logical volume
•Aurora Replicas scale-out read
requests
•Up to 15 Aurora Replicas with
sub-10ms replica lag
•Aurora Replicas are
independent endpoints
•Can promote Aurora Replica to
be a new primary or create
new primary
•Set priority (tiers) on Aurora
Replicas to control order of
promotion
•Can use Auto Scaling to add
replicas
Aurora Replicas are within a region

© Digital Cloud Training | https://digitalcloud.training
## Amazon Aurora Key Features
Aurora FeatureBenefit
High performance and scalability
Offers high performance, self-healing storage that scales up to 128TB, point-
in -time recovery and continuous backup to S3
DB compatibilityCompatible with existing MySQL and PostgreSQL open-source databases
Aurora ReplicasIn-region read scaling and failover target – up to 15 (can use Auto Scaling)
MySQL Read Replicas
Cross-region cluster with read scaling and failover target (each can have up
to 15 Aurora Replicas)
## Global Database
Cross-region cluster with read scaling (fast replication / low latency reads).
Can remove secondary and promote
ServerlessOn-demand, autoscaling configuration for Amazon Aurora

© Digital Cloud Training | https://digitalcloud.training
## Amazon Aurora Replicas
FeatureAurora ReplicaMySQL Replica
Number of replicasUp to 15Up to 5
Replication typeAsynchronous (milliseconds)Asynchronous (seconds)
Performance impact on primaryLowHigh
Replica locationIn-regionCross-region
Act as failover targetYes (no data loss)
Yes (potentially minutes of
data loss)
Automated failoverYe sNo
Support for user-defined replication delayNoYe s
Support for different data or schema vs. primaryNoYe s

© Digital Cloud Training | https://digitalcloud.training
## Amazon Aurora Deployment
## Options

© Digital Cloud Training | https://digitalcloud.training
Aurora Fault Tolerance and Aurora Replicas
Availability ZoneAvailability ZoneAvailability Zone
## Primary
## Data Copies
## Data Copies
## Data Copies
## Replica
ReplicaReplica
## Writes
## Writes
## Writes
## Reads
## Reads
## Reads
## Reads
## Region
## Single Logical Volume
## Aurora Fault Tolerance
•Fault tolerance across 3 AZs
•Single logical volume
•Aurora Replicas scale-out read
requests
•Up to 15 Aurora Replicas with
sub-10ms replica lag
•Aurora Replicas are
independent endpoints
•Can promote Aurora Replica to
be a new primary or create
new primary
•Set priority (tiers) on Aurora
Replicas to control order of
promotion
•Can use Auto Scaling to add
replicas
Aurora Replicas are within a region

© Digital Cloud Training | https://digitalcloud.training
Cross-Region Replica with Aurora MySQL
## Region
## Availability
## Zone
## Availability
## Zone
## Availability
## Zone
## Writes
## Writes
## Region
## Availability
## Zone
## Availability
## Zone
## Availability
## Zone
## Reads
## Reads
## Asynchronous
replication
## Region
## Availability
## Zone
## Availability
## Zone
## Availability
## Zone
## Reads
## Reads
Asynchronous replication
## Primary Region
Replication uses the MySQL
database engine

© Digital Cloud Training | https://digitalcloud.training
## Aurora Global Database
## Region
## Availability
## Zone
## Availability
## Zone
## Availability
## Zone
## Writes
## Writes
## Region
## Availability
## Zone
## Availability
## Zone
## Availability
## Zone
## Reads
## Reads
## Asynchronous
replication
## Primary Region
## Secondary Region
Applications can connect to the
cluster Reader Endpoint
Replication uses the
Aurora storage layer
A database in a secondary Region can
be promoted to full read/write
capabilities in less than 1 minute
Secondary clusters can be configured
with write-forwarding

© Digital Cloud Training | https://digitalcloud.training
## Aurora Serverless
ACU assigned ->
## App Server
## Database
## Storage
Warm pool of
capacity
Router fleet
## Each Aurora Capacity
Unit (ACU) is 2 GB of
memory plus CPU
Capacity seamlessly
scales up and down

© Digital Cloud Training | https://digitalcloud.training
## Aurora Serverless Use Cases
•Infrequently used applications
•New applications
•Variable workloads
•Unpredictable workloads
•Development and test databases
•Multi-tenant applications

© Digital Cloud Training | https://digitalcloud.training
Amazon RDS Proxy

© Digital Cloud Training | https://digitalcloud.training
Amazon RDS Proxy
## Connection Pool
•Reduces stress on CPU/MEM
•Shares infrequently used connections
•Drives increased efficiency
•High availability with failover
•Control authentication methods
•RDS Proxy is a fully managed database proxy for RDS
•Highly available across multiple AZs
•Increases scalability, fault tolerance, and security

© Digital Cloud Training | https://digitalcloud.training
Amazon ElastiCache

© Digital Cloud Training | https://digitalcloud.training
Amazon ElastiCache
•Fully managed implementations Redis and Memcached
•ElastiCache is a key/value store
•In-memory database offering high performance and low latency
•Can be put in front of databases such as RDS and DynamoDB
•ElastiCache nodes run on Amazon EC2 instances, so you must choose an instance
family/type
## Instance
ElastiCache
## Node
Amazon RDS
Load data
Cache hit
Database write

© Digital Cloud Training | https://digitalcloud.training
Amazon ElastiCache
FeatureMemcachedRedis (cluster mode disabled)Redis (cluster mode enabled)
Data persistenceNoYe sYe s
Data typesSimpleComplexComplex
Data partitioningYe sNoYe s
EncryptionNoYe sYe s
High availability (replication)NoYe sYe s
Multi-AZ
Yes, place nodes in multiple AZs.
No failover or replication
Yes, with auto-failover. Uses read replicas (0-5
per shard)
Yes, with auto-failover. Uses read replicas (0-5
per shard)
ScalingUp (node type); out (add nodes)Up (node type); out (add replica)Up (node type); out (add shards)
MultithreadedYe sNoNo
Backup and restoreNo (and no snapshots)Yes, automatic and manual snapshotsYes, automatic and manual snapshots

© Digital Cloud Training | https://digitalcloud.training
Amazon ElastiCache Use Cases
•Data that is relatively static and frequently accessed
•Applications that are tolerant of stale data
•Data is slow and expensive to get compared to cache retrieval
•Require push-button scalability for memory, writes and reads
•Often used for storing session state

© Digital Cloud Training | https://digitalcloud.training
Amazon ElastiCache Examples
Use CaseBenefit
Web session storeIn cases with load-balanced web servers, store web session information in Redis so if a server is
lost, the session info is not lost, and another web server can pick it up
Database cachingUse Memcached in front of AWS RDS to cache popular queries to offload work from RDS and
return results faster to users
LeaderboardsUse Redis to provide a live leaderboard for millions of users of your mobile app
Streaming data dashboardsProvide a landing spot for streaming sensor data on the factory floor, providing live real-time
dashboard displays

© Digital Cloud Training | https://digitalcloud.training
Scaling ElastiCache

© Digital Cloud Training | https://digitalcloud.training
Amazon ElastiCache - Scalability
## Memcached
•Add nodes to a cluster
•Scale vertically (node type) – must create a new cluster manually
## Redis
•Cluster mode disabled:
•Add replica or change node type – creates a new cluster and migrates data
•Cluster mode enabled:
•Online resharding to add or remove shards; vertical scaling to change node type
•Offline resharding to add or remove shards change node type or upgrade engine (more
flexible than online)

© Digital Cloud Training | https://digitalcloud.training
Amazon ElastiCache Memcached
## Region A
## Availability Zone A
## Node 2
## Availability Zone B
## Node 4
## Node 1
## Node 5
ElastiCache Memcached Cluster
## Node 3
Node n
Each node is a
partition of data

© Digital Cloud Training | https://digitalcloud.training
Amazon ElastiCache Redis (Cluster mode enabled)
## Region A
## Availability Zone A
## Shard
## Replica 1
## Availability Zone B
## Replica 2
## Primary
ElastiCache Redis Cluster
## Shard
## Replica 1
## Replica 2
## Primary
## Shard
## Replica 1
## Replica 2
## Primary

© Digital Cloud Training | https://digitalcloud.training
Amazon ElastiCache Redis (Cluster mode disabled)
## Region A
## Availability Zone A
## Shard
## Replica
## Availability Zone B
## Replica
## Primary
## Replica
ElastiCache Redis Cluster
Can failover to a
replica

© Digital Cloud Training | https://digitalcloud.training
Amazon DynamoDB

© Digital Cloud Training | https://digitalcloud.training
Amazon DynamoDB
•Fully managed NoSQL database service
•Key/value store and document store
•It is a non-relational, key-value type of database
•Fully serverless service
•Push button scaling
DynamoDB Table

© Digital Cloud Training | https://digitalcloud.training
Amazon DynamoDB
•DynamoDB is made up of:
•Tables
•Items
•Attributes
useridorderidbook
user0011000092
price
## ISBN100..
## 1000102
## 1000168
date
user002
user003
## ISBN100..
## ISBN2X0..
## 9.992020.04..
## 2020.03..
## 2020.04..
## 24.99
## 12.50

© Digital Cloud Training | https://digitalcloud.training
DynamoDB Time to Live (TTL)
•TTL lets you define when items in a table
expire so that they can be automatically
deleted from the database
•With TTL enabled on a table, you can set a
timestamp for deletion on a per-item basis
•No extra cost and does not use WCU / RCU
•Helps reduce storage and manage the table
size over time

© Digital Cloud Training | https://digitalcloud.training
Amazon DynamoDB
clientid
created
skucategorysize
john@example.com
## 1583975308
## SKU-S523
## SKU-J091
## SKU-R873
## SKU-I019
T-Shirt
## Chair
colour
## SKU-A234
## Small
## Pen
## Red
## Blue
## Mug
## 30
## Attributes
## Sort  Key
## Partition
## Key
## Primary Key
## 4011
weight
## Light
## 1583975613
## 1583975449
## 1583976311
## 1583976323
chris@example.com
chris@example.com
sarah@example.com
jenny@example.com
## Plate
This is known as a
composite key as it has a
partition key + sort key
Useful when the data
structure is unpredictable

© Digital Cloud Training | https://digitalcloud.training
Amazon DynamoDB
DynamoDB FeatureBenefit
ServerlessFully managed, fault tolerant, service
Highly available99.99% availability SLA – 99.999% for Global Tables!
NoSQL type of database with Name / Value
structure
Flexible schema, good for when data is not well structured or unpredictable
Horizontal scalingSeamless scalability to any scale with push button scaling or Auto Scaling
DynamoDB Streams
Captures a time-ordered sequence of item-level modifications in a DynamoDB table and durably stores
the information for up to 24 hours. Often used with Lambda and the Kinesis Client Library (KCL)
DynamoDB Accelerator (DAX)Fully managed in-memory cache for DynamoDB that increases performance (microsecond latency)
Transaction optionsStrongly consistent or eventually consistent reads, support for ACID transactions
BackupPoint-in -time recovery down to the second in last 35 days; On-demand backup and restore
Global TablesFully managed multi-region, multi-master solution

© Digital Cloud Training | https://digitalcloud.training
Practice Creating DynamoDB
## Tables

© Digital Cloud Training | https://digitalcloud.training
## Practice Creating
DynamoDB Tables

© Digital Cloud Training | https://digitalcloud.training
DynamoDB Streams

© Digital Cloud Training | https://digitalcloud.training
DynamoDB Streams
1.Application inserts / updates /deletes item
2.A record is written to the DynamoDB stream
3.A Lambda function is triggered
4.The Lambda function writes to CloudWatch
## Logs
DynamoDB Stream
DynamoDB Table
## Application
## 1
## 2
AWS Lambda
Amazon CloudWatch
## 3
## 4

© Digital Cloud Training | https://digitalcloud.training
DynamoDB Streams
•Captures a time-ordered sequence of item-level
modifications in any DynamoDB table and stores this
information in a log for up to 24 hours
•Can configure the information that is written to the
stream:
•KEYS_ONLY — Only the key attributes of the modified
item
•NEW_IMAGE — The entire item, as it appears after it was
modified
•OLD_IMAGE — The entire item, as it appeared before it
was modified
•NEW_AND_OLD_IMAGES — Both the new and the old
images of the item

© Digital Cloud Training | https://digitalcloud.training
DynamoDB Accelerator (DAX)

© Digital Cloud Training | https://digitalcloud.training
DynamoDB Accelerator (DAX)
•DAX is a fully managed, highly available, in -memory cache
for DynamoDB
•Improves performance from milliseconds to microseconds
•Can be a read-through cache and a write-through cache
•Used to improve READ and WRITE performance
•You do not need to modify application logic, since DAX is
compatible with existing DynamoDB API calls

© Digital Cloud Training | https://digitalcloud.training
DynamoDB Accelerator (DAX)
AWS Cloud
Amazon DynamoDB
## DAX
EC2 Instance
IAM Role
## VPC
IAM Role
## Permissions:
•Access DynamoDB + DAX
## Permissions:
•Access DynamoDB
Security group
Inbound rules:
•TCP 8000 (DynamoDB) from 0.0.0.0/0
•TCP 8111 (DAX) from 0.0.0.0/0

© Digital Cloud Training | https://digitalcloud.training
DAX vs ElastiCache
•DAX is optimized for DynamoDB
•With ElastiCache you have more management
overhead (e.g. invalidation)
•With ElastiCache you need to modify application
code to point to cache
•ElastiCache supports more datastores

© Digital Cloud Training | https://digitalcloud.training
DynamoDB Global Tables

© Digital Cloud Training | https://digitalcloud.training
DynamoDB Global Tables
## Region A
Amazon DynamoDB
## App Server
ReadWrite
## Region B
Amazon DynamoDB
## App Server
## Asynchronous
replication
## Write
## Region C
Amazon DynamoDB
## App Server
ReadWrite
## Read
## Asynchronous
replication
Global Tables is a
Multi-region, multi-
active database
Each replica table
stores the same
set of data items
Use logic in the
application to
failover to a
replica region

© Digital Cloud Training | https://digitalcloud.training
## Enable Global Table

© Digital Cloud Training | https://digitalcloud.training
Amazon RedShift

© Digital Cloud Training | https://digitalcloud.training
Amazon RedShift
•Amazon Redshift is a fast, fully managed data warehouse
•Analyze data using standard SQL and existing Business Intelligence (BI)
tools
•RedShift is a SQL based data warehouse used for analytics applications
•RedShift is a relational database that is used for Online Analytics
Processing (OLAP) use cases
•RedShift uses Amazon EC2 instances, so you must choose an instance
family/type
•RedShift always keeps three copies of your data
•RedShift provides continuous/incremental backups

© Digital Cloud Training | https://digitalcloud.training
OLTP vs OLAP (refresher)
Operational / transactionalAnalytical
Online Transaction Processing (OLTP)Online Analytics Processing (OLAP) – the source
data comes from OLTP DBs
Production DBs that process transactions. E.g.
adding customer records, checking stock
availability (INSERT, UPDATE, DELETE)
Data warehouse. Typically, separated from the
customer facing DBs. Data is extracted for
decision making
Short transactions and simple queriesLong transactions and complex queries
Examples: Amazon RDS, DynamoDBExamples: Amazon RedShift, Amazon EMR
Key differences are use cases and how the database is optimized

© Digital Cloud Training | https://digitalcloud.training
Reporting and Analytics Use Cases
Amazon RDSAmazon RDS
## Amazon Redshift
## COPY
## COPY
## Reporting Tool
Production transactional
database for customer orders
Amazon RDS
## Read Replica
Reporting tool runs
against live data
Production DBs for
additional geographies
Data is loaded
into RedShift
Data can be analyzed
with BI tools such as
QuickSight using SQL
## JDBC/ODBC

© Digital Cloud Training | https://digitalcloud.training
## Redshift Data Sources
## Amazon Redshift
Amazon DynamoDB
Amazon RDS
## Amazon S3
Amazon EMR
AWS Glue
AWS Data Pipeline
Amazon EC2
On-Premises Server
RedShift Spectrum can
run SQL queries on data
directly in S3

© Digital Cloud Training | https://digitalcloud.training
RedShift Use Cases
•Perform complex queries on massive collections of
structured and semi-structured data and get fast
performance
•Frequently accessed data that needs a consistent,
highly structured format
•Use Spectrum for direct access of S3 objects in a data
lake
•Managed data warehouse solution with:
•Automated provisioning, configuration and patching
•Data durability with continuous backup to S3
•Scales with simple API calls
•Exabyte scale query capability

© Digital Cloud Training | https://digitalcloud.training
## Amazon Elastic Map Reduce
## (EMR)

© Digital Cloud Training | https://digitalcloud.training
Amazon EMR
•Managed cluster platform that simplifies running
big data frameworks including Apache Hadoop
and Apache Spark
•Used for processing data for analytics and business
intelligence
•Can also be used for transforming and moving
large amounts of data
•Performs extract, transform, and load (ETL)
functions

© Digital Cloud Training | https://digitalcloud.training
Amazon EMR
## Availability Zone
Amazon EMR
## Cluster
AWS Cloud
## Amazon S3
Amazon DynamoDB
## Amazon Redshift
## Amazon S3 Glacier
Amazon RDS
## HDFS
EBS volume
ClusterCluster
Data Store options
Optionally attach
EBS volumes
Root access to
cluster instances
Scale cluster instances
or deploy multiple
clusters

© Digital Cloud Training | https://digitalcloud.training
## Amazon Kinesis

© Digital Cloud Training | https://digitalcloud.training
## Amazon Kinesis Services
## Amazon Kinesis
## Data Streams
## Data Sources
## Amazon Kinesis
## Data Analytics
## Amazon Kinesis
## Data Firehose
## Amazon S3
## Amazon Athena
## Amazon Redshift
Amazon QuickSight
AWS Lambda
Amazon DynamoDB
Data Analytics uses Apache
Flink for processing data
streams
Data is ingested into
## Data Streams
Firehose loads data
straight to destinations

© Digital Cloud Training | https://digitalcloud.training
## Amazon Kinesis Data Streams
•Producers send data to Kinesis, data is stored in Shards
for 24 hours (by default, up to 365 days)
•Consumers then take the data and process it - data can
then be saved into another AWS service
•Real time (~200ms)
## Shards
## Stream
## Amazon S3
Amazon DynamoDB
Amazon RedShift
Amazon EMR
## Kinesis Firehose
## Destinations
## Analytics Tools
Consumers process the
data and save to
destinations
Producers capture and
send data to Kinesis
Data is captured and stored
for processing

© Digital Cloud Training | https://digitalcloud.training
Kinesis Client Library (KCL)
•The Kinesis Client Library (KCL) helps you consume and
process data from a Kinesis data stream
## Shards
## Kinesis Data Stream
EC2 Instance
EC2 Instance
## KCL
## KCL
KCL enumerates shards and
instantiates a record processor for
each shard it manages
KCL Worker with multiple
record processors

© Digital Cloud Training | https://digitalcloud.training
Kinesis Client Library (KCL)
•Each shard is processed by exactly one KCL worker and has exactly
one corresponding record processor
•One worker can process any number of shards, so it's fine if the
number of shards exceeds the number of instances
## Shards
## Kinesis Data Stream
EC2 Instance
EC2 Instance
## KCL
## KCL
Each shard is processed
by exactly one KCL
worker
A record processor maps to
exactly one shard

© Digital Cloud Training | https://digitalcloud.training
## Amazon Kinesis Data Streams
## Stream
## Producers
## (EC2)
## 1
## 2
## 3
## 4
## 5
## 1
## 1
## 2
## 1
## 5
## 5
## 1
EC2 Instance
EC2 Instance
## KCL
## KCL
## Shards:
Order is maintained for
records within a shard
A partition key can be specified
with PutRecord to group data by
shard

© Digital Cloud Training | https://digitalcloud.training
## Kinesis Data Firehose
•Producers send data to Firehose
•There are no Shards, completely automated (scalability is elastic)
•Firehose data is sent to another AWS service for storing, data can be
optionally processed/transformed using AWS Lambda
•Near real-time delivery (~60 seconds latency)
## Amazon S3
Amazon RedShift
## Destinations
## Amazon Elasticsearch
## Analytics Tools
## Optional Lambda
transformation
Firehose captures, transforms
and loads streaming data
Data is loaded
continuously to
destinations

© Digital Cloud Training | https://digitalcloud.training
## Kinesis Data Firehose
Kinesis Data Firehose destinations (changes over time):
•RedShift (via an intermediate S3 bucket)
•OpenSearch
•Amazon S3
•Splunk
•Datadog
•Honeycomb
•Coralogix
•LogicMonitor
•Logz.io
•MongoDB
•New Relic
•Sumo Logic
•HTTP Endpoint

© Digital Cloud Training | https://digitalcloud.training
## Kinesis Data Analytics
•Provides real-time SQL processing for streaming data
•Provides analytics for data coming in from Kinesis Data Streams and
## Kinesis Data Firehose
•Destinations can be Kinesis Data Streams, Kinesis Data Firehose, or
AWS Lambda
## Amazon Kinesis
## Data Streams
## Amazon Kinesis
## Data Analytics
AWS Lambda
## Amazon Kinesis
## Data Firehose
## Data Sources
Run SQL queries on real-
time streaming data

© Digital Cloud Training | https://digitalcloud.training
Amazon Athena and AWS
## Glue

© Digital Cloud Training | https://digitalcloud.training
Amazon Athena and AWS Glue
Data Lake on Amazon S3
## Amazon Athena
AWS Glue
Athena can query
data in CSV, TSV,
JSON, Parquet and
ORC formats
Point Athena at data
source in S3 and then
run SQL queries
AWS Glue is used as a
metadata catalog (can
also use Apache Hive)

© Digital Cloud Training | https://digitalcloud.training
Amazon Athena and AWS Glue
## Amazon Athena
Data from source is
mapped in tables in
Athena and is queryable
Lambda function
A Lambda function
connects Athena to
data source
SQL queries can also be
run against these data
sources

© Digital Cloud Training | https://digitalcloud.training
## Amazon Athena
•Athena queries data in S3 using SQL
•Can be connected to other data sources with Lambda
•Data can be in CSV, TSV, JSON, Parquet and ORC
formats
•Uses a managed Data Catalog (AWS Glue) to store
information and schemas about the databases and
tables

© Digital Cloud Training | https://digitalcloud.training
Optimizing Athena for Performance
•Partition your data
•Bucket your data – bucket the data within a single
partition
•Use Compression – AWS recommend using either
Apache Parquet or Apache ORC
•Optimize file sizes
•Optimize columnar data store generation – Apache
Parquet and Apache ORC are popular columnar data
stores
•Optimize ORDER BY and Optimize GROUP BY
•Use approximate functions
•Only include the columns that you need

© Digital Cloud Training | https://digitalcloud.training
AWS Glue
•Fully managed extract, transform and load (ETL)
service
•Used for preparing data for analytics
•AWS Glue runs the ETL jobs on a fully managed,
scale-out Apache Spark environment
•AWS Glue discovers data and stores the associated
metadata (e.g. table definition and schema) in the
AWS Glue Data Catalog
•Works with data lakes (e.g. data on S3), data
warehouses (including RedShift), and data stores
(including RDS or EC2 databases)

© Digital Cloud Training | https://digitalcloud.training
AWS Glue
•You can use a crawler to populate the AWS Glue
Data Catalog with tables
•A crawler can crawl multiple data stores in a single
run
•Upon completion, the crawler creates or updates
one or more tables in your Data Catalog.
•ETL jobs that you define in AWS Glue use the Data
Catalog tables as sources and targets

© Digital Cloud Training | https://digitalcloud.training
Query S3 ALB Access Logs
with Athena

© Digital Cloud Training | https://digitalcloud.training
Amazon OpenSearch Service
(Elasticsearch)

© Digital Cloud Training | https://digitalcloud.training
Amazon OpenSearch Service
Amazon OpenSearch Service
Successor to Amazon
## Elasticsearch Service
Search, visualize, and
analyze text and
unstructured data
Deploy to Amazon VPC
and integrates with IAM
Deploy nodes and
replicas across AZs

© Digital Cloud Training | https://digitalcloud.training
Amazon OpenSearch Service
•Distributed search and analytics suite
•Based on the popular open source Elasticsearch
•Supports queries using SQL syntax
•Integrates with open-source tools
•Scale by adding or removing instances
•Availability in up to three Availability Zones
•Backup using snapshots
•Encryption at-rest and in-transit

© Digital Cloud Training | https://digitalcloud.training
OpenSearch Service Deployment
•Clusters are created (Management Console, API,
or CLI)
•Clusters are also known as OpenSearch Service
domains
•You specify the number of instances and instance
types
•Storage options include UltraWarm or Cold
storage

© Digital Cloud Training | https://digitalcloud.training
Ingesting Data into OpenSearch Service Domains
## Amazon Kinesis
## Data Firehose
Amazon OpenSearch
## Service
## Logstash
## Elasticsearch /
OpenSearch API
## Kibana Dashboard
Search, visualize, and
analyze data
Data is ingested from
multiple sources

© Digital Cloud Training | https://digitalcloud.training
OpenSearch in an Amazon VPC
•Clusters can be deployed in a VPC for secure intra-
VPC communications
•VPN or proxy required to connect from the
internet (public domains are directly accessible)
•Cannot use IP-based access policies

© Digital Cloud Training | https://digitalcloud.training
OpenSearch in an Amazon VPC
•Limitations of VPC deployments:
•You can’t switch from VPC to a public endpoint. The
reverse is also true
•You can’t launch your domain within a VPC that uses
dedicated tenancy
•After you place a domain within a VPC, you can’t
move it to a different VPC, but you can change the
subnets and security group settings

© Digital Cloud Training | https://digitalcloud.training
The ELK Stack
•ELK stands for Elasticsearch, Logstash, and Kibana
•This is a popular combination of projects
•Aggregate logs from systems and applications,
analyze these logs, and create visualizations
•Use cases include:
•Visualizing application and infrastructure monitoring data
•Troubleshooting
•Security analytics
Amazon OpenSearch
## Service
## Logstash
## Kibana Dashboard

© Digital Cloud Training | https://digitalcloud.training
OpenSearch Access Control
•Resource-based policies – often called a domain
access policy
•Identity-based policies – attached to users or roles
## (principals)
•IP-based policies – Restrict access to one or more IP
addresses or CIDR blocks
•Fine-grained access control – Provides:
•Role-based access control
•Security at the index, document, and field level
•OpenSearch Dashboards multi-tenancy
•HTTP basic authentication for OpenSearch and
OpenSearch Dashboards

© Digital Cloud Training | https://digitalcloud.training
OpenSearch Access Control
•Authentication options include:
•Federation using SAML to on-premises directories
•Amazon Cognito and social identity providers

© Digital Cloud Training | https://digitalcloud.training
OpenSearch Best Practices
•Deploy OpenSearch data instances across three
Availability Zones (AZs) for the best availability
•Provision instances in multiples of three for equal
distribution across AZs
•If three AZs are not available use two AZs with equal
numbers of instances

© Digital Cloud Training | https://digitalcloud.training
OpenSearch Best Practices
•Use three dedicated master nodes
•Configure at least one replica for each index
•Apply restrictive resource-based access policies to
the domain (or use fine-grained access control)
•Create the domain within an Amazon VPC
•For sensitive data enable node-to-node encryption
and encryption at rest

© Digital Cloud Training | https://digitalcloud.training
AWS Batch

© Digital Cloud Training | https://digitalcloud.training
AWS Batch
Launch a Batch Job
## Job Definition
## Job Queue
## Batch Compute Environment

© Digital Cloud Training | https://digitalcloud.training
## Optimize Containers
•Small containers (< 4GB)
•Offload libraries to AMI
•Bind mounts
•Small layers (< 2GB)
•Use Amazon ECR as container registry
•Use Fargate for fastest start times

© Digital Cloud Training | https://digitalcloud.training
## Other Database
## Services

© Digital Cloud Training | https://digitalcloud.training
Amazon DocumentDB
•Amazon DocumentDB provides MongoDB compatibility
•It is a database service that is purpose-built for JSON data
management at scale

© Digital Cloud Training | https://digitalcloud.training
Amazon DocumentDB
•Fully managed service
•Storage scales automatically up to 64 TB without
any impact to your application
•Supports millions of requests per second with up
to 15 low latency read replicas
•Designed for 99.99% availability and replicates six
copies of your data across three AZs
•Can migrate from MongoDB using the AWS
Database Migration Service (AWS DMS)

© Digital Cloud Training | https://digitalcloud.training
## Amazon Keyspaces (for Apache Cassandra)
•A scalable, highly available, and managed Apache
Cassandra–compatible database service
•Keyspaces enables you to use the Cassandra Query
Language (CQL) API code
•Keyspaces is serverless and fully managed
•Scales automatically in response to application traffic
•Can serve thousands of requests per second with
virtually unlimited throughput and storage
•Consistent, single-digit-millisecond response times at
any scale
•99.99% availability SLA within an AWS Region

© Digital Cloud Training | https://digitalcloud.training
## Amazon Neptune
•Fully managed graph database service
•Build and run identity, knowledge, fraud
graph, and other applications
•Deploy high performance graph applications
using popular open-source APIs including:
•Gremlin
•openCypher
## •S PA RQ L
•Offers greater than 99.99% availability
•Storage is fault-tolerant and self-healing
•DB volumes grow in increments of 10 GB up
to a maximum of 64 TB
•Create up to 15 database read replicas

© Digital Cloud Training | https://digitalcloud.training
## Amazon Quantum Ledger Database
•Amazon QLDB  is a fully managed ledger database that
provides a transparent, immutable, and cryptographically
verifiable transaction log
•Amazon QLDB has a built-in immutable journal that stores
an accurate and sequenced entry of every data change
•The journal is append-only, meaning that data can only be
added to a journal, and it cannot be overwritten or deleted
•Amazon QLDB uses cryptography to create a concise
summary of your change history
•Generated using a cryptographic hash function (SHA-256)
•Serverless and offers automatic scalability

© Digital Cloud Training | https://digitalcloud.training
## Other Analytics
## Services

© Digital Cloud Training | https://digitalcloud.training
## Amazon Timestream
•Time series database service for IoT and
operational applications
•Faster and cheaper than relational databases
•Keeps recent data in memory and moves
historical data to a cost optimized storage tier
based upon user defined policies
•Serverless and scales automatically

© Digital Cloud Training | https://digitalcloud.training
AWS Data Exchange
•AWS Data Exchange is a data marketplace with over
3,000 products from 250+ providers
•AWS Data Exchange supports Data Files, Data Tables,
and Data APIs
•Consume directly into data lakes, applications,
analytics, and machine learning models
•Automatically export new or updated data sets to
## Amazon S3
•Query data tables with AWS Data Exchange for
## Amazon Redshift
•Use AWS-native authentication and governance,
AWS SDKs, and consistent API documentation

© Digital Cloud Training | https://digitalcloud.training
AWS Data Exchange - Benefits

© Digital Cloud Training | https://digitalcloud.training
AWS Data Pipeline
•AWS Data Pipeline is a managed ETL (Extract-
Transform-Load) service
•Process and move data between different AWS
compute and storage services
•Data sources can also be on-premises
•Data can be processed and transformed
•Results can be loaded to services such as Amazon
S3, Amazon RDS, Amazon DynamoDB, and
Amazon EMR

© Digital Cloud Training | https://digitalcloud.training
AWS Data Pipeline – Clickstream Data Example
Clickstream data
HiveActivity
## Pipeline
HiveActivity converts log
files to .csv using EMR
Results saved to S3
RedShiftCopyActivity loads to
RedShift

© Digital Cloud Training | https://digitalcloud.training
What is a Data Lake?
A data lake is a centralized
repository that allows you
to store all your
structured and
unstructured data at any
scale
You can store your data
as-is, without having to
first structure the data
Can create dashboards,
and visualizations
Big data processing, real-
time analytics, ML

© Digital Cloud Training | https://digitalcloud.training
Data Warehouse vs Data Lake
CharacteristicsData WarehouseData Lake
## Data
Relational from transactional systems,
operational databases, and line of
business applications
Non-relational and relational from IoT devices,
web sites, mobile apps, social media, and
corporate applications
## Schema
Designed prior to the DW implementation
## (schema-on-write)
Written at the time of analysis (schema-on-
read)
Price/Performance
Fastest query results using higher cost
storage
Query results getting faster using low-cost
storage
Data QualityHighly curated data that serves as the
central version of the truth
Any data that may or may not be curated (ie.
raw data)
UsersBusiness analysts
Data scientists, Data developers, and Business
analysts (using curated data)
AnalyticsBatch reporting, BI and visualizations
Machine Learning, Predictive analytics, data
discovery and profiling

© Digital Cloud Training | https://digitalcloud.training
AWS Lake Formation
•AWS Lake Formation enables you to set up secure data
lakes in days
•Data can be collected from databases and object storage
•It is saved to the Amazon S3 data lake
•You can then clean and classify data using ML algorithms
•Security can be applied at column, row, and cell-levels
•The data sets can then be used through services such as
Amazon Redshift, Amazon Athena, Amazon EMR for
Apache Spark, and Amazon QuickSight
•Lake Formation builds on the capabilities available in AWS
## Glue

© Digital Cloud Training | https://digitalcloud.training
Amazon Managed Streaming for Apache Kafka (MSK)
•Amazon MSK is used for ingesting and processing
streaming data in real-time
•Build and run Apache Kafka applications
•It is a fully managed service
•Provisions, configures, and maintains Apache Kafka
clusters and Apache ZooKeeper nodes
•Security levels include:
•VPC network isolation
•AWS IAM for control-plane API authorization
•Encryption at rest
•TLS encryption in-transit
•TLS based certificate authentication
•SASL/SCRAM authentication secured by AWS Secrets
## Manager

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns –
Databases and Analytics

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns – Databases & Analytics
Relational database running on MySQL
must be migrated to AWS and must be
highly available
Use Amazon RDS MySQL and configure
a Multi-AZ standby node for HA
Amazon RDS DB has high query traffic
that is causing performance
degradation
Create a Read Replica and configure the
application to use the reader endpoint
for database queries
Amazon RDS DB is approaching its
storage capacity limits and/or is
suffering from high write latency
Scale up the DB instance to an instance
type that has more storage / CPU
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns – Databases & Analytics
Amazon RDS database is unencrypted
and a cross-Region read replica must
be created with encryption
Encrypt a snapshot of the main DB and
create a new encrypted DB instance
from the encrypted snapshot. Create a
encrypted cross-Region read replica
Amazon Aurora DB deployed and
requires a cross-Region replica
Deploy an Aurora MySQL Replica in the
second Region
Amazon Aurora DB deployed and
requires a read replica in the same
Region with minimal synchronization
latency
Deploy an Aurora Replica in the Region
in a different Availability Zone
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns – Databases & Analytics
Aurora deployed and app in another
Region requires read-only access with
low latency – synchronization latency
must also be minimized
Use Aurora Global Database and
configure the app in the second Region
to use the reader endpoint
Application and DB migrated to Aurora
and requires the ability to write to the
DB across multiple nodes
Use Aurora Multi-Master for an in-
Region multi-master database
Application requires a session-state
data store that provides low-latency
Use either Amazon ElastiCache or
DynamoDB
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns – Databases & Analytics
Multi-threaded in-memory datastore
required for unstructured data
Use Amazon ElastiCache Memcached
In-memory datastore required that
offers microsecond performance for
unstructured data
Use Amazon DynamoDB DAX (DAX)
In-memory datastore required that
supports data persistence and high
availability
Use Amazon ElastiCache Redis
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns – Databases & Analytics
Serverless database required that
supports No-SQL key-value store
workload
Use Amazon DynamoDB
Serverless database required that
supports MySQL or PostgreSQL
## Use Amazon Aurora Serverless
Relational database required for a
workload with an unknown usage
pattern (usage expected to be low and
variable)
## Use Amazon Aurora Serverless
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns – Databases & Analytics
Application requires a key-value
database that can be written to from
multiple AWS Regions
Use DynamoDB Global Tables
RequirementSolution
Athena is being used to analyze a large
volume of data based on date ranges.
Performance must be optimized
Store data using Apache Hive
partitioning with a key based on the
data. Use the Apache Parquet and ORC
storage formats
Lambda is processing streaming data
from API Gateway and is generating a
TooManyRequestsException as volume
increases
Stream the data into a Kinesis Data
Stream from API Gateway and process
in batches

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns – Databases & Analytics
Lambda function is processsing
streaming data that must be analyzed
with SQL
Load data into a Kinesis Data Stream
and then analyze with Kinesis Data
## Analytics
RequirementSolution
Security logs generated by AWS WAF
must be sent to a third-party auditing
application
Send logs to Kinesis Data Firehose and
configure the auditing application using
an HTTP endpoint
Real-time streaming data must be
stored for future analysis
Ingest data into a Kinesis Data Stream
and then use Firehose to load to a data
store for later analysis

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns – Databases & Analytics
Company runs several production
databases and must run complex
queries across consolidated data set
for business forecasting
Load the data from the OLTP databases
into a RedShift data warehouse for
## OLAP
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## SECTION 13
Deployment and Management

© Digital Cloud Training | https://digitalcloud.training
Infrastructure as Code with
AWS CloudFormation

© Digital Cloud Training | https://digitalcloud.training
AWS CloudFormation
## VPC
Public subnet
Public subnet
AWS CloudFormation
## Auto Scaling
group
Infrastructure patterns are
defined in a template file
using code
CloudFormation builds
your infrastructure
according to the template

© Digital Cloud Training | https://digitalcloud.training
AWS CloudFormation
ComponentDescription
## Templates
The JSON or YAML text file that contains the instructions for building out
the AWS environment
## Stacks
The entire environment described by the template and created, updated,
and deleted as a single unit
StackSets
AWS CloudFormation StackSets extends the functionality of stacks by
enabling you to create, update, or delete stacks across multiple accounts
and regions with a single operation
## Change Sets
A summary of proposed changes to your stack that will allow you to see
how those changes might impact your existing resources before
implementing them

© Digital Cloud Training | https://digitalcloud.training
Creating and Updating
## Stacks

© Digital Cloud Training | https://digitalcloud.training
Create Nested Stack using the
## AWS CLI

© Digital Cloud Training | https://digitalcloud.training
CloudFormation Nested Stacks
VPCSubnet 1Subnet 2
TheAWS::CloudFormation::Stackresource nests a stack as a resource
in a top-level template
## Nested
## Stack

© Digital Cloud Training | https://digitalcloud.training
Platform as a Service with
AWS Elastic Beanstalk

© Digital Cloud Training | https://digitalcloud.training
## Cloud Service Models: Comparison
Linux OS
## Java Runtime
## Data
Java WebApp
## Data
Java WebApp
IaaS
PaaS
You manage from the
virtual server upwards
You simply upload your
code/data to create your
application
Example is
Amazon EC2
Example is AWS
## Elastic Beanstalk

© Digital Cloud Training | https://digitalcloud.training
AWS Elastic Beanstalk
## Region
## VPC
## Availability Zone
Public subnet
## Availability Zone
Public subnet
## ALB
EB Environment
AWS Elastic Beanstalk
## Developer
## Client
Everything within the
environment is launched and
managed by Elastic Beanstalk
Upload source
code in ZIP file

© Digital Cloud Training | https://digitalcloud.training
AWS Elastic Beanstalk
•Supports many application platforms including:
- Java, .NET, Node.js, PHP, Ruby, Python, Go, and Docker
•Uses core AWS services including EC2, ECS, Auto
Scaling, and Elastic Load Balancing
•Elastic Beanstalk provides a UI to monitor and
manage the health of applications
•Managed platform updates deploy the latest
versions of software and patches

© Digital Cloud Training | https://digitalcloud.training
AWS Elastic Beanstalk
There are several layers
## Applications:
•Contain environments, environment
configurations, and application
versions
•You can have multiple application
versions held within an application
## APPLICATION

© Digital Cloud Training | https://digitalcloud.training
AWS Elastic Beanstalk
Application version
•A specific reference to a section of
deployable code
•The application version will point
typically to an Amazon S3 bucket
containing the code
## APPLICATION
## Version 1
## Version 2
## Version 3
## Version 4
## S3 Bucket
Versions can be
applied to any
environment

© Digital Cloud Training | https://digitalcloud.training
AWS Elastic Beanstalk
## Environments:
•An application version that has been
deployed on AWS resources
•The resources are configured and
provisioned by AWS Elastic Beanstalk
•The environment is comprised of all
the resources created by Elastic
Beanstalk and not just an EC2 instance
with your uploaded code
## DEVELOPMENT
## PRODUCTION
## APPLICATION
## Version 1
## Version 2
## Version 3
## Version 4
## S3 Bucket
Versions can be
applied to any
environment

© Digital Cloud Training | https://digitalcloud.training
Web Servers and Workers
•Web servers are standard applications that listen for
and then process HTTP requests, typically over port 80
•Workers are specialized applications that have a
background processing task that listens for messages
on an Amazon SQS queue
•Workers should be used for long-running tasks

© Digital Cloud Training | https://digitalcloud.training
AWS Elastic Beanstalk
## Web Server
Elastic Beanstalk application
## App User
## Worker
SQS Queue
## Web Server Environment
## Worker Environment
Web server places message in
the SQS queue
The worker polls the queue
Inbound traffic on
port 80/443

© Digital Cloud Training | https://digitalcloud.training
Create an Elastic
## Beanstalk Application

© Digital Cloud Training | https://digitalcloud.training
AWS Systems Manager
## Parameter Store

© Digital Cloud Training | https://digitalcloud.training
AWS SSM Parameter Store
•Parameter Store provides secure, hierarchical storage
for configuration data and secrets
•Highly scalable, available, and durable
•Store data such as passwords, database strings, and
license codes as parameter values
•Store values as plaintext (unencrypted data) or
ciphertext (encrypted data)
•Reference values by using the unique name that you
specified when you created the parameter
•No native rotation of keys (difference with AWS Secrets
Manager which does it automatically)
Amazon EC2
Amazon RDS
## Parameter
## Store
Retrieve database
connection string

© Digital Cloud Training | https://digitalcloud.training
AWS Config

© Digital Cloud Training | https://digitalcloud.training
AWS Config
•Evaluate your AWS resource configurations for desired settings
•Get a snapshot of the current configurations of resources that are
associated with your AWS account
•Retrieve configurations of resources that exist in your account
•Retrieve historical configurations of one or more resources
•Receive a notification whenever a resource is created, modified,
or deleted
•View relationships between resources

© Digital Cloud Training | https://digitalcloud.training
AWS Config
AWS Config
## Amazon S3
Amazon EC2
## Elastic Load Balancing
Amazon RDS
## Example Services:
## Amazon Simple
## Notification Service
CloudWatch Events
## Systems Manager
## Automation
AWS Config evaluates the configuration
against desired configurations
Configuration changes occur and
information is sent to AWS Config
## Automatic
remediation
Alert via CW Events
when changes occur
Send notifications
with SNS

© Digital Cloud Training | https://digitalcloud.training
AWS Config
Example RuleDescription
rds-instance-public-access-checkChecks whether the Amazon Relational Database Service
(RDS) instances are not publicly accessible
restricted-sshChecks whether security groups that are in use disallow
unrestricted incoming SSH traffic
cloudtrail-enabledChecks whether AWS CloudTrail is enabled in your AWS
account
s3-bucket-versioning-enabledChecks whether versioning is enabled for your S3 buckets
approved-amis-by-idChecks whether running instances are using specified AMIs

© Digital Cloud Training | https://digitalcloud.training
SSM Automation and Config
## Rules

© Digital Cloud Training | https://digitalcloud.training
AWS Secrets Manager

© Digital Cloud Training | https://digitalcloud.training
AWS Secrets Manager
•Stores and rotate secrets safely without the need
for code deployments
•Secrets Manager offers automatic rotation of
credentials (built-in) for:
•Amazon RDS (MySQL, PostgreSQL, and
## Amazon Aurora)
•Amazon Redshift
•Amazon DocumentDB
•For other services you can write your own AWS
Lambda function for automatic rotation
AWS Secrets Manager
Amazon RDS
AWS Lambda
Secrets automatically
rotated periodically

© Digital Cloud Training | https://digitalcloud.training
AWS Secrets Manager vs SSM Parameter Store
Secrets ManagerSSM Parameter Store
Automatic Key RotationYes, built-in for some services, use
Lambda for others
No native key rotation; can use custom
## Lambda
Key/Value TypeString or Binary (encrypted)String, StringList,  SecureString (encrypted)
Hierarchical KeysNoYe s
PriceCharges apply per secretFree for standard, charges for advanced

© Digital Cloud Training | https://digitalcloud.training
AWS Resource Access
Manager (RAM)

© Digital Cloud Training | https://digitalcloud.training
## AWS RAM
•Shares resources:
•Across AWS accounts
•Within AWS Organizations or OUs
•IAM roles and IAM users
•Resource shares are created with:
•The AWS RAM Console
•AWS RAM APIs
## •AWS CLI
•AWS SDKs

© Digital Cloud Training | https://digitalcloud.training
## AWS RAM
RAM can be used to share:
•AWS App Mesh
•Amazon Aurora
•AWS Certificate Manager Private Certificate Authority
•AWS CodeBuild
•Amazon EC2
•EC2 Image Builder
•AWS Glue
•AWS License Manager
•AWS Network Firewall
•AWS Outposts
•Amazon S3 on Outposts
•AWS Resource Groups
•Amazon Route 53
•AWS Systems Manager Incident Manager
•Amazon VPC

© Digital Cloud Training | https://digitalcloud.training
RPO, RTO, and DR Strategies

© Digital Cloud Training | https://digitalcloud.training
RPO and RTO
Recovery Point Objective (RPO)
•Measurement of the amount of data that can be acceptably
lost
•Measured in seconds, minutes, or hours
•Example:
•You can acceptably lose 2 hours of data in a database (2hr RPO)
•This means backups must be taken every 2 hours

© Digital Cloud Training | https://digitalcloud.training
RPO and RTO
Recovery Time Objective (RTO)
•Measurement of the amount of time it takes to restore after
a disaster event
•Measured in seconds, minutes, or hours
•Example:
•The IT department expect it to take 4 hours to bring applications
online after a disaster
•This would be an RTO of 4 hours

© Digital Cloud Training | https://digitalcloud.training
RPO and RTO
How much data is lost?How long to recover?
## RPO
## RTO
## Disaster Occurs

© Digital Cloud Training | https://digitalcloud.training
Achievable RPOs
Recovery Point ObjectiveTechnique
Milliseconds - SecondsSynchronous replication
Seconds - MinutesAsynchronous replication
Minutes to hoursSnapshots, cloud backup, D2D
Hours to daysOffsite / traditional backups / tape backups
The RPO is determined by how you take a backup of data

© Digital Cloud Training | https://digitalcloud.training
Achievable RTOs
Recovery Time ObjectiveTechnique
Milliseconds / SecondsFault tolerance
Seconds - MinutesHigh availability, load balancing, auto scaling
Minutes to hoursCross-site recovery (cloud), automated recovery
Hours to daysCross-site recovery (cloud/on-premises), manual
recovery
The RTO is determined by how quickly you can recover

© Digital Cloud Training | https://digitalcloud.training
DR Strategies
Backup and Restore
•Low priority
workloads
•Provision/restore
after event
•Cost $
## Pilot Light
•Data replicated
•Services idle/off
•Resources
activated after
event
•Cost $$
Warm standby
•Minimum
resources always
running
•Business critical
workloads
•Scale up/out after
event
•Cost $$$
## Multi-site
active/active
•Zero downtime
•Near zero data loss
•Mission critical
workloads
•Cost $$$$

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns –
Deployment and Management

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – Deployment and Management
Application must authenticate to
Amazon Aurora and need to securely
store credentials. Automatic credential
rotation is required on a monthly basis
Use AWS Secrets Manager to store the
credentials. Update the app to retrieve
credentials from Secrets Manager;
enable automatic monthly rotation
RequirementSolution
Company currently uses Chef
cookbooks to manage infrastructure
and is moving to the cloud. Need to
minimize migration complexity
Use AWS OpsWorks for Chef Automate
Need a managed environment for
running a simple web application. App
processes incoming data which can
take several minutes per task
Use an Elastic Beanstalk environment
with a web server for the app front-end
and a decoupled worker tier for the
long running process

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – Deployment and Management
Systems integrator deploys
standardized Amazon VPC configuration
for many customers. Need to increase
efficiency and reduce errors
Create an AWS CloudFormation
template based on the standard config
and use CloudFormation to deploy to
new customers
RequirementSolution
Company has experienced issues rolling
out updates to a CloudFormation Stack
and needs to preview changes before
the next update
Preview the change by creating a
change set with the updated template
before updating the stack
Manager wishes to monitor and enforce
configuration compliance for AWS
resources including S3 buckets and
security groups
Use AWS Config to create rules to
monitor compliance and use auto
remediation to enforce compliance

© Digital Cloud Training | https://digitalcloud.training
## SECTION 14
Monitoring, Logging, and Auditing

© Digital Cloud Training | https://digitalcloud.training
Amazon CloudWatch
## Overview

© Digital Cloud Training | https://digitalcloud.training
Amazon CloudWatch
CloudWatch is used for performance monitoring,
alarms, log collection and automated actions
Use cases / benefits include:
•Collect performance metrics from AWS and on-
premises systems
•Automate responses to operational changes
•Improve operational performance and resource
optimization
•Derive actionable insights from logs
•Get operational visibility and insight

© Digital Cloud Training | https://digitalcloud.training
Amazon CloudWatch
CloudWatch Core Features:
•CloudWatch Metrics – services send time-ordered data
points to CloudWatch
•CloudWatch Alarms –   monitor metrics and initiate actions
•CloudWatch Logs –   centralized collection of system and
application logs
•CloudWatch Events –   stream of system events describing
changes to AWS resources and can trigger actions

© Digital Cloud Training | https://digitalcloud.training
Amazon CloudWatch Metrics
•Metrics are sent to CloudWatch for many AWS services
•EC2 metrics are sent every 5 minutes by default (free)
•Detailed EC2 monitoring sends every 1 minute (chargeable)
•Unified CloudWatch Agent sends system-level metrics for EC2
and on-premises servers
•System-level metrics include memory and disk usage
Amazon CloudWatchAmazon EC2
CPUUtilization, DiskReadOps,
NetworkIn, StatusCheckFailed
## Memory, Disk Usage
CloudWatch Agent sends
system-level metrics
Standard every 5 minutes;
detailed every 1 minute

© Digital Cloud Training | https://digitalcloud.training
Amazon CloudWatch Metrics
•Can publish custom metrics using CLI or API
•Custom metrics are one of the following resolutions:
•Standard resolution – data having a one-minute granularity
•High resolution – data at a granularity of one second
•AWS metrics are standard resolution by default
Amazon CloudWatchAmazon EC2
CPUUtilization, DiskReadOps,
NetworkIn, StatusCheckFailed
## Memory, Disk Usage
CloudWatch Agent sends
system-level metrics
Standard every 5 minutes;
detailed every 1 minute

© Digital Cloud Training | https://digitalcloud.training
Amazon CloudWatch Alarms
Two types of alarms
•Metric alarm – performs one or more actions based on a single metric
•Composite alarm – uses a rule expression and takes into account multiple alarms
•You can create a custom metric using the API or CLI command set-alarm-state
•Metric alarm states:
•OK – Metric is within a threshold
•ALARM – Metric is outside a threshold
•INSUFFICIENT_DATA – not enough data
Amazon CloudWatch
CPU Utilization
EC2 Auto Scaling
## Metrics:
## ALARM
Amazon EC2
ec2:RunInstances

© Digital Cloud Training | https://digitalcloud.training
Create a Custom Metric
and Alarm

© Digital Cloud Training | https://digitalcloud.training
Amazon CloudWatch Logs

© Digital Cloud Training | https://digitalcloud.training
Amazon CloudWatch Logs
•Gather application and system logs in CloudWatch
•Defined expiration policies and KMS encryption
•Send to:
•Amazon S3 (export)
•Kinesis Data Streams
•Kinesis Data Firehose
Amazon CloudWatch
Amazon EC2
Application logs
System logs
AWS Lambda
## On-premises
servers
Application logs
System logs
Unified CloudWatch Agent
installed on EC2 and on-
premises servers
Function requires
permissions to
CloudWatch Logs
AWS Lambda
Real-time log
processing with
subscription filters
## Amazon Elasticsearch
## Service

© Digital Cloud Training | https://digitalcloud.training
The Unified CloudWatch
## Agent

© Digital Cloud Training | https://digitalcloud.training
The Unified CloudWatch Agent
The unified CloudWatch agent enables you to do
the following:
•Collect internal system-level metrics from
Amazon EC2 instances across operating systems
•Collect system-level metrics from on-premises
servers
•Retrieve custom metrics from your applications
or services using the StatsD and collectd
protocols
•Collect logs from Amazon EC2 instances and on-
premises servers (Windows / Linux)

© Digital Cloud Training | https://digitalcloud.training
The Unified CloudWatch Agent
•Agent must be installed on the server
•Can be installed on:
•Amazon EC2 instances
•On-premises servers
•Linux, Windows Server, or macOS
•You can use the following installation methods:
•Command line
•AWS Systems Manager
•AWS CloudFormation
•List of metrics collected:
https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/metrics-
collected-by-CloudWatch-agent.html

© Digital Cloud Training | https://digitalcloud.training
The Unified CloudWatch Agent
## Installation Process:
1.Create IAM roles to enable metric collection
2.Download the agent package
3.Update CloudWatch agent configuration file
4.Start the agent
•When starting the agent, you must attach the IAM
role (EC2), or specify a named profile (on-premises)
•You can optionally integrate with AWS Systems
## Manager

© Digital Cloud Training | https://digitalcloud.training
AWS CloudTrail Deep Dive

© Digital Cloud Training | https://digitalcloud.training
AWS CloudTrail
•CloudTrail records API calls made in your AWS account by
users, services, and applications
•It logs details such as who made the request, what action
was taken, which resources were touched, and when it
happened
•You can send logs to S3, CloudWatch Logs, or EventBridge for
monitoring and alerting
•It helps with security audits, troubleshooting, compliance,
and tracking changes across your AWS environment

© Digital Cloud Training | https://digitalcloud.training
AWS CloudTrail
API auditing with CloudTrail records information including:
•Which user or service...
•Made a request for an action (API call)...
•On which resource...
•At what date/time

© Digital Cloud Training | https://digitalcloud.training
AWS CloudTrail – Example Event

© Digital Cloud Training | https://digitalcloud.training
AWS CloudTrail Trails
•By default, management events are logged and retained for 90
days
•A CloudTrail Trail logs any events to S3 or CloudWatch Logs for
indefinite retention
•A Trail can be within a Region or across all Regions

© Digital Cloud Training | https://digitalcloud.training
AWS CloudTrail
•Amazon EventBridge can be triggered based on API calls in
CloudTrail
•When using CloudWatch Logs, subscription filters can be used
to trigger CloudWatch Alarms

© Digital Cloud Training | https://digitalcloud.training
AWS CloudTrail Deployment
AWS CloudTrail
## S3 Bucket
CloudWatch
## Logs
CloudWatch
## Alarm
SNS Topic
## Lambda
Create a Trail for
indefinite retention
Subscription filter used to
trigger CW Alarm
API event triggers Lambda
function or SNS topic
CloudTrail logs
API actions
## Amazon Athena
Query CloudTrail
logs using SQL
EventBridge
event bus
Can also store logs in
CloudWatch Logs

© Digital Cloud Training | https://digitalcloud.training
CloudTrail – Event Types
•Management events – Control-plane actions (create, update,
delete AWS resources)
•Data events – Data-plane actions inside resources
•Insights events – Detects unusual API activity, like spikes in
calls or abnormal error rates
•Network activity events –   API calls and service-calls that
traverse a VPC Endpoint

© Digital Cloud Training | https://digitalcloud.training
CloudTrail – Event Types
Management events:
•These record control-plane actions, meaning operations that
change the configuration of AWS resources
•Examples: creating a VPC, updating a security group, deleting
an S3 bucket, starting or stopping an EC2 instance
•They are enabled by default in CloudTrail because they track
important account-level changes

© Digital Cloud Training | https://digitalcloud.training
CloudTrail – Event Types
Example management event

© Digital Cloud Training | https://digitalcloud.training
CloudTrail – Event Types
Data events:
•These record data-plane actions, meaning activity inside a
resource
•Examples:
•S3 object-level actions (GetObject, PutObject)
•Lambda function invocations
•DynamoDB item-level operations
•They are not enabled by default because they generate a
large amount of logs

© Digital Cloud Training | https://digitalcloud.training
CloudTrail – Event Types
Example data event

© Digital Cloud Training | https://digitalcloud.training
CloudTrail – Event Types
Insights events:
•Detect unusual or unexpected API activity in your AWS
account
•Show spikes, drops, or abnormal patterns compared to your
normal baseline
•Help identify issues such as misconfigurations, automation
loops, or potential security problems
•Provide a summary record plus a detailed “Insight event”
showing what changed and when

© Digital Cloud Training | https://digitalcloud.training
CloudTrail – Event Types
Example insights event

© Digital Cloud Training | https://digitalcloud.training
CloudTrail – Event Types
Network activity events:
•Capture requests made through VPC endpoints or supported
network paths
•Log which account or service made the network call, the
target service, and whether it was allowed or denied
•Help verify access patterns for private connectivity setups like
PrivateLink
•Useful for debugging endpoint policies, blocked requests, and
unexpected network usage

© Digital Cloud Training | https://digitalcloud.training
CloudTrail – Event Types
Example network activity event

© Digital Cloud Training | https://digitalcloud.training
CloudTrail Lake and Event Data Stores
CloudTrail Lake:
•A feature that lets you ingest, store, and query CloudTrail
events using SQL
•It gives you long-term, centralized storage for audit and
security data
•You can run SQL queries directly inside CloudTrail without
exporting logs
•It supports CloudTrail events plus outside sources (security
tools, apps, other audit logs)

© Digital Cloud Training | https://digitalcloud.training
CloudTrail Lake and Event Data Stores
## Event Data Stores:
•These are the storage containers inside CloudTrail Lake where
your event data is kept
•Each store has its own retention period, access rules, and
data sources
•You can create multiple stores for different teams or
compliance needs
•Used for long-term audit history, investigations, and advanced
analytics

© Digital Cloud Training | https://digitalcloud.training
CloudTrail Lake Dashboards
•Lake dashboards show charts and summaries of your
CloudTrail Lake data
•They highlight trends like API usage, errors, and unusual
activity
•Powered by SQL queries that update automatically
•Used for quick audit and security insights

© Digital Cloud Training | https://digitalcloud.training
CloudTrail Channels
•Channels let you bring external audit logs into CloudTrail Lake
•They define how outside systems send events to AWS
•Imported events follow the CloudTrail format and can be
queried
•Used to centralize AWS and non-AWS activity logs in one
place

© Digital Cloud Training | https://digitalcloud.training
CloudTrail – Multi Account and Region
## Region
## Region
## Account A
## Account B
## Account C
## S3 Bucket
AWS CloudTrail
AWS CloudTrail
## Region
Configure logging to
bucket in Account C
Bucket policy required for
cross-account permissions

© Digital Cloud Training | https://digitalcloud.training
## Organization Trails
AWS Organization
## Management
## Account
## Production
## Development
Enable an Organization Trail
in management account and
apply to members
Logs are centralized into
one S3 bucket
Settings can be enforced
so accounts cannot turn
logging off

© Digital Cloud Training | https://digitalcloud.training
Create a Trail in AWS
CloudTrail

© Digital Cloud Training | https://digitalcloud.training
Amazon EventBridge
(Refresher)

© Digital Cloud Training | https://digitalcloud.training
Amazon CloudWatch Events / EventBridge
EventBridge used to be
known as CloudWatch
## Events
AWS Services
## Custom Apps
SaaS Apps
## Event Sources
## Events
EventBridge
event bus
## Rules
Ta rge t s

© Digital Cloud Training | https://digitalcloud.training
Create EventBridge rule for
CloudTrail API calls

© Digital Cloud Training | https://digitalcloud.training
Metric Analysis and Tracing
(Grafana, Prometheus, X-Ray)

© Digital Cloud Training | https://digitalcloud.training
Tracing with AWS X-Ray
•You can use AWS X-Ray to visualize the components of your
application, identify performance bottlenecks, and troubleshoot
requests that resulted in an error
•AWS services send trace data to X-Ray, and X-Ray processes the
data to generate a service map and searchable trace summaries

© Digital Cloud Training | https://digitalcloud.training
Tracing with AWS X-Ray
•X-Ray can be used with applications running on EC2, ECS,
Lambda, and Elastic Beanstalk
•You must integrate the X-Ray SDK with your application and
install the X-Ray agent
•The AWS X-Ray agent is a software application that gathers
raw segment data and relays it to the AWS X-Ray service
•The agent works in conjunction with the AWS X-Ray SDKs so
that data sent by the SDKs can reach the X-Ray service
•The X-Ray SDK captures metadata for requests made to
MySQL and PostgreSQL databases and Amazon DynamoDB
•It also captures metadata for requests made to Amazon SQS
and Amazon SNS

© Digital Cloud Training | https://digitalcloud.training
Amazon Managed Service for Prometheus
•Prometheus is an open-source monitoring system and time series
database
•Use the open-source Prometheus query language (PromQL) to
monitor and alert on the performance of containerized workloads
•Automatically scales the ingestion, storage, alerting, and querying
of operational metrics as workloads grow or shrink
•Integrated with Amazon EKS, Amazon ECS, and AWS Distro for
OpenTelemetry

© Digital Cloud Training | https://digitalcloud.training
## Amazon Managed Grafana
•Grafana is an open-source analytics and
monitoring solution for databases
•Highly scalable, highly available, and fully
managed service Grafana
•Provides interactive data visualization for your
monitoring and operational data
•Visualize, analyze, and alarm on your metrics, logs,
and traces collected from multiple data sources
•Integrates with AWS SSO and SAML

© Digital Cloud Training | https://digitalcloud.training
## Amazon Managed Grafana
Example of
anAmazon
## Managed Grafana
dashboard
visualizing data
from AWS X-Ray as
a data source

© Digital Cloud Training | https://digitalcloud.training
## Amazon Managed Grafana
Example visualizing
an imported MySQL
dashboard

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns -
Monitoring, Logging and Auditing

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – Monitoring, Logging and Auditing
Need to stream logs from Amazon EC2
instances in an Auto Scaling Group
Install the unified CloudWatch Agent
and collect log files in Amazon
CloudWatch
Need to collect metrics from EC2
instances with a 1 second granularity
Create a custom metric with high
resolution
The application logs from on-premises
servers must be processed by AWS
Lambda in real time
Install the unified CloudWatch Agent on
the servers and use a subscription filter
in CloudWatch to connect to a Lambda
function
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – Monitoring, Logging and Auditing
CloudWatch Logs entries must be
transformed with Lambda and then
loaded into Amazon S3
Configure a Kinesis Firehose
destination, transform with Lambda
and then load into an S3 bucket
Access auditing must be enabled, and
records must be stored for a minimum
of 5 years. Any attempts to modify the
log files must be identified
Create a trail in CloudTrail that stores
the data in an S3 bucket and enable log
file integrity validation
RequirementSolution
API activity must be captured from all
accounts in an Organization. Admins in
member accounts must not be able to
modify or delete the trail
Create an Organization trail in AWS
CloudTrail that applies to the
management account and all member
accounts

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – Monitoring, Logging and Auditing
RequirementSolution
Company requires API events that
involve the root user account to
generate a notification
Create a CloudTrail trail and an
EventBridge rule that looks for API
events that involve root and configure
an SNS notification
For compliance reasons all S3 buckets
must have encryption enabled and any
non-compliant buckets must be auto
remediated
Use AWS Config to check the
encryption status of the buckets and
use auto remediation to enable
encryption as required

© Digital Cloud Training | https://digitalcloud.training
## SECTION 15
Security in the Cloud

© Digital Cloud Training | https://digitalcloud.training
AWS Directory Services

© Digital Cloud Training | https://digitalcloud.training
AWS Directory Services
Types of Directory Services:
•AWS Managed Microsoft AD – Full AD in AWS, supports Group Policy
and trust relationships
•AD Connector – Proxy to on-prem AD, no replication
•Simple AD – Lightweight, Samba-based, limited features, lower cost

© Digital Cloud Training | https://digitalcloud.training
AWS Managed Microsoft AD
Corporate Office / DC
## VPC
Azure AD
Microsoft AD
ADSync
## ADFS
ConsoleWorkspaces
RDSWorkdocs
QuickSightWorkmail
## VPN
Also Allows you to:
•Apply group policy
•Use single sign-on to
apps and services
•Enable MFA with
## RADIUS
Managed implementation of Microsoft Active
Directory running on Windows Server
HA pair of Windows Server
Domain Controllers (DCs)
Many apps and services
support authentication and
authorization using AWS
## Directory Services
Synchronize users and
federate identities with
Azure/O365
Securely connect to
Amazon EC2 Linux and
Windows instances
A one or two-way trust
relationship is established

© Digital Cloud Training | https://digitalcloud.training
AWS Managed Microsoft AD
## Key Features:
•Supports Group Policy, Kerberos, LDAP, and NTLM
authentication
•Trust relationships with on-prem AD (one-way or two-way)
•Multi-AZ replication for high availability
•Custom OU (Organizational Unit) support
## Use Cases:
•Extend on-prem Active Directory to AWS (hybrid cloud)
•Manage Windows-based workloads in AWS (EC2, FSx, RDS
for SQL Server)
•Centralized identity management for AWS services like
WorkSpaces

© Digital Cloud Training | https://digitalcloud.training
AD Connector
## AD
## Connector
## Active Directory
Amazon EC2
AWS Management
## Console
Amazon WorkSpaces
Corporate Office / DC
## VPN
Sign-in to AWS applicationssuch as Amazon
WorkSpaces, Amazon WorkDocs, and Amazon
WorkMail by using your Active Directory credentials
Connection over VPN or
## Direct Connect
## Self-managed
Micorosoft AD
AD Connector provides federated sign-in to
the AWS Management Console by mapping
Active Directory identities to IAM Roles
Seamlessly join Windows EC2
instances to an on-premise
AD domain
## Deployment Options:
•Small AD Connector: Up to 500
users
•Large AD Connector: More than
500 users

© Digital Cloud Training | https://digitalcloud.training
AD Connector
## Key Features:
•No directory data replication to AWS (queries forwarded to
on-prem AD)
•Supports Windows workloads, IAM authentication, AWS
IAM Identity Center
•Redundant, deployed across two subnets in a VPC
## Use Cases:
•Extend on-prem AD authentication to AWS without
syncing users
•Authenticate services for AWS WorkSpaces, FSx, RDS SQL,
and EC2
•Avoid AD replication for compliance/security reasons

© Digital Cloud Training | https://digitalcloud.training
Simple AD
What it is: A lightweight, Samba 4-based directory in
## AWS
## Key Features:
•Supports LDAP, Kerberos, and NTLM authentication.
•No trust relationships with on-prem AD
•Basic Group Policy support but lacks advanced AD features
## Use Cases:
•Small-scale applications that don’t require full Microsoft
## AD
•Standalone Linux/Unix authentication
•Basic AWS WorkSpaces or EC2 authentication

© Digital Cloud Training | https://digitalcloud.training
Simple AD
Deployment options:
•Small Directory: Up to 500 users
•Large Directory: Up to 5,000 users

© Digital Cloud Training | https://digitalcloud.training
AWS Directory Services
FeatureManaged AD AD ConnectorSimple AD
TypeFull AD in AWSProxy to on-prem ADLightweight AD
ReplicationYe sNoNo
Trusts with on-prem ADYe sUses existing on-prem ADNo
User authenticationAWS + on-prem usersOn-prem users onlyUsers within the directory
Group Policy supportYe sYes (via on-prem AD)Limited
AWS Services IntegrationYe sYe sLimited
Use CaseWindows workloads,
hybrid AD
Use on-prem AD for AWS
login
Small, standalone
environments

© Digital Cloud Training | https://digitalcloud.training
Identity Providers and
## Federation

© Digital Cloud Training | https://digitalcloud.training
IAM – SAML 2.0 Identity Federation
Corporate Office / DC
Users log in
App must access data in a DynamoDB table
## App
## ADFS
## Active Directory Federation Services
is an Identity Provider (IdP)
Active Directory is an
LDAP Identity Store
## AWS STS
DynamoDB Table
AWS Security Token Service (STS) returns
temporary security credentials
IdP authenticates
the user
IdP sends client
SAML assertion
App calls
sts:AssumeRoleWithSAML
App uses credentials to
access DynamoDB

© Digital Cloud Training | https://digitalcloud.training
IAM – Web Identity Federation
## Mobile App
Social identity providers (IdPs)
## AWS STS
DynamoDB Table
AWS Security Token Service (STS) returns
temporary security credentials
App uses credentials to
access DynamoDB
AWS recommend to use Cognito for web
identity federation in most cases
Any Open ID Connect (OIDC)
compatible IdP supported
App calls
sts:AssumeRoleWithWebIdentity

© Digital Cloud Training | https://digitalcloud.training
IAM Identity Center
IAM Identity Center is the successor to
AWS Single Sign-On (SSO)
IAM Identity Center
AWS Organizations
## AWS
## Account A
## AWS
## Account B
AWS Account C
AWS Account D
## Active Directory
## (self-managed)
Azure AD
Corporate Office / DC
Built-in SSO integrations to
business applications
Identity sources can be Identity Center
directory, Active Directory and
standard providers using SAML 2.0
Enables centralized permissions
management and SSO
AD Connector or AWS
Managed Microsoft AD

© Digital Cloud Training | https://digitalcloud.training
## Amazon Cognito
Amazon DynamoDB
## Mobile App
## Cognito User
## Pool
## Cognito Identity
## Pool
Social identity providers (IdPs)
Token returned
## (JWT)
## AWS STS
Token gets exchanged for
temporary security credentials
CIP calls
sts:AssumeRoleWithWebIdentity

© Digital Cloud Training | https://digitalcloud.training
IAM Identity Center in
## Action

© Digital Cloud Training | https://digitalcloud.training
## Amazon Cognito

© Digital Cloud Training | https://digitalcloud.training
## Cognito User Pools
## Cognito User Pool
## Client /
## Mobile App
A User Pool is a directory for
managing sign-in and sign-up
for mobile applications
Cognito acts as an
Identity Broker between
the IdP and AWS
## SAML
## OIDC
## Identity
## Providers
Users can also sign
in using social IdPs
The app sends an
authentication request
Token (JWT)
## Lambda Authorizer
Token (JWT)
## API
Authenticated requests are
passed to the application
A Lambda authorizer
accepts the JWT
## Application
API Gateway is used as
the app front-end

© Digital Cloud Training | https://digitalcloud.training
## Cognito User Pools
•Manages user authentication (sign-in/sign-up)
•Acts as an Identity Provider (IdP) or brokers authentication from
external IdPs
•Issues JWT tokens (ID token, access token, refresh token) for
authentication
•Used for securing applications (e.g., API Gateway, Lambda,
AppSync)
•Supports MFA, adaptive authentication, and custom
authentication flows
•Does NOT provide AWS credentials—only authentication

© Digital Cloud Training | https://digitalcloud.training
## Cognito Identity Pool
## Cognito Identity Pool
## SAML
## OIDC
## Identity
## Providers
AWS Lambda
## STS
IAM Role
Amazon DynamoDB
## Cognito User Pool
Identities can come from a
Cognito user pool
Identity pools use AWS STS to
obtain the credentials
Identities can come
from social IdPs
Identity pools are used to obtain
temporary, limited-privilege
credentials for AWS services
An IAM role is assumed providing
access to the AWS services

© Digital Cloud Training | https://digitalcloud.training
## Cognito Identity Pools
•Manages access to AWS services by providing temporary
IAM credentials
•Uses federated identities (User Pool users, external IdPs,
guest users)
•Issues temporary AWS IAM credentials via AWS Security
Token Service (STS)
•Allows access to AWS services like S3, DynamoDB, and
Lambda directly
•Works alongside User Pools but can also use social logins or
SAML directly

© Digital Cloud Training | https://digitalcloud.training
## User Pools + Identity Pools
## Cognito User
## Pool
## Region
## Cognito Identity
## Pool
Other AWS Services
Amazon DynamoDB
Token (JWT)
Authenticate and get
tokens
Exchange tokens for AWS credentials
Access AWS services
with credentials
AWS Lambda
## SAML
## OIDC
## Identity Providers
## 1
## 2
## 3
## Client /
## Mobile App
An IAM role is assumed
providing access to the
AWS services

© Digital Cloud Training | https://digitalcloud.training
User Pools vs Identity Pools
•User Pools → Authentication (Who the user is, JWT tokens)
•Identity Pools → Authorization (What the user can do, AWS
IAM credentials)

© Digital Cloud Training | https://digitalcloud.training
## Encryption Primer

© Digital Cloud Training | https://digitalcloud.training
Encryption In Transit vs At Rest
## User
## Unencrypted
## Object
## Encrypted
bucket
Encryption process
Data encryption key
## Encryption In Transit
## Encryption At Rest
HTTPS Connection
## ALB
Data is protected by
SSL/TLS in transit
Amazon S3 encrypts the
object as it is written to
the bucket it

© Digital Cloud Training | https://digitalcloud.training
## Asymmetric Encryption
•Asymmetric encryption is also known as public key cryptography
•Messages encrypted with the public key can only be decrypted with
the private key
•Messages encrypted with the private key can be decrypted with the
public key
•Examples include SSL/TLS and SSH
## Encrypted
data
Plaintext data
Public keyPrivate key
Plaintext data
## Encryption
## Decryption

© Digital Cloud Training | https://digitalcloud.training
## Symmetric Encryption
Data encryption key
## Encrypted
data
Encryption process
Plaintext data
## Encrypted
data
Encryption process
Plaintext data
Data encryption key
## Encryption
## Decryption
The same key is used
for both encryption
and decryption

© Digital Cloud Training | https://digitalcloud.training
AWS Key Management
Service (KMS)

© Digital Cloud Training | https://digitalcloud.training
AWS Key Management Service (KMS)
•Create and managed symmetric and asymmetric encryption keys
•The KMS keys are protected by hardware security modules (HSMs)
## Customer Managed Keys
KeyKeyKeyKey
## Developer
aws/acmaws/sqsaws/fsxaws/ebs
AWS Managed Keys
## AWS KMS
Developer creates customer
managed KMS keys in AWS KMS

© Digital Cloud Training | https://digitalcloud.training
KMS Keys
•KMS keys are the primary resources in AWS KMS
•Used to be known as “customer master keys” or CMKs
•The KMS key also contains the key material used to encrypt
and decrypt data
•By default, AWS KMS creates the key material for a KMS key
•You can also import your own key material
•A KMS key can encrypt data up to 4KB in size
•A KMS key can generate, encrypt and decrypt Data Encryption
Keys (DEKs)

© Digital Cloud Training | https://digitalcloud.training
## Alternative Key Stores
## External Key Store
•Keys can be stored outside of AWS to meet regulatory requirements
•You can create a KMS key in an AWS KMS external key store (XKS)
•All keys are generated and stored in an external key manager
•When using an XKS, key material never leaves your HSM
## Custom Key Store
•You can create KMS keys in an AWS CloudHSM custom key store
•All keys are generated and stored in an AWS CloudHSM cluster that you own and manage
•Cryptographic operations are performed solely in the AWS CloudHSM cluster you own
and manage
•Custom key stores are not available for asymmetric KMS keys

© Digital Cloud Training | https://digitalcloud.training
AWS Managed KMS Keys
•Created, managed, and used on your behalf
by an AWS service that is integrated with
## AWS KMS
•You cannot manage these KMS keys, rotate
them, or change their key policies
•You also cannot use AWS managed KMS keys
in cryptographic operations directly; the
service that creates them uses them on your
behalf

© Digital Cloud Training | https://digitalcloud.training
## Data Encryption Keys
•Data keys are encryption keys that you can use to encrypt
large amounts of data
•You can use AWS KMS keys to generate, encrypt, and
decrypt data keys
•AWS KMS does not store, manage, or track your data keys,
or perform cryptographic operations with data keys
•You must use and manage data keys outside of AWS KMS
## Key
## AWS KMS
## Encryption
## Algorithm
Plaintext data key
Encrypted data key

© Digital Cloud Training | https://digitalcloud.training
KMS Keys and Automatic Rotation
Type of KMS KeyCan viewCan manageUsed only for my AWS accountAutomatic rotation
Customer managed keyYe sYe sYe sOptional. Every 365 days
AWS managed keyYe sNoYe sRequired. Every 365 days
AWS owned keyNoNoNoVaries
•You cannot enable or disable key rotation for AWS owned keys
•Automatic key rotation is supported only on symmetric encryption KMS keys
with key material that AWS KMS generates (Origin = AWS_KMS)

© Digital Cloud Training | https://digitalcloud.training
KMS Keys and Automatic Rotation
•Automatic rotation generates new key material every year
(optional for customer managed keys)
Rotation only changes the
key material used for
encryption, the KMS key
remains the same

© Digital Cloud Training | https://digitalcloud.training
KMS Keys and Automatic Rotation
With automatic key rotation:
•The properties of the KMS key, including its key ID, key ARN, region, policies, and
permissions, do not change when the key is rotated
•You do not need to change applications or aliases that refer to the key ID or key ARN
of the KMS key
•After you enable key rotation, AWS KMS rotates the KMS key automatically every
year
Automatic key rotation is not supported on the following types of KMS keys:
•Asymmetric KMS keys
•HMAC KMS keys
•KMS keys in custom key stores
•KMS keys with imported key material
Note: You can rotate these
KMS keys manually

© Digital Cloud Training | https://digitalcloud.training
## Manual Rotation
•Manual rotation is creating a new KMS key with a different key ID
•You must then update your applications with the new key ID
•You can use an alias to represent a KMS key so you don’t need to modify your
application code
Old KeyNew Key
## Application
## Alias
The alias is associated
with the new KMS key

© Digital Cloud Training | https://digitalcloud.training
KMS Key Policies
•Key policies define management and usage permissions for KMS
keys
This key policy defines the
administrative actions that are
permitted for a key administrator

© Digital Cloud Training | https://digitalcloud.training
KMS Key Policies
•Multiple policy statements can be combined to specify separate
administrative and usage permissions
This key policy defines the cryptographic
actions for encrypting and decrypting data
with the KMS key

© Digital Cloud Training | https://digitalcloud.training
KMS Key Policies
•Permissions can be specified for delegating use of the key to AWS
services
Grants are useful for temporary permissions
as they can be used without modifying key
policies or IAM policies

© Digital Cloud Training | https://digitalcloud.training
## Additional Exam Tips
•To share snapshots with another account you must specify Decrypt
and CreateGrant permissions
•The kms:ViaService condition key can be used to limit key usage to
specific AWS services
•For example:

© Digital Cloud Training | https://digitalcloud.training
## Additional Exam Tips
•Cryptographic erasure means removing the ability to decrypt data
and can be achieved when using imported key material and
deleting that key material
•You must use the DeletelmportedKeyMaterial API to remove the key
material
•An InvalidKeyId exception when using SSM Parameter Store indicates
the KMS key is not enabled
•Make sure you know the differences between AWS managed and
customer managed KMS keys and automatic vs manual rotation

© Digital Cloud Training | https://digitalcloud.training
Encrypt and Decrypt Data
with AWS KMS

© Digital Cloud Training | https://digitalcloud.training
AWS CloudHSM

© Digital Cloud Training | https://digitalcloud.training
AWS CloudHSM
•AWS CloudHSM is a cloud-based hardware security module
## (HSM)
•Generate and use your own encryption keys on the AWS
## Cloud
•CloudHSM runs in your Amazon VPC
•Uses FIPS 140-2 level 3 validated HSMs
•Managed service and automatically scales
•Retain control of your encryption keys - you control access
(and AWS has no visibility of your encryption keys)

© Digital Cloud Training | https://digitalcloud.training
AWS CloudHSM Use Cases
•Offload SSL/TLS processing from web servers
•Protect private keys for an issuing certificate authority (CA)
•Store the master key for Oracle DB Transparent Data Encryption
•Custom key store for AWS KMS – retain control of the HSM that
protects the master keys

© Digital Cloud Training | https://digitalcloud.training
AWS CloudHSM vs KMS
CloudHSMAWS KMS
TenancySingle-tenant HSMMulti-tenant AWS service
AvailabilityCustomer-managed durability and
available
Highly available and durable key storage
and management
Root of TrustCustomer managed root of trustAWS managed root of trust
FIPS 140-2Level 3Level 2 / Level 3
## 3
rd
Party SupportBroad 3
rd
Party SupportBroad AWS service support

© Digital Cloud Training | https://digitalcloud.training
AWS Certificate Manager
## (ACM)

© Digital Cloud Training | https://digitalcloud.training
AWS Certificate Manager (ACM)
•Create, store and renew SSL/TLS X.509 certificates
•Single domains, multiple domain names and
wildcards
•Integrates with several AWS services including:
•Elastic Load Balancing
•Amazon CloudFront
•AWS Elastic Beanstalk
•AWS Nitro Enclaves
•AWS CloudFormation

© Digital Cloud Training | https://digitalcloud.training
AWS Certificate Manager (ACM)
•Public certificates are signed by the AWS public
## Certificate Authority
•You can also create a Private CA with ACM
•Can then issue private certificates
•You can also import certificates from third-party
issuers

© Digital Cloud Training | https://digitalcloud.training
SSL/TLS Certificate in ACM

© Digital Cloud Training | https://digitalcloud.training
AWS Web Application
Firewall (WAF)

© Digital Cloud Training | https://digitalcloud.training
## AWS WAF
•AWS WAF is a web application firewall
•WAF lets you create rules to filter web traffic based on
conditions that include IP addresses, HTTP headers and
body, or custom URIs
•WAF makes it easy to create rules that block common
web exploits like SQL injection and cross site scripting

© Digital Cloud Training | https://digitalcloud.training
## AWS WAF
## AWS WAF
Amazon CloudFront
## ALB
Amazon API Gateway
## AWS WAF
## AWS WAF
Amazon EC2
AWS AppSync
## AWS WAF

© Digital Cloud Training | https://digitalcloud.training
## AWS WAF
•Web ACLs – You use a web access control list (ACL) to protect a set
of AWS resources
•Rules – Each rule contains a statement that defines the inspection
criteria, and an action to take if a web request meets the criteria
•Rule groups – You can use rules individually or in reusable rule
groups

© Digital Cloud Training | https://digitalcloud.training
## AWS WAF
•IP Sets - An IP set provides a collection of IP addresses and IP
address ranges that you want to use together in a rule statement
•Regex pattern set - A regex pattern set provides a collection of
regular expressions that you want to use together in a rule
statement

© Digital Cloud Training | https://digitalcloud.training
## AWS WAF
A rule action tells AWS WAF what to do with a web request when it
matches the criteria defined in the rule:
•Count – AWS WAF counts the request but doesn't determine
whether to allow it or block it. With this action, AWS WAF
continues processing the remaining rules in the web ACL
•Allow – AWS WAF allows the request to be forwarded to the AWS
resource for processing and response
•Block – AWS WAF blocks the request and the AWS resource
responds with an HTTP 403 (Forbidden) status code

© Digital Cloud Training | https://digitalcloud.training
## AWS WAF
Match statements compare the web request or its origin against
conditions that you provide
Match StatementDescription
Geographic matchInspects the request's country of origin
IP set matchInspects the request against a set of IP addresses and address ranges
Regex pattern setCompares regex patterns against a specified request component
Size constraintChecks size constraints against a specified request component
SQLi attackInspects for malicious SQL code in a specified request component
String matchCompares a string to a specified request component
XSS scripting attackInspects for cross-site scripting attacks in a specified request component

© Digital Cloud Training | https://digitalcloud.training
AWS Shield

© Digital Cloud Training | https://digitalcloud.training
AWS Shield
•AWS Shield is a managed Distributed Denial of Service
(DDoS) protection service
•Safeguards web application running on AWS with always-on
detection and automatic inline mitigations
•Helps to minimize application downtime and latency
•Two tiers –
•Standard –   no cost
•Advanced - $3k USD per month and 1 year commitment
•Integrated with Amazon CloudFront (standard included by
default)

© Digital Cloud Training | https://digitalcloud.training
## Amazon Macie

© Digital Cloud Training | https://digitalcloud.training
## Amazon Macie
•Macie is a fully managed data security and data privacy service
•Uses machine learning and pattern matching to discover,
monitor, and help you protect your sensitive data on Amazon S3
•Macie enables security compliance and preventive security as
follows:
•Identify a variety of data types, including PII, Protected Health
Information (PHI), regulatory documents, API keys, and secret keys
•Identify changes to policy and access control lists
•Continuously monitor the security posture of Amazon S3
•Generate security findings that you can view using the Macie console,
AWS Security Hub, or Amazon EventBridge
•Manage multiple AWS accounts using AWS Organizations

© Digital Cloud Training | https://digitalcloud.training
## Amazon Macie
Amazon S3Amazon Macie
CloudWatch Events
## Automatically
discovers S3 buckets
Analyzes buckets using
ML to discover sensitive
information
Sends findings to
CloudWatch Events

© Digital Cloud Training | https://digitalcloud.training
## Amazon Inspector

© Digital Cloud Training | https://digitalcloud.training
## Amazon Inspector
•Runs assessments that check for security exposures and
vulnerabilities in EC2 instances
•Can be configured to run on a schedule
•Agent must be installed on EC2 for host assessments
•Network assessments do not require an agent

© Digital Cloud Training | https://digitalcloud.training
## Amazon Inspector
## Network Assessments
•Assessments: Network configuration analysis to check for
ports reachable from outside the VPC
•If the Inspector Agent is installed on your EC2 instances, the
assessment also finds processes reachable on port
•Price based on the number of instance assessments

© Digital Cloud Training | https://digitalcloud.training
## Amazon Inspector
## Host Assessments
•Assessments: Vulnerable software (CVE), host hardening (CIS
benchmarks), and security best practices
•Requires an agent (auto-install with SSM Run Command)
•Price based on the number of instance assessments

© Digital Cloud Training | https://digitalcloud.training
AWS GuardDuty

© Digital Cloud Training | https://digitalcloud.training
AWS GuardDuty
•Intelligent threat detection service
•Detects account compromise, instance compromise,
malicious reconnaissance, and bucket compromise
•Continuous monitoring for events across:
•AWS CloudTrail Management Events
•AWS CloudTrail S3 Data Events
•Amazon VPC Flow Logs
•DNS Logs

© Digital Cloud Training | https://digitalcloud.training
Defense in Depth

© Digital Cloud Training | https://digitalcloud.training
Defense in Depth
•Layered security uses multiple defenses to protect against
threats at various levels, like network, application, and data

© Digital Cloud Training | https://digitalcloud.training
Defense in Depth
•Redundant layers ensure backup protection if one layer is
compromised
•Minimizes risk by reducing single points of failure, making
unauthorized access more difficult
•Combines firewalls, encryption, access control, and
monitoring for stronger overall security

© Digital Cloud Training | https://digitalcloud.training
Defense in Depth
DB Subnet 1App Subnet 1
## Web Subnet 1
DB Subnet 2App Subnet 2
## Web Subnet 2

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns - Security

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns – Security
Need to enable custom domain name
and encryption in transit for an
application running behind an
## Application Load Balancer
Use AWS Route 53 to create an Alias
record to the ALB’s DNS name and
attach an SSL/TLS certificate issued by
Amazon Certificate Manager (ACM)
RequirementSolution
Website running on EC2 instances
behind and ALB must be protected
against well known web exploits
Create a Web ACL in AWS WAF to
protect against web exploits and attach
to the ALB
Need to block access to an application
running on an ALB from connections
originating in a specific list of countries
Create a Web ACL in AWS WAF with a
geographic match and block traffic that
matches the list of countries

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns – Security
RequirementSolution
Company needs to encrypt large
volumes of data using a CMK in AWS
## KMS
Create a data encryption key using the
CMK to encrypt large volumes of data
Mobile app requires authorized access
to AWS services. Users authenticate
using social IdPs and a preconfigured
Web UI is required for logging in
Create an Amazon Cognito User Pool
that leverages the social IdPs and an
Identity Pool for gaining temporary
credentials for AWS
Company has an on-premises
Microsoft AD and AWS DX connection.
Requires joining EC2 instances to on-
premises domain
Configure an AD Connector that uses
the on-premises AD

© Digital Cloud Training | https://digitalcloud.training
## SECTION 16
Migration and Transfer Services

© Digital Cloud Training | https://digitalcloud.training
AWS Migration Tools
## Overview

© Digital Cloud Training | https://digitalcloud.training
AWS Migration Tools
EC2 Instances
EFS File system
Corporate data center
## Servers
## Region
VPN, Direct
Connect or Internet
Amazon RDS
## Amazon S3
## Database
NAS / File
## Server
AWS Database Migration
## Service
AWS DataSync
AWS Migration Hub
AWS Application
## Discovery Service
AWS Application
## Migration Service
Monitor migrations that use
AWS or partner tools
Collect data
about servers in
on-premises DC

© Digital Cloud Training | https://digitalcloud.training
AWS Application Discovery Service
Data center
VMware
## Server
## Server
## Server
AWS Application
## Discovery Service
HostnamesIP Addresses  MACAddresses
## Disk Resource Allocations
VM Utilization
CPU, RAM, Disk I/O
Static config dataTime-series perf data
Network In/OutRunning Processes
Hyper-V
Agent-based discovery
(Windows / Linux)
Agentless discovery
(OVA) file in vCenter
Data can be saved to S3
and queried with
Athena / QuickSight
Collects server hostnames, IP addresses, MAC addresses,as
well as resource allocation and utilization details of key
resources including CPU, network, memory, and disk

© Digital Cloud Training | https://digitalcloud.training
AWS Application Discovery Service
Discovery ConnectorDiscovery Agent
Supported ServersVMwareVMware, Physical
DeploymentPer vCenterPer Server
Collected dataVM inventory, configuration, and
performance history such as CPU, memory,
and disk usage
System configuration
System performance
Running processes
Network connections between systems
Supported OSAny OS running in VMware vCenter (v5.5,
v6, & v6.5
Amazon Linux, Ubuntu, RHEL, CentOS,
SUSE, Windows Server

© Digital Cloud Training | https://digitalcloud.training
AWS Database Migration
Service (DMS)

© Digital Cloud Training | https://digitalcloud.training
AWS Database Migration Service (DMS)
Data center
Data center
## Oracle
database
MySQL
database
Can be on-premises,
on EC2, or RDS
AWS Database Migration
## Service
AWS Database Migration
## Service
Amazon RedShift
## Amazon Aurora
Use the Schema
Conversion Tool for
heterogeneous migrations
Destinations include Aurora,
RedShift DynamoDB, and
DocumentDB

© Digital Cloud Training | https://digitalcloud.training
AWS DMS Use Cases
•Cloud to Cloud – EC2 to RDS, RDS to RDS, RDS to Aurora
•On-Premises to Cloud
•Homogeneous migrations –   Oracle to Oracle, MySQL to RDS
MySQL,  Microsoft SQL to RDS for SQL Server
•Heterogeneous migrations –   Oracle to Aurora, Oracle to
PostgreSQL, Microsoft SQL to RDS MySQL (must convert
schema first with the Shema Conversion Tool (SCT))

© Digital Cloud Training | https://digitalcloud.training
AWS DMS Use Cases
•Development and Test –   use the cloud for dev/test
workloads
•Database consolidation –   consolidate multiple source DBs to
a single target DB
•Continuous Data Replication –   use for DR, dev/test, single
source multi-target or multi-source single target

© Digital Cloud Training | https://digitalcloud.training
AWS Application
Migration Service (MGN)

© Digital Cloud Training | https://digitalcloud.training
AWS Application Migration Service (MGN)
EC2 Instances
Data center
VMware
Hyper-V
Agentless snapshot-based
replication possible with the AWS
MGN vCenter Client installed
AWS recommend agent-based
replication when possible as it support
continuous data protection (CDP)
Automated, incremental
and scheduled migrations
EC2 instances are launched
from launch templates
CloudWatch Events
and Lambda can
automate actions
## Launch Template
AWS Application
## Migration Service

© Digital Cloud Training | https://digitalcloud.training
AWS Application Migration Service (MGN)
Data center
## Database Servers
## App Servers
## Web Servers
EC2 Instances
CloudFormation
Te m p l a t e
CloudFormation
## Launch Template
AWS Application
## Migration Service
Entire application group
is launched in a
migration wave

© Digital Cloud Training | https://digitalcloud.training
AWS Application Migration Service (MGN)
•Highly automated lift-and-shift (rehost) solution for
migrating applications to AWS
•Utilizes continuous, block-level replication and enables
short cutover windows measured in minutes
•Server Migration Service (SMS) utilizes incremental,
snapshot-based replication and enables cutover windows
measured in hours
•AWS recommend using AWS MGN instead of SMS
•Integrates with the Cloud Migration Factory for
orchestrating manual processes
•Can migrate virtual and physical servers

© Digital Cloud Training | https://digitalcloud.training
AWS DataSync

© Digital Cloud Training | https://digitalcloud.training
AWS DataSync
Data center
## NFS, SMB, S3
## API, HDFS
## Shared File System
or Object Storage
AWS DataSync
Amazon FSx
## Amazon Simple
## Storage Service
## Amazon Elastic File
## System
AWS SnowCone
DataSync agent installed
on Snowcone
DataSync software agent
connects to storage system
Scheduled, automated
data transfer
Data is encrypted in
transit with TLS
Amazon S3 on
## Outposts

© Digital Cloud Training | https://digitalcloud.training
AWS DataSync
•Secure, online service that automates and accelerates
moving data between on premises and AWS Storage services
•DataSync can copy data between:
•Network File System (NFS) shares
•Server Message Block (SMB) shares
•Hadoop Distributed File Systems (HDFS)
•Self-managed object storage
•AWS Snowcone
•Amazon S3 buckets
•Amazon Elastic File System (Amazon EFS) file systems
•Amazon FSx (Windows, Lustre, OpenZFS, and NetApp ONTAP)

© Digital Cloud Training | https://digitalcloud.training
AWS Snow Family

© Digital Cloud Training | https://digitalcloud.training
AWS Snow Family
## Snowball Edge
•Compute Optimized (28 TB)
•Provides block and object storage and optional GPU
•Use for data collection, machine learning and processing, and
storage in environments with intermittent connectivity (edge use
cases)
•Storage Optimized (210 TB)
•Provides block storage and Amazon S3-compatible object storage
•Use for local storage and large-scale data transfer
•Use SCT to save data to device and load into AWS
•Snowcone (up to 14 TB)
•Small device used for edge computing, storage and data
transfer
•Can transfer data offline or online with AWS DataSync
agent

© Digital Cloud Training | https://digitalcloud.training
The 7 Rs of Migration

© Digital Cloud Training | https://digitalcloud.training
The 7 Rs of Migration
•Refactor –   Re-architect to a cloud-native serverless architecture
•Replatform –   Ex. database to RDS; server to Elastic Beanstalk
•Repurchase –   Use a different solution (e.g. SaaS)
•Rehost –   OS/App moved to another host system (lift & shift)
•Relocate –   Move without modification (lift & Shift)
•Retain –   Leave as is (revisit at a later date)
•Retire –   No longer needed, get rid of it
## Least Effort
## Most Effort

© Digital Cloud Training | https://digitalcloud.training
The 7 Rs of Migration
•Rehost –   OS/App moved to another host system
•AWS recommend the AWS Application Migration
Service (AWS MGN) for lift & shift
•Can also use AWS SMS and AWS VM Import / Export
EC2 Instances
Data center
VMware
Hyper-V
Te s t and cutover
instances launched
AWS Application
## Migration Service
AWS Replication Agent
installed on servers
Agentless replication
for vCenter

© Digital Cloud Training | https://digitalcloud.training
The 7 Rs of Migration
•Replatform –   Ex. database to RDS; server to Elastic Beanstalk
•AWS Database Migration Service (AWS DMS) and Schema
Conversion Tool (SCT)
•Migrate to EB using custom AMI, or code-level migration
•Moderate development and migration effort
Data center
MySQL DB
## AWS DMS
## Amazon Aurora

© Digital Cloud Training | https://digitalcloud.training
The 7 Rs of Migration
•Refactor –   Re-architect to a cloud-native serverless
architecture
•Leverage serverless services and event-driven architecture patterns
•Migrate servers to serverless functions or containers
•Migrate databases to managed DBs or serverless NoSQL DBs
•Migrate file stores to object stores or elastic file systems
•Decouple with queues, notification services, and orchestration tools
•May involve a large amount of development and migration effort as
well as expense

© Digital Cloud Training | https://digitalcloud.training
## Architecture Patterns –
Migration and Transfer

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – Migration and Transfer
Company is migrating Linux and
Windows VMs in VMware to the cloud.
Need to determine performance
requirements for right-sizing
Install the Application Discovery Service
discovery connector in VMware vCenter
to gather data
Company has a mixture of VMware
VMs and physical servers to migrate to
AWS and dependencies exist between
application components
Install the AWS MGN replication agent
and create Application groups to
migrate in waves
Need to migrate an Oracle data
warehouse to AWS
Migrate using AWS DMS and SCT to a
RedShift data warehouse
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
Architecture Patterns – Migration and Transfer
Snowball Edge used to transfer millions
of small files using a shell script.
Transfer times are very slow
Perform multiple copy operations at
one time by running each command
from a separate terminal, in separate
instances of the Snowball client
Need to minimize downtime for
servers that must be migrated to AWS
Use AWS MGN and perform a final
synchronization before cutting over in a
short outage window
Need to migrate 50TB of data and
company only has a 1Gbps internet
link. Requirement is urgent
Use AWS Snowball to transfer the data
RequirementSolution

© Digital Cloud Training | https://digitalcloud.training
## SECTION 17
Web, Mobile, ML, and Cost Management

© Digital Cloud Training | https://digitalcloud.training
AWS Amplify and AppSync

© Digital Cloud Training | https://digitalcloud.training
AWS Amplify
•Tools and features for building full-stack applications on
## AWS
•Build web and mobile backends, and web frontend UIs
•AWS Amplify Studio is a visual interface for building web
and mobile apps:
•Use the visual interface to define a data model, user
authentication, and file storage without backend expertise
•Easily add AWS services not available within Amplify Studio
using the AWS Cloud Development Kit (CDK)
•Connect mobile and web apps using Amplify Libraries for iOS,
Android, Flutter, React Native, and web (JavaScript)
•AWS Amplify Hosting is a fully managed CI/CD and hosting
service for fast, secure, and reliable static and server-side
rendered apps

© Digital Cloud Training | https://digitalcloud.training
AWS AppSync
•AWS AppSync is a fully managed service that makes it
easy to develop GraphQL APIs
•Applications can securely access, manipulate, and receive
real-time updates from multiple data sources such as
databases or APIs

© Digital Cloud Training | https://digitalcloud.training
AWS AppSync
•AWS AppSync automatically scales a GraphQL API execution
engine up and down to meet API request volumes
•Uses GraphQL, a data language that enables client apps to
fetch, change and subscribe to data from servers
•AWS AppSync lets you specify which portions of your data
should be available in a real-time manner using GraphQL
## Subscriptions
•AWS AppSync supports AWS Lambda, Amazon DynamoDB,
and Amazon Elasticsearch
•Server-side data caching capabilities reduce the need to
directly access data sources
•AppSync is fully managed and eliminates the operational
overhead of managing cache clusters

© Digital Cloud Training | https://digitalcloud.training
AWS AppSync
Example of using AppSync and Amplify to
simplify access to microservices
Amplify is used to
build and host the
WebStore application
and create backend
services
AppSync creates a
unified API layer for
integrating the
microservices

© Digital Cloud Training | https://digitalcloud.training
AWS Device Farm

© Digital Cloud Training | https://digitalcloud.training
AWS Machine Learning
and AI Services

© Digital Cloud Training | https://digitalcloud.training
AWS Rekognition
Identify objects
Perform facial analysis
Celebrity recognition

© Digital Cloud Training | https://digitalcloud.training
AWS Rekognition in Event-Driven Architecture
## S3 Bucket
AWS LambdaAmazon Rekognition
Amazon SNSAWS Lambda
Amazon DynamoDB
User uploads image
Upload to S3 triggers a
Lambda function
Rekognition publishes result
status to an SNS Topic
A Lambda function
processes the results
and creates an item in
DynamoDB
Rekognition analyzes
the image

© Digital Cloud Training | https://digitalcloud.training
AWS Rekognition
•Add image and video analysis to your applications
•Identify objects, people, text, scenes, and activities
in images and videos
•Processes videos stored in an Amazon S3 bucket
•Publish completion status to Amazon SNS Topic

© Digital Cloud Training | https://digitalcloud.training
## Amazon Transcribe
•Add speech to text capabilities to applications
•Recorded speech can be converted to text before it
can be used in applications
•Uses a deep learning process called automatic
speech recognition (ASR) to convert speech to text
quickly and accurately

© Digital Cloud Training | https://digitalcloud.training
## Amazon Translate
•Neural machine translation service that delivers
fast, high-quality, and affordable language
translation
•Uses deep learning models to deliver more accurate
and more natural sounding translation
•Localize content such as websites and applications
for your diverse users

© Digital Cloud Training | https://digitalcloud.training
## Amazon Comprehend
•Natural-language processing (NLP) service
•Uses machine learning to uncover information in
unstructured data
•Can identify critical elements in data, including
references to language, people, and places, and the
text files can be categorized by relevant topics
•In real time, you can automatically and accurately
detect customer sentiment in your content

© Digital Cloud Training | https://digitalcloud.training
## Amazon Lex
•Conversational AI for Chatbots
•Build conversational interfaces into any application
using voice and text
•Build bots to increase contact center productivity,
automate simple tasks, and drive operational
efficiencies across the enterprise

© Digital Cloud Training | https://digitalcloud.training
Amazon DevOps Guru
•Cloud operations service for improving application
operational performance and availability
•Detect behaviors that deviate from normal
operating patterns
•Benefits:
•Automatically detect operational issues
•Resolve issues with ML-powered insights
•Elastically scale operational analytics
•Uses ML to reduce alarm noise

© Digital Cloud Training | https://digitalcloud.training
Amazon CodeGuru Security
•Detect, track, and fix code security vulnerabilities
anywhere in the development cycle using ML and
automated reasoning
•Integrates with IDEs and CI/CD tools
•Automated bug tracking
•Assisted remediation through suggested code fixes
•Offers performance optimization recommendations
•Detects anomalies in application profiles

© Digital Cloud Training | https://digitalcloud.training
Process and Analyze Images

© Digital Cloud Training | https://digitalcloud.training
Process and Analyze Images
## S3 Bucket
AWS LambdaAmazon Rekognition
Amazon DynamoDB
User uploads image
Upload to S3 triggers a
Lambda function
The Lambda function receives the results
and creates an item in DynamoDB
Rekognition analyzes
the image

© Digital Cloud Training | https://digitalcloud.training
AWS License Manager

© Digital Cloud Training | https://digitalcloud.training
AWS License Manager
•Used to manage licenses from software vendors
•For example, manage your Microsoft, Oracle, SAP
and IBM licenses
•Centralized management of software licenses for
AWS and on-premises resources
•Can track license usage including when licensed
based on virtual cores (vCPUs), sockets, or
number of machines
•Distribute, activate, and track software licenses
across accounts and throughout an organization
•Enforce limits across multiple Regions

© Digital Cloud Training | https://digitalcloud.training
AWS Compute Optimizer

© Digital Cloud Training | https://digitalcloud.training
AWS Compute Optimizer
•Recommends optimal AWS resources for your
workloads to reduce costs and improve
performance
•Uses machine learning to analyze historical
utilization metrics
•Offers optimization guidance for:
•Amazon EC2 instances
•Amazon EBS volumes
•AWS Lambda functions
•Results can be viewed in the console or via the CLI

© Digital Cloud Training | https://digitalcloud.training
AWS Compute Optimizer

© Digital Cloud Training | https://digitalcloud.training
AWS Compute Optimizer

© Digital Cloud Training | https://digitalcloud.training
AWS Cost Explorer

© Digital Cloud Training | https://digitalcloud.training
AWS  Cost Allocation Tags

© Digital Cloud Training | https://digitalcloud.training
AWS Cost Management Tools

© Digital Cloud Training | https://digitalcloud.training
AWS Cost Explorer
•The AWS Cost Explorer is a free tool that allows you
to view charts of your costs
•You can view cost data for the past 13 months and
forecast how much you are likely to spend over the
next three months
•Cost Explorer can be used to discover patterns in how
much you spend on AWS resources over time and to
identify cost problem areas
•Cost Explorer can help you to identify service usage
statistics such as:
•Which services you use the most
•View metrics for which AZ has the most traffic
•Which linked account is used the most

© Digital Cloud Training | https://digitalcloud.training
AWS Cost & Usage Report
•Publish AWS billing reports to an Amazon S3
bucket
•Reports break down costs by:
•Hour, day, month, product, product resource, tags
•Can update the report up to three times a day
•Create, retrieve, and delete your reports using the
AWS CUR API Reference

© Digital Cloud Training | https://digitalcloud.training
AWS Price List API
•Query the prices of AWS services
•Price List Service API (AKA the Query API) –   query
with JSON
•AWS Price List API (AKA the Bulk API) – query
with HTML
•Alerts via Amazon SNS when prices change