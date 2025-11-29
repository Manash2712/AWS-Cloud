### Solution

#### For this task follow below steps:
- Search for subnets in search bar, and choose subnets in VPC option.
- In subnets click on create subnet button on right side.
- Choose default VPC in VPC ID section.
- In subnet name put ```nautilus-subnet```.
- Put this in subnet CIDR ```172.31.255.90/20```, you may choose this based on the VPC CIDR and other subnet CIDR.
- Lets keep all other details as default and click on create subnet.

#### Notes:
- CIDR (Classless Inter-Domain Routing) is a method for efficiently allocating IP addresses by grouping them into blocks, which improves routing efficiency and conserves addresses. To choose a CIDR block, determine the number of IP addresses your network needs, and then select a block size that has enough IPs while leaving room for future growth.
- How it works: The number after the slash (the subnet mask) indicates how many bits are "fixed" for the network and how many are variable "host" bits.A /24 means the first 24 bits are fixed, leaving 8 bits for host addresses, providing 256 total addresses (\(2^{8}\)).A /32 means all 32 bits are fixed, representing a single IP address.

#### How to choose a CIDR block
- Estimate your needs: Determine the maximum number of IP addresses you will need for the foreseeable future, including room for future growth.
- Select a CIDR block size: Based on your estimate, choose the appropriate CIDR prefix. Remember that a larger prefix (e.g., /24) means a smaller number of available IPs, while a smaller prefix (e.g., /16) provides a much larger range of addresses.
- Avoid overlaps: When creating multiple subnets, ensure their CIDR blocks do not overlap, or they won't be able to communicate correctly.
- Consider your network structure:
- For large networks: Use a smaller prefix like /16 for a VPC and then subnet it into smaller /24 or /26 blocks for different regions or security zones.
