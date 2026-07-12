# cloud concept 24%

* Iaas >> you manage server and os (e.g ec2)
* PaaS >> you responseable code and data, AWS manage Iac (e.g Elastic Beanstalk) 
* SaaS >> final product you use it direct (e.g Gmail)

&#x20;

* Deployment models 
1. puplic
2. private (on-premises)
3. hybrid



* Capex >> buy first  to buy hardware
* Oppex >> pay-as-you-go >> model AWS





* AWS well- Architected framework

1-operational excellence >> power and monitor system to business value 

2- security >> secure system and information

3- realiabilty >> system ability to slove problem 

4- performance efficiency >> use resorces smart

5- cost optimization >> avoid cost  not neccssary

6-sustainability >> reduce  environmental impact of cloud services

# security and compliance 30%

* shared responsibility model

&#x20;1- AWS >> respose  security of the cloud (security of the cloud),secure Iac,hardware,networks,datacenters



2- customer >> response secirty in the cloud ,your data,os(update),encrypt,seting of the fiirewale



* IAM 

&#x20;1- users (someone or app)

&#x20;2- groups (users group with same permission)

&#x20;3- roles (time permission >>usually gives to service aws to communicate with another sevice e.g  ec2 connect s3)

&#x20; 4- polices( JSON files select permission (least privilege))



* AWS WAF (firewale to secure web app(secure attack SQL Injection))
* AWS Shield basises secure and advance aginst ataak DDOS
* Amazon Macie >> use ai to discover and secure to sensitive data
* AWS CloudTrail >> record all API Calls(who you work and where and when ?useful to review and Auditing)
* AWS KMS  >> manage encrypts key
* Amazon Gaurduty >> service discover threat detection by usu machine learning to monitor account active and find Malicious activity or not factuly
* Amazon Inspector >> check automatic tools (automated vulnerability management)check servers ec2 and containers to search software flaws
* AWS Artifact >> Central portal for accessing dedicated security and compliance reports (e.g iso,soc)
* AWS CloudWatch >> service monitoring performance metrics ex. cpu usage >> alarms or start Auto Scaling
* AWS Trust Advisor >> tools check your account  and give advice (real-time guiedance) debends on  5 field best practice (cost, performance,security,handiling errors,service limit)
* AWS Config >> service record and category resources seteing(configrations)if you need whats  change in security groups from week to day



# technology and services 34%

* global Infrastructure

&#x20;1-regions >> separate geographical locations around the world

&#x20;2- availability zones(AZs) >> data centers more and isolate inside the same region to available high availability

&#x20;3- edge locations >> nearby points of end users to cachenig speed(cloudfront)



* compute 

&#x20;1- Amazone Ec2 >> virtual machines

&#x20;2- AWS lambda >> start code without manage servers(serverless)

&#x20; 3-Amazone ECS/EKS >> manage and start containers (Docker \& Kubernetes)

&#x20;4- AWS Fargate >> compute engine process serverless to ECS AND EKS ,make containers start without need manage servers ec2 

* storage

&#x20;1-Amazone S3 >> object storage to files and photos and backups(durability 11 >>9)

&#x20;2- Amazone EBS >> Block Storage link with EC2 in the same az one server

&#x20;3-Amazone EFS >> Shared files system can link it to more Linux sever in the same time (more az more server)

&#x20;4- AWS Snow Family >> physical devices for transferring massive amounts of data (betabytes) to AWS without using the internet

5- Amazon s3 Glacier >> category of s3 spical to data Archeving ,it not need want it speed ,the cost very low but ,data recovery takes time(from minutes to hours)

* Datebases

&#x20;1- Amazone RDS >> reational databases (SQL,MYSQL,PostgreSQL) AWS response updates,patching and backups

&#x20; 2-Amazone DynamoDB >> non reational databases (NOSQL)very speed(serverless )

&#x20;3- Amazone Redshift >> Dtae Warehouse to anylysis big data 

4- Amazon Aurora >> reational databases of AWS ,integratded with MYSQL AND PostgreSQL but it 5 speed and low cost 



* Networking 
1. &#x20;Amazone VPC >> isolate private network on AWS
 1-subnets >> div vpc to small network(public,private)
 2-security group >> work a virtual firewale level on instances ec2
 3-NACLs (Network Access Control Lists) >> work  afirewale level on subnet
2. Amazone Route 53 >> DNS Service (Domain Forwarding)
3. Amazone CloudFront >> content deliver network (CDN) to accelerate websites loading
4. Elastic Load Balencer(ELB)>> distribute incoming traffic acroos multible servers to ensure system does not fail under load
5. Auto Scaling >> usually work with ELB,it add new server when increase triffic (scale out),and remove it when reduce traffic (scale in)  

# Biling,Pricing and Support 12%



* model cost ec2
1. on-demand >> pay by second or hours high choice cost but not commitment
2. reserved instances >> book one year or 3 years ,significant reduction (suitable for constant loads)
3. spot instances >> exploits surple resources to AWS ,cheapest option (discount of up to 90%),however aws cloud shut it down on you at any time (suitable for batch processing)

4\. saving plans >> greater booking flexibility ,subject to a minimum spending requirement in exchange for discount



* cost management tools
1. AWS Pricing Calculator >> cost estimation prior to project construction
2. AWS Cost Explorer >> Analyzing current and past cost data and generating forecasts
3. AWS Budgets >> create a budget and receive alerts if you exceed the allowed limit
4. SCPs (Service Control Polices)>> allow and deny some service on the all accounts 



* Support plans 
1. Basic >> free,Access to customer service and documentation only 
2. Developer >> Email technical support during business hours(respone via 12 :24 hours)
3. Business >> 24/7n technical support via chat and phone  (for the production environment)(respone via one our)
4. Enterprise >> very fast technical support with a dedicated technical Account Manager (TAM)(response in 15 minutes if imergancy)



* AWS Organization >> manage and link AWS accounts with advantages consolidated Billing









# KEY Words





|AWS Service|Keyword|
|-|-|
|AWS lambda|serverless compute /run code without managing servers|
|AWS CloudTrail|who did what and when /track API calls /Auditing|
|Amazon CloudWatch|Performance monitoring /Metrics/Alarm/logs|
|AWS Trust Advisor|Best Practise guidance /Cost optimization checks|
|Amazon RDS|SQL/Relational Databases/managed database|
|Amazon DyanmoDB|NOSQL/Key-value/Single-digit millisecond latency|
|Amazon Redshift|date warehouse/Analytic on massive datasets|
|Amazon CloudFront|Content Delivery Network(CDN)/Low Letancy/Caching|
|Amazon Route 53|DNS/Domain Name routing|
|AWS Shield|Protect against DDoS attacks|
|AWS WAF|Protect against SQL injection \& cross-site Scripting|
|Amazon Guarduty|Threat detection/Malicious activity/Machine Learning|
|Amazon Macie|PII/Senstive data protection in s3 /machine leaerning|
|IAM Role|Temporary credentials/grant permission to AWS service|
|AWS Artifact|Compliance reports/ISO /SOC|
|AWS ClouudFormation|IaC/Provision using templates|
|AWS Organization |Centralized account management /Consolidated billing|
|AWS Pricing Calculator|Estimate cost before provisioning resources|
|AWS Cost Explorer|Analyze past and current cost /Forecast future cost|
|Amazon VPC|Virtual Private Network/isolated section of AWS cloud|
|Amazon ElasticCache|Sub-millisecond latency/in memory data store/ cache|
|AWS Snowball/Snowmobile|Transfer Petabytes/Exabytes of data offline|
|Amazon EFS|Shared file system for Linux instances|
|Amazon EBS|Block Storage attached to a single EC2 instance|



