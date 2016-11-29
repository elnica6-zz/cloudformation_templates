# cloudformation_templates

## Synopsis

A library of CloudFormation templates I've crafted over time. 

## Motivation

I use these cloudformation templates for my own development purposes, and I share them frequently with others, so I decided to host them on GitHub to make sharing and improvement easier.

## Installation

Just clone the repo down and you are good to go!

The `orchestration` folder contains templates that leverage other templates throughout the folder structure via nested stacks to deploy purpose built solutions.

To use them in your AWS accounts, simply clone this entire repo to a private S3 bucket in your AWS account and maintain the folder structure. For example:

```
myprivatecloudformationbucket/

	cloudformation_templates/

		cloudtrail/

		cloudwatch/

		ec2/

		......

		orchestration/

		s3/

		vpc/

		......
```

THe `standalone` folder contains templates that are standalone and do not leverage other templates via nested stacks. They, too, deploy purpose built solutions from a single template file.

Once cloned, simply pass the name of your S3 bucket where the templates are stored to the `CloudFormationS3BucketName` parameter in any of the orchestration templates and you are off to the races!

## Contributors

So far...just me @elnica6.
