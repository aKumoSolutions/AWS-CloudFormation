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


## [Templates](templates)
| Template | Description | Parameters |
| ------------ | ------------ | ----- |
| [s3bucket-example1.yaml](templates/s3bucket-example1.yaml) | CF Template that creates S3Bucket. |
| [s3bucket-example2.yaml](templates/s3bucket-example2.yaml)  | CF Template that creates S3Bucket with Tags. |
| [s3bucket-example3.yaml](templates/s3bucket-example3.yaml) | CF Template that creates S3Bucket based on parameters. | SampleBucketName  TeamTagValue EnvTagValue VersioningConfig |
| [securitygroup.yaml](templates/securitygroup.yaml) |  CF Template that creates SecurityGroup with Tags based on parameters. | SGName MyVpc |
| [ec2instance-example1.yaml](templates/ec2instance-example1.yaml) | CF Template that creates EC2-Instance with Tags based on parameteres. | AMIid EC2Type SubnetID RootVolumeSize EC2Name TeamTag EnvTag KeyName |
| [ec2instance-example2.yaml](templates/ec2instance-example2.yaml) | CF Template that creates EC2-Instance based on parameteres. | ImageId InstanceType SubnetId SSHKeyName SecurityGroupId |
| [ec2instance-example3.yaml](templates/ec2instance-example3.yaml) | CF Template that creates EC2-Instance and SecurityGroup. | No parameters - hardcoded values |