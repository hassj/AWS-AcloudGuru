# CHAPTER 5: STORAGE

## Chapter 5.1 Studying STORAGE

- file STORAGE 

- block STORAGE (EC2 is using)

- object STORAGE ( ex: S3 , aws services also have aws storage gateway- provide unlimited access from on premise to cloud; aws datasync - easily transfer data to AWS upto 10 times than normal)

![S3 types](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Image/05-S3-types.JPG)

[s3 object classes](https://aws.amazon.com/vi/s3/storage-classes/)

![Storage SlA](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Image/05-Storage-SLA.JPG)

![Amazon s3 glacier](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Image/05-Amazon-s3-glacier.JPG)

## Chapter 5.3: Amazon EFS (elastic file system)

![EFS is](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Image/05-EFS-is.JPG)

![EFS](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Image/05-EFS.JPG)

- EFS have two storage classes bellow, it is automatically grows and shrinks. It supported encrypted

![EFS storage classes](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Image/05-EFS-storage-classes.JPG)

## Chapter 5.4 Solving STORAGE gateway 

- in case you want to access to virtual storage unlimited form your premise or your data center, that is the case you use aws STORAGE gateway. Having 3 type of aws STORAGE gateway

+ File gateway: gives you SMB and NFS interface to s3 

![File gateway](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Image/05-file-gateway.JPG)

+ Tape gateway: you want to store tape backup content to cloude, you should use Tape gateway like virtual tape library on your local netowrk.

![tape gateway](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Image/05-Tape-gateway.JPG)

+ Volume gateway: play as volume on local virtual machine with data stored on s3 cloud. with two modes: cached mode and store mode.

![Voluem gateway](https://github.com/hassj/AWS-DEVOPS-AcloudGuru/blob/main/01-Novice/Image/05-voluem-gateway.JPG)






