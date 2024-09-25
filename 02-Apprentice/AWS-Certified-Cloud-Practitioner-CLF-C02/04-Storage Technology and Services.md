# CHAPTER 4: Storage Technology and Services

## Chapter 4.1: Exploring amazon ec2 storage Services

### EBS 

![EBS](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/04-EBS.JPG)

### EFS

![EFS](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/04-EFS.JPG)

### Instance Storage

![Instance-storage](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/04-Instance-storage.JPG)

Instance storage use case:

![Instance-storage-useCase](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/04-Instance-storage-useCase.JPG)


## Chapter 4.2: Amazon Simple Storage Service (S3): The Bigger Picture

![S3](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/04-S3.JPG)

### What it is? 

### S3 components

### Benefit of S3

### Use cases

## Chapter 4.3: Exploring S3 Storage Classes

[S3 storage classes](https://aws.amazon.com/vi/s3/storage-classes/)

### Standard
high througput performance and low latency, suitable for frequently accessed data

### Intelligent-Tiering
support moving data between two storage class. suitable or perfect for unpredictable access pattern
it's designed to saving cost without performance impact

### Infrequent-access classes
Access less frequently, but rapid access when need it.

- one zone Infrequent-access suitable for secondary backup.

### Glacier classes

- S3 glacier instant retrieval: archive data, instant retrieval

- S3 glacier flexible retrieval: archive the storage, not immediate access or retrieval

- S3 glacier deep archive: archive storage along 10 years or more. Retrieval can take up 12 hours

### Tips

## Demo S3 in Action

- Bucket name is globally unique

- S3 bucket will encrypted automatically

- be aware of difference between bucket policy and IAM console. first one specific permission of accessed user, and the other one will controll who can access to S3 Bucket

- lifecycle policies will move object from specific storage class to another one automatically. it will help to save cost for your.

## Chapter 4.6: Additional Storage Service
![Elastic-Disater-Recovery](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/04-Elastic-Disater-Recovery.JPG)

### Amazon FSx
FSx is for windows and it offers seamless integration

### Elastic Disater Recovery
it is not only data backuped also provisioning power and continuity plan...

## Chapter 4.7: Amazon Elastic Block Storage

![EBS-types](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/04-EBS-types.JPG)

## Chapter 4.8: AWS Storage Gateway

why use storage GW: 

- cost-effective: reduce on-premise storage infrastructure

- secure: Data encrypted for safe transfer and stroage

- Seamless integration: Integrates with existing applications without disrupting the operation

- four types of aws S3:

S3 file Gateway: Keep your data in native format on cloud / in cloud-native format

Volume Gateway: offer stores and cached volume

Tape Gateway: for archive long term access data.

FSx file Gateway: extends on-premise file system

## Chapter 4.9: Overview of AWS Backup

### AWS resources

EBS, DynamoDB table, EC2, Relational Database service, Elastic file system, FSx file system, Storage Gateway Volume

### Core Features

- Centralize management

- automated backup scheduling

- Encryption and compliance 

- Cross-region & Account backup

### Use cases

Cloud-native backup

hybrid data protection

Data protection compliance 

### Recovery

## Chapter 4.10: Storage Exam Tip

