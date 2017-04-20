# VPC

## Synopsis

The vpc.template file leverages nested templates to  deploy either a 2 or 3 tiered network VPC. This set of templates
will also created replication subnet groups for RDS, ElastiCache, and Redshift in all private subnets. 

The end result is as follows:

![multi-tiered network vpc](https://github.com/elnica6/cloudformation_templates/blob/master/images/multi_network_tier_vpc.png)
