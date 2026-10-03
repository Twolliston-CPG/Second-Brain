

What is the IP CIDR of a default VPC




in Amazon Web Services (AWS), the default Virtual Private Cloud (VPC) in every region is assigned the ==IPv4 CIDR block== **`172.31.0.0/16`**


This CIDR block provides the following: 
- **Total IP Addresses:** 65,536 (ranging from `172.31.0.0` to `172.31.255.255`)
- **Default Subnets:** Automatically created in each Availability Zone (AZ) with a **`/20`** CIDR block
- **Subnet IPs:** 4,096 IP addresses per default subnet (with a few reserved by AWS for internal networking








   