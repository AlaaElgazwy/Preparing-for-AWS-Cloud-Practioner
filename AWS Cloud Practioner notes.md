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



# technology and services 34%

* global Infrastructure

&#x20;1-regions >> separate geographical locations around the world

&#x20;2- availability zones(AZs) >> data centers more and isolate inside the same region to available high availability

&#x20;3- edge locations >> nearby points of end users to cachenig speed(cloudfront)



* compute 

&#x20;1- Amazone Ec2 >> virtual machines

&#x20;2- AWS lambda >> start code without manage servers(serverless)

&#x20; 3-Amazone ECS/EKS >> manage and start containers (Docker \& Kubernetes)

* storage

&#x20;1-Amazone S3 >> object storage to files and photos and backups

&#x20;2- Amazone EBS >> Block Storage link with EC2

&#x20;3-Amazone EFS >> Shared files system can link it to more Linux sever in the same time

&#x20;4- AWS Snow Family >> physical devices for transferring massive amounts of data (betabytes) to AWS without using the internet

* Datebases

&#x20;1- Amazone RDS >> reational databases (SQL,MYSQL,PostgreSQL)

&#x20; 2-Amazone DynamoDB >> non reational databases (NOSQL)very speed

&#x20;3- Amazone Redshift >> Dtae Warehouse to anylysis big data



* Networking 
1. &#x20;Amazone VPC >> isolate private network on AWS
2. Amazone Route 53 >> DNS Service (Domain Forwarding)
3. Amazone CloudFront >> content deliver network (CDN) to accelerate websites loading

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



* Support plans 
1. Basic >> free,Access to customer service and documentation only 
2. Developer >> Email technical support during business hours(respone via 12 :24 hours)
3. Business >> 24/7n technical support via chat and phone  (for the production environment)(respone via one our)
4. Enterprise >> very fast technical support with a dedicated technical Account Manager (TAM)(response in 15 minutes if imergancy)



* AWS Organization >> manage and link AWS accounts with advantages consolidated Billing



