AWS Asset management

https://summitroute.com/blog/2018/06/05/cloudmapper_collect/

https://zinatullin.com/2019/11/12/how-to-inventory-your-aws-assets/

https://duo.com/blog/introducing-cloudmapper-an-aws-visualization-tool

https://summitroute.com/blog/2018/06/18/how_to_inventory_aws_accounts/

AWS VAPT and Patch managment

AWS Pro Prep

https://www.linkedin.com/pulse/how-i-passed-aws-certified-solution-architect-exam-glenn-richard-bech/

GCP Pro Prep

https://www.linkedin.com/pulse/how-i-passed-google-professional-cloud-architect-exam-khan/


Open topics:

* EMR - general setup 
* Spot instances - allocation strategy and rebalancing
* EC2 dedicated hosting and changing, limits https://docs.aws.amazon.com/general/latest/gr/aws_service_limits.html#limits_ec2 https://docs.aws.amazon.com/general/latest/gr/ec2-service.html
* Storage gateway - types and use cases
* SQS - details, cloud watch metrics (backlog per instance)
* ENI attachment https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-eni.html
* AWS DR patterns
* Restore Glacier to S3
* Launch templates https://docs.aws.amazon.com/autoscaling/ec2/userguide/LaunchTemplates.html
* EMR Dynamo DB https://docs.aws.amazon.com/emr/latest/ReleaseGuide/EMRforDynamoDB.html
* Kinesis - Analytics vs Straems https://docs.aws.amazon.com/solutions/latest/real-time-iot-device-monitoring-with-kinesis/overview.html
* Direct Connect vs Direct Gateway - https://docs.aws.amazon.com/whitepapers/latest/aws-vpc-connectivity-options/aws-direct-connect.html https://docs.aws.amazon.com/whitepapers/latest/aws-vpc-connectivity-options/network-to-amazon-vpc-connectivity-options.html

Allocation strategies in Auto Scaling groups help you to provision your target capacity without the need to manually look for the Spot Instance pools with spare capacity. AWS recommends using the capacity optimized strategy because this strategy automatically provisions instances from the most-available Spot Instance pools. You can also take advantage of the capacity optimized allocation strategy in Spot Fleet. Because your Spot Instance capacity is sourced from pools with optimal capacity, this decreases the possibility that your Spot Instances are reclaimed. Reference: Best practices for EC2 Spot.

Capacity Rebalancing helps you maintain workload availability by proactively augmenting your fleet with a new Spot Instance before a running Spot Instance receives the two-minute Spot Instance interruption notice. When Capacity Rebalancing is enabled, Auto Scaling or Spot Fleet attempts to proactively replace Spot Instances that have received a rebalance recommendation, providing the opportunity to rebalance your workload to new Spot Instances that are not at elevated risk of interruption. Capacity Rebalancing complements the capacity optimized allocation strategy (which is designed to help find the most optimal spare capacity) and the mixed instances policy (which is designed to enhance availability by deploying instances across multiple instance types running in multiple Availability Zones). Reference: Best practices for EC2 Spot.
