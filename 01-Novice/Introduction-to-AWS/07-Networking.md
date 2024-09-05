# CHAPTER 7: NETWORKING

## Chapter 7.1: Negotiating Networking

1. cloud network

![Cloud-network](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/07-Cloud-network.JPG)

- vpc: isolating and provisioning network to connect your resources.

- private link: provide private link to connect vpc to on-premmise applications

- aws transit gateway: connect vpcs and on-premmise network.

2. Network scaling

![Network scaling](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/07-Network-scaling.JPG)

- ELB- elastic load balancing: distribute network traffic across a pool of resources

- AWS global accelerator: direct traffic to the aws global network to improve global application performance

3. Content delivery

![Content delivery](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/07-CDN.JPG)

- Amazon cloudfront: securly delivery content of application, data, video ... to global user with high performance transfer speed.

## Chapter 7.2: Valuing VPC

![VPC NETOWRK](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/07-VPC.JPG)

- NAT gateway : allows access to internet from inside

- Access control list: control and allow or denied network traffic to your application

- Internet gateway: you want form internet access into your application

## Chapter 7.3: Chosing Cloudfront

![Amazon cloudfront](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/07-Amazon-cloudFront.JPG)

![Amazon cloudfront](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/07-Amazon-cloudFront-2.JPG)

## Chapter 7.4: Revising Route 53

- weighted policy: smaller weight will received lower traffic than other.

## Chapter 7.5: Hands-on Lab

![Hands-on-lab](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Introduction-to-AWS/Image/07-Hands-on-Lab.JPG)

> Notice: troubleshooting when connect to EC2 https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/TroubleshootingInstancesConnecting.html#TroubleshootingInstancesConnectingSSH

- Create VPC -> subnet -> associate subnet to auomatically IP address -> create Internet Gateway -> create route table -> associate routeable to public subnet -> create NACL

