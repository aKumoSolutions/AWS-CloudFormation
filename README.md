# AWS CloudFormation

<p align="center">
  <img width="400" height="200" src="img/aws.gif">
</p>

<p align="center">
  <img width="400" height="200" src="img/CloudFormation.png">
</p>

## What is AWS CloudFormation?

AWS CloudFormation is a service that gives developers and businesses an easy way to create a collection of related AWS and third party resources and provision them in an orderly and predictable fashion.

[Official Documentation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html)


## Templates
| a | b |
| ------------ | ------------ |

| [s3bucket.yaml](templates/s3bucket.yaml) | simple CloudFormation Template that creates S3Bucket. |
| [taggeds3bucket.yaml](templates/taggeds3bucket.yaml) | simple CloudFormation Template that creates S3Bucket with Tags. 
| [parameterizeds3bucket.yaml](templates/parameterizeds3bucket.yaml) | simple CloudFormation Template that creats S3Bucket based on the following parameter inputs: |

* MyBucketName   

* TeamTagValue

* EnvTagValue 

[securitygroup.yaml](templates/securitygroup.yaml) - simple CloudFormation Template that creates SecurityGroup with Tags, and requires the following parameteres: 

* SGName  - name for the resource
* MyVpc   - VpcId for which the SG will be created

[ec2instance.yaml](templates/ec2instance.yaml) - CloudFormation Template that creates EC2-Instance with Tags, and requires the following parameteres: 

* AMIid - Amazon Image Id
* EC2Name - name of the EC2 resource
* EC2Type - EC2-Instance Type
* EnvTag - Value for Env Tag key
* KeyName - SSH Key name for SSH Access
* RootVolumeSize - Size of the root volume
* SubnetID - SubnetId to which the EC2 should be launched
* TeamTag - Value for Team Tag key

[ec2_sg.yaml](templates/ec2_sg.yaml) - CloudFormation Template that creates EC2-Instance and Security Group with Tags, and requires the following parameteres. 

Note: modify the file with your inputs. 
