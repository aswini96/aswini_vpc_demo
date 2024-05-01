# own_vpc_demo
project on custom vpc with public and private subnets with high availability and resiliency

Overview

This project demonstrates how to create a VPC that you can use for servers in a production environment. We can improve resiliency by deploying the servers in two or more Availability Zones, by using an Auto Scaling group and an Application Load Balancer. For additional security, we deploy the servers in private subnets whereas loadbalancer and NAt gateway are in public subnets. The servers receive requests through the load balancer and can connect to the internet by using a NAT gateway. To improve resiliency, we deploy the NAT gateway in both Availability Zones. We attach IGW(Internet gateway) to the vpc which acts as a entrypoint to enter into the private network.

