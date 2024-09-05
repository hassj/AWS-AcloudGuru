# CHAPTER 8: MANAGEMENT AND GOVERNANCE

## Chapter 8.1: Memorizing Management and Governance

1. Account management service

![Account MANAGEMENT service](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/08-Account-management-service.JPG)

- aws control tower: set up and govern a secure multi account aws environments

- aws Organizations: centrally govern and manage your environments across multi aws accounts

- aws budgets: Improve your planing and cost control

2. Provisionin services

![Provisioning service](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/08-Provisioning-service.JPG)

- AWS CloudFormation: Model and manage the AWS resource via code

- AWS service catalog: Create, govern, and organize aws resource 

- AWS opsWork: Automate AWS via code such as pupet, chef

- AWS marketPlace: deploy, test, buy app that run on AWS

3. Operating service

![Operating service](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/08-Operating-service.JPG)

- AWS cloudWatch: monitoring aws cloud via metric

- AWS config: evaluate and optimze aws resource configuration.

- AWS cloudtrail: tracking user activity across your aws Account

- AWS System Manager: Optimize performance and secure the cluster while managing alarge of aws accounts.

- AWS x-ray: analyze and debug AWS production application.

## Chatper 8.3: Composing CloudFormation 

(just like Teraform or azure resource template)

- It allows you to create AWS infrastructure like EC2, vpc, event Cloudfront content delivery network just via text file.

- It allows you to use yaml or json format to create aws resource via cloudformation template

![Cloudformation template](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/08-CloudFormation-Template.JPG)

> Note: CloudFormation allows to call nested template.

![CloudFormation template sample](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/08-CloudFormation-Template-Sample.JPG)

> some of features supported by CloudFormation is: automation, and scale quickly and immediately.

## Chapter 8.3: Collecting CloudWatch

- It collects information of user account or service via metric. Its also predefine many graph for collecting metric for many services.

![Amazon cloudWatch](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/08-Amazon-CloudWatch.JPG)

- It allows log storage send to it 

![Amazon cloudWatch](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/08-Amazon-CloudWatch-2.JPG)

- Example of log storage send log to cloudWatch

![Amazon cloudWatch](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/08-Amazon-CloudWatch-hands-on-lab.JPG)

## Chapter 8.4: Applying auto scaling

- It allow you to defines the condition which will be triger to automatically scaling EC2 running application or decrease if dont need it anymore, will help you to saving money

![Auto scaling](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/08-Auto-scaling.JPG)

![Auto scaling](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/08-Auto-scaling-02.JPG)

## Chapter 8.5: hands-on-lab

![Hands-on-lab](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/08-Hands-on-lab.JPG)

[AWS resource template](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-template-resource-type-ref.html)

[AWS resource repo](https://github.com/ACloudGuru-Resources/Course-Certified-Solutions-Architect-Associate)


