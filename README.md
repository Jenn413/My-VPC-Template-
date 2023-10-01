# My-VPC-Template-
VPC Template with Route Table, Internet Gateway, Nat Gateway, Public and Private Subnet

Created a VPC Template, with 2 private and 2 public subnets with well-structured CIDR. To enable an entry point of internet to my VPC,
I created an internet gateway and attached to my VPC, however the internet gateway alone will not suffice, 
so I created route table that has mapping entries, that determines how the  traffic will be directed I associated my public subnet to the route table that
has route (0.0.0.0/0) pointing to the internet gateway, Also for security reasons I created a NAT Gateway for my private subnets. 

For high availability I created 1 public and 1 private subnet in one availability zone. To make my template re-usable I created Parameters for my VPC and all my subnet CIDR Block
