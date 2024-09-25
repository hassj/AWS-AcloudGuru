# CHAPTER 5: CONTENT DELIVERY AND NETWORKING TECHNOLOGY AND SERVICES

## Chapter 5.1: CDN

1. key benefits of CDN: 

- speed faster

- Reliability: automatically sacles on demand without disrupting application.	

- Global reach

2. Amazon Cloudfront

cost charging by data transfer but free for the first Terabyte network and including AWS free tier account

- Aws cloudfront provide security such as aws shield for DDOS protection and WAF to safeguard website from common web exploits.

- It also support seamless to other service like EC2, Route53 and S3...

3. Use cases

- helping streaming video smoothy

- Secure transaction like purchase information, or creadit card information....

- handling when traffice spike, it will help the application stable or surge without a hitch

## Chapter 5.2: AWS Global Accelerator

it is networking service that send user data to aws's CDN. AWS global Accelarator like a special path help you to choose the best data or path in AWS cloudfront networking.

1. Benefits

- Improve performance significance is throughput upto 60% 

- Simplified management with static public IP.

- Consistent global user experience

- Security and Reliability - DDoS resillience, automatic reroute 

2. Use cases

## Chapter 5.3: Networking: The Bigger Picture

![Network-vpc](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/05.Network.JPG)

Within AWS cloud account, we have an own VPC network, it will seperate your environment and resource with other. under VPC we have subnets, and attach each of subnets we have security group, each subnets will have route table used to route network traffic
 in and out the internet. many subnets residen within an Availability zone.

Security group will control inbound and outbound of each subnets resource like ec2...Network access controll list - NACLs will control traffic in and out the internet.

Each subnets within VPC must associated with an route 

Security groups are stateful which means that allow traffic incomming allowed will be allowed at outgoing direction automatically.

on the other hand NACLs is stateless firewall. it operates at subnet level

The main difference lies of NACLs and Security Groups is scope and the detail of each.

![05-Security-NACLs.JPG](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/05-Security-NACLs.JPG)

## Chapter 5.6: DNS: The Bigger Picture

![DNS](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/05-DNS.JPG)

![DNS](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/05-DNS-2.JPG)

## Chapter 5.7: Applying Hybrid Models with Networking Services

### Amazon Direct connect

![Amazon-Direct-connect](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/05-Amazon-Direct-connect.JPG)

### Amazon VPN

![Amazon-VPN](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/05-Amazon-VPN.JPG)

![vpn-direct-connect](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/02-Apprentice/AWS-Certified-Cloud-Practitioner-CLF-C02/Image/05-vpn-direct-connect.JPG)

## Chapter 5.8: Content Delivery and Networking Exam Tips

Cloudfront

## Route 53

Which feature of Amazon Route 53 helps to manage traffic for your application based on various criteria, such as geographic location? -> Traffic flow 


