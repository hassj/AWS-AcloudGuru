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
