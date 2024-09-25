# CHAPTER 3: COMPUTE TECHNOLOGIES AND SERVICES

## Chapter 3.1: Compute: The Bigger Picture

Ec2 have 6 types of instance consist of: General purpose, Compute optimized, Memory optimized, Storage optimized, Accelerated computing, high performance computing optimized.

03-Ondemand-EC2.JPG

03-spot-instance.JPG

03-dedicated-host.JPG

03-Reserved-Instance.JPG

03-Saving-plans.JPG

## Chapter 3.2: EC2 feature review

[Ec2 features comparing](https://aws.amazon.com/vi/elasticloadbalancing/features/)

[compute optimizer support guidance](https://aws.amazon.com/vi/blogs/compute/aws-compute-optimizer-supports-aws-graviton-migration-guidance/)

### Load Balancing

having 4 types of load balancing

- Classic: Often use in many case, used for layer 4/7

- Gateway: used in layer 3/4, used to monitoring with third party virtual appliance.

- Application: Layer 7, flexible application management

- Network: extreme performance and static IP, used in layer 4

### Auto scaling

two types of automatic scaling: horizontal and vertical scaling

## Chapter 3.3 Demo

![Connect to EC2](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/03-Connect-to-EC2.JPG)

## Chapter 3.4: Containers: The Bigger Picture

![AWS-container-service](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/03-AWS-container-service.JPG)

![ECS and EKS](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/03-ECS-EKS.JPG)

> Biggest different between ECS and EKS is supporting docker of ECS and kubernetes of EKS

## Chapter 3.5: Serverless Services: The Bigger Picture

Lambda is serverless compute service without managing server. the code you write called function and you can use many languages such as: python, Rust, Rubby.

![Lambda-using](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/03-lambda-using.JPG)

Fargate is pay as you go auto-scaling compute engine

![fargate-service](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/03-fargate-service.JPG)

![Fargate-usecase](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/03-Fargate-usecase.JPG)

![Fargate-usecase](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/03-Fargate-usecase-2.JPG)

## Chapter 3.6: Understanding Serverless Services Pricing and Features

- Lambda feature

![Lambda-feature](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/03-Lambda-feature.JPG)

- Lambda pricing

![lambda-pricinge](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/03-lambda-pricinge.JPG)

- Fargate pricing

![Fargate-pricing](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/03-Fargate-pricing.JPG)

> The different of Lambda is free for 1 million request a month, and Fargate has no upfront costs, pay only for resource used such as: memory and cp and storage.

## Chapter 3.7: Demo, Lambda in action

## Chapter 3.9: Introducing Additional Compute Services

![Additional-compute-service](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/03-Additional-compute-service.JPG)

### Outposts
it supports hybrid deployment models while maintaining the local data residency requirements.

### Lightgsail
it is used to quickly launch small projects

### Batch
it process larger workload in small peices batches

### WaveLength
Allow users and devices to reach application without leaving the 5G mobile network.

