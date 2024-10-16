# CHAPTER 7: DEPLOYMENT MESSAGING, DEPLOYMENT TECHNOLOGY AND SERVICE

## Chapter 7.1: What is CI/CD?

Quickly integrate to share or central repository with small changes of code from multi branch or developer.

![CI-WorkFlow](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-CI-WorkFlow.JPG)

Automate build, test and package also deploy to application.

![CD-WorkFlow](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-CD-WorkFlow.JPG)

## Chapter 7.2: AWS Development Tools

!

### AWS CodeCommit
like Private git repository on cloud, automate control version from multi source after commit changes codes

![AWS-CodeCommit](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-AWS-CodeCommit.JPG)

### AWS CodeBuild
Automate build and test then package to the artifact like .net core, docker image, node.js package ready move on to aws CodeDeploy

![AWS-CodeBuild](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-AWS-CodeBuild.JPG)

### AWS CodeDeploy
Automate deploy artifact to environments like lambda, ec2 or onpremises quickly avoid downtime.

![AWS-CodeDeploy](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-AWS-CodeDeploy.JPG)

### AWS CodePipeline

A serials integrate many service like CodeCommit, CodeBuild, CodeDeploy like an orchestration service 

![Code-Pipeline](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Code-Pipeline.JPG)

![Code-Pipeline](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Code-Pipeline-02.JPG)

![Exam-tip](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Exam-tip.JPG)

## Chapter 7.3: Demo using AWS console and cloud shell

Create S3 bucket: 
```

aws --version
aws s3 mb s3://mybucket-unique-name-as-your			//mb: made bucket
aws s3 ls
echo >> "myname new file " > file.txt
ls
aws s3 cp file.txt s3://mybucket-unique-name-as-your
aws s3 ls s3://mybucket-unique-name-as-your 	//list object contained in remote s3 bucket
aws s3 mb help 

```

## Chapter 7.4: Using AWS cloud9

Cloud9 is aws online ide tool support many languages and including cli tool.

## Chapter 7.5: Understanding AWS CodeArtifact

### What is code artifact?

Central artifact repository: it's an artifact repository

![Code artifact](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Code-Artifact.JPG)

The benefit of codeArtifact: save time for developer of searching on the internet, unit the same version for multiple team.

![Code artifact scenario](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Code-Artifact-scenario.JPG)

### What is artifact?

![Artifact](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-artifact.JPG)

### Exams tips 

![Artifact Exam tips](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Exam-tips.JPG)

## Chapter 7.6: Decoupling Application Components

[Decoupling application components](https://docs.aws.amazon.com/prescriptive-guidance/latest/modernization-integrating-microservices/decouple-messaging.html)

![Application integration service](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Application-integrated-service.JPG)

inmong of the applicatoin integration service, SQS is the service used to decopling the applicaiton component.

### Exam tips

![Decoupling Application components tips](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Decoupling-application-component-tips.JPG)

## Chapter 7.7: Introducing Amazon Simple Notification Service (SNS)

What is SNS: easily setup, operate or send notification, sms, email supported

![What is SNS](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-What-is-SNS.JPG)

Pub and Sub model:

![What is SNS](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-pub-sub-model.JPG)

use case of SNS usage: 

![What is SNS](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-SNS-use-cases.JPG)

### Exam tips

SNS allows you to send or push notfication to subcriber.

![SNS exam tips](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-SNS-examp-tips.JPG)

## Chapter 7.9: Introducing Amazon Simple Queue Service (SQS)

SQS is an simple queue services. it is a temporary repository for messages awaiting processing.

![SQS](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-SQS.JPG)

### SQS key features

It is full-based that means it pull message from the Queue.

Multi consummer can pull message from same queue.

Message are processed asynchronously - that means concummer just pull message from queue no matter know the producer request message or not.

SQS message are guaranteed to be processed at least once.

![SQS key features](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-SQS-features.JPG)

### Scenario

![SQS scenarios](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-SQS-Scenario.JPG)

### Tips

![SQS Exam tips](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-SQS-tips.JPG)

## Chapter 7.10: Standard And FIFO Queues

### Standard Queue

- Some features of standard Queue

![SQS standard queue](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-SQS-standard-queue.JPG)

> guaranteed delivered message at least once
>
> best-effort ordering means that messages are deliverded in the same order as they sent 
>
> Occasionally more than one copy of messages might be delivered out of the order.

- Best-effort ordering

![SQS best effort ordering](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-SQS-best-effort-ordering.JPG)

- FIFO Queue - first in first out ordering

![SQS FIFO queue](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-FIFO-queue.JPG)

![SQS FIFO queue](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-FIFO-queue-2.JPG)

> FIFO queue is the best option for financial transaction in case the order strictly ensure. any duplicate transaction is gonna cause a problem

### Tips

FIFO and standard queue (defautl queue)

![SQS fifo and standard tips](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-SQS-standard-fifo-tips.JPG)

## Chapter 7.11: Short Polling vs Long Polling

![SQS short polling](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-SQS-short-polling.JPG)=

> you must still pay for this empty responses

![SQS long polling](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-SQS-long-polling.JPG)

> wait untill have mesages or timout of schedule time to get polling from the queue.

### Tips

![SQS polling tips](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-SQS-polling-tips.JPG)

## Chapter 7.12: What Is Amazon Simple Email Service (SES)?

![SES](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-SES.JPG)

![SES](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-SES-2.JPG)

### Tips

![SES tips](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-SES-tips.JPG)

> dont get it confused with SNS - SNS just send or push notfication or email as basic format or text format, whereas SES send the richly format 

## Chapter 7.13: Introducing Amazon EventBridge

![EventBridge](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Event-Bridged.JPG)

![EventBridge](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Event-Bridged-2.JPG)

EC2 (the service generate the state log), cloudwatch - monitoring service, cloudtrail - tracking user activity service will send event to eventbridge then match some pre-defined rules then route to 
appropriate target - target is a serice might be EC2, lambda, and finally take pre-defined action to do, such as send notification about changes using SNS, or lambda...

![EventBridge example](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Event-Bridged-example.JPG)

![EventBridge](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Event-Bridged-3.JPG)

### Tips

![EventBridge tips](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Event-Bridged-tips.JPG)

## Chapter 7.14: Understanding Step Functions

![Step functions](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Step-function.JPG)

Step Functions are a great way to visualize your serverless application. They automatically trigger and track each step in a process, and log the state of each step, so you can track what went wrong, and where.

https://learn.acloud.guru/course/1ab914a9-23d2-4776-9862-e2ab3cd24807/learn/42490b2f-4fd6-46de-8754-27036c237717/a954fa48-d905-4c8c-bd31-3cf18bc996d6/watch

## Chapter 7.15: Deploying Infrastructure as Code with AWS CloudFormation

IAC on AWS is cloudformation like teraform of Harshicorp

![Cloudformation](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-CloudFormation.JPG)

> resulting set of resources built by the template known as cloudformation stack

![Cloudformation benefits](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Cloudformation-benefit.JPG)

### Tips

![Cloudformation tips](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Cloudformation-tip.JPG)

## Chapter 7.17: What Is AWS Elastic Beanstalk?

it's an service help developer just focus on code instead of pay attention to another like: platform environment, web server type, or database  or managing infrastructure .... That's Elastic beanstalk comes in.

![Elastic BeanStalk](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Elastic-Beanstalk.JPG)

![Elastic BeanStalk](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Elastic-Beanstalk-2.JPG)

### Tips

![Elastic BeanStalk tips](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Elastic-Beanstalk-tips.JPG)

## Chapter 7.18: Elastic Beanstalk Demo

![Elastic BeanStalk demo](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Elastic-Beanstalk-demo.JPG)

[demo repository](https://github.com/pluralsight-cloud/AWS-Certified-Cloud-Practitioner-CCP-CLF-C02)

![Elastic BeanStalk demo tips](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Elastic-Beanstalk-demo-tips.JPG)

## Chapter 7.19: Demo: Using AWS X-Ray to Identify Performance Issues

X-Ray is a tool helps developer troubleshoot application performance and figure out root cuase of errors.

![X-Ray](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Xray.JPG)

![X-Ray scenario](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Xray-scenario.JPG)

### Tips

![X-Ray tips](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Xray-tips.JPG)

## Chapter 7.20: Development, Messaging, and Deployment Exam Tips - Part 1

CI-CD Tools

![Ci-CD tools](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-Ci-CD-review.JPG)

AWS deployment tools: 

![AWS deployment tool](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-AWS-deployment-tool.JPG)

AWS cloud shell and cli

![AWS cloudshell and cli](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-cloud-shell-cli.JPG)

AWS IDE browser-based tool

![AWS cloud 9](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-AWS-cloud9.JPG)

AWS Code Artifact: 

![AWS code artifact](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-AWS-code-artifact.JPG)

Decoupling application

![AWS decoupling application](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-AWS-Decoupling-application.JPG)

AWS SNS service 

![AWS SNS service](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-AWS-SNS-reviews.JPG)

## Chapter 7.21: Development, Messaging, and Deployment Exam Tips - Part 2

![SQS queues](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-SQS-review.JPG)

Polling types:

![SQS types of polling](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-SQS-Polling-types-reveiw.JPG)

Event Bridge:

![Event bridge](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/07-EventBridge-review.JPG)

