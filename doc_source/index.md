# Amazon Virtual Private Cloud User Guide

-----
*****Copyright &copy; Amazon Web Services, Inc. and/or its affiliates. All rights reserved.*****

-----
Amazon's trademarks and trade dress may not be used in
connection with any product or service that is not Amazon's,
in any manner that is likely to cause confusion among customers,
or in any manner that disparages or discredits Amazon. All other
trademarks not owned by Amazon are the property of their respective
owners, who may or may not be affiliated with, connected to, or
sponsored by Amazon.

-----
## Contents
+ [What is Amazon VPC?](what-is-amazon-vpc.md)
+ [How Amazon VPC works](how-it-works.md)
+ [Get started with Amazon VPC](vpc-getting-started.md)
+ [IP addressing for your VPCs and subnets](vpc-ip-addressing.md)
   + [VPC CIDR blocks](vpc-cidr-blocks.md)
   + [Subnet CIDR blocks](subnet-sizing.md)
   + [Group CIDR blocks using managed prefix lists](managed-prefix-lists.md)
      + [Work with customer-managed prefix lists](working-with-managed-prefix-lists.md)
      + [Work with AWS-managed prefix lists](working-with-aws-managed-prefix-lists.md)
      + [Work with shared prefix lists](sharing-managed-prefix-lists.md)
      + [Reference prefix lists in your AWS resources](managed-prefix-lists-referencing.md)
   + [AWS IP address ranges](aws-ip-ranges.md)
   + [Migrate your VPC from IPv4 to IPv6](vpc-migrate-ipv6.md)
   + [AWS services that support IPv6](aws-ipv6-support.md)
+ [Virtual private clouds (VPC)](configure-your-vpc.md)
   + [Default VPCs](default-vpc.md)
   + [Create a VPC](create-vpc.md)
   + [Configure your VPC](modify-vpcs.md)
   + [DHCP option sets in Amazon VPC](VPC_DHCP_Options.md)
      + [DHCP option set concepts](DHCPOptionSetConcepts.md)
      + [Work with DHCP option sets](DHCPOptionSet.md)
   + [DNS attributes for your VPC](vpc-dns.md)
   + [Network Address Usage for your VPC](network-address-usage.md)
   + [Share your VPC with other accounts](vpc-sharing.md)
      + [Example of sharing public subnets and private subnets](example-vpc-share.md)
   + [Extend a VPC to a Local Zone, Wavelength Zone, or Outpost](Extend_VPCs.md)
   + [Delete your VPC](delete-vpc.md)
+ [Subnets for your VPC](configure-subnets.md)
   + [Create a subnet](create-subnets.md)
   + [Configure your subnets](modify-subnets.md)
   + [Subnet CIDR reservations](subnet-cidr-reservation.md)
   + [Configure route tables](VPC_Route_Tables.md)
      + [Example routing options](route-table-options.md)
      + [Work with route tables](WorkWithRouteTables.md)
      + [Middlebox routing wizard](middlebox-routing-console.md)
         + [Manage middlebox routes](working-with-routing-console.md)
         + [Middlebox scenarios](middlebox-routing-examples.md)
            + [Inspect traffic destined for a subnet](internet-gateway-subnet.md)
            + [Inspect traffic using appliances in a security VPC](gwlb-route.md)
            + [Inspect traffic between subnets](intra-vpc-route.md)
   + [Delete a subnet](subnet-deleting.md)
+ [Connect your VPC to other networks](extend-intro.md)
   + [Connect to the internet using an internet gateway](VPC_Internet_Gateway.md)
   + [Enable outbound IPv6 traffic using an egress-only internet gateway](egress-only-internet-gateway.md)
   + [Connect to the internet or other networks using NAT devices](vpc-nat.md)
      + [NAT gateways](vpc-nat-gateway.md)
         + [NAT gateway use cases](nat-gateway-scenarios.md)
         + [DNS64 and NAT64](nat-gateway-nat64-dns64.md)
         + [Monitor NAT gateways with Amazon CloudWatch](vpc-nat-gateway-cloudwatch.md)
         + [Troubleshoot NAT gateways](nat-gateway-troubleshooting.md)
      + [NAT instances](VPC_NAT_Instance.md)
      + [Compare NAT gateways and NAT instances](vpc-nat-comparison.md)
   + [Associate Elastic IP addresses with resources in your VPC](vpc-eips.md)
   + [Connect your VPC to other VPCs and networks using a transit gateway](extend-tgw.md)
   + [Connect your VPC to remote networks using AWS Virtual Private Network](vpn-connections.md)
   + [Connect VPCs using VPC peering](vpc-peering.md)
+ [Monitoring your VPC](monitoring.md)
   + [Logging IP traffic using VPC Flow Logs](flow-logs.md)
      + [Flow log record examples](flow-logs-records-examples.md)
      + [Work with flow logs](working-with-flow-logs.md)
      + [Publish flow logs to CloudWatch Logs](flow-logs-cwl.md)
      + [Publish flow logs to Amazon S3](flow-logs-s3.md)
      + [Publish flow logs to Kinesis Data Firehose](flow-logs-firehose.md)
      + [Query flow logs using Amazon Athena](flow-logs-athena.md)
      + [Troubleshoot VPC Flow Logs](flow-logs-troubleshooting.md)
   + [CloudWatch metrics for your VPCs](vpc-cloudwatch.md)
+ [Security in Amazon Virtual Private Cloud](security.md)
   + [Data protection in Amazon Virtual Private Cloud](data-protection.md)
   + [Identity and access management for Amazon VPC](security-iam.md)
      + [How Amazon VPC works with IAM](security_iam_service-with-iam.md)
      + [Amazon VPC policy examples](vpc-policy-examples.md)
      + [Troubleshoot Amazon VPC identity and access](security_iam_troubleshoot.md)
      + [AWS managed policies for Amazon Virtual Private Cloud](security-iam-awsmanpol.md)
   + [Internetwork traffic privacy in Amazon VPC](VPC_Security.md)
   + [Control traffic to resources using security groups](vpc-security-groups.md)
      + [Security groups](security-groups.md)
      + [Security group rules](security-group-rules.md)
      + [Default security groups for your VPCs](default-security-group.md)
   + [Control traffic to subnets using Network ACLs](vpc-network-acls.md)
   + [Infrastructure security in Amazon VPC](infrastructure-security.md)
   + [Resilience in Amazon Virtual Private Cloud](disaster-recovery-resiliency.md)
   + [Compliance validation for Amazon Virtual Private Cloud](VPC-compliance.md)
   + [Security best practices for your VPC](vpc-security-best-practices.md)
+ [Use Amazon VPC with other AWS services](related-services.md)
   + [Connect your VPC to services using AWS PrivateLink](endpoint-services-overview.md)
   + [Filter network traffic using AWS Network Firewall](network-firewall.md)
   + [Filter DNS traffic using Route 53 Resolver DNS Firewall](resolver-dns-firewall.md)
+ [VPC examples](vpc-examples-intro.md)
   + [Example: VPC for a test environment](vpc-example-dev-test.md)
   + [Example: VPC for web and database servers](vpc-example-web-database-servers.md)
   + [Example: VPC with servers in private subnets and NAT](vpc-example-private-subnets-nat.md)
+ [Amazon VPC quotas](amazon-vpc-limits.md)
+ [Document history](WhatsNew.md)