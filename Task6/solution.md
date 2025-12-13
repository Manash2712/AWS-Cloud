### Solution

- Search for ec2 in the search bar.
- Then from the menu on left hand side go to instances.
- On right hand side click on launch instances.
- Put name as datacenter-ec2.
- From AMI choose amazon linux ami.
- Now in instance type select t2.micro.
- Then click on create new key pair.
- Put name of key pair as datacenter-kp, leave everything default and click create key pair.
- Now in firewall (security groups) choose select existing key pair and select the default security group.
- Click launch instance.

This way we can create ec2 instance in AWS along with its key pair to login.
