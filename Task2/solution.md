### Solution

#### For this task first login to the AWS console. Then follow below steps:
- Search for security groups on the search bar and then go to security groups.
- Then click on the create security group button on right side.
- Then under basic details put security group name and description as mentioned in the task. Note keep the VPC as default.
- Now under inboud rules click on add rule.
- Select HTTP as type of inboud rule and in source select it as anywhere which means ```0.0.0.0/0```.
- Again click on add rule.
- This time select SSH as type of rule and in source select anywhere.
- Note: Do not touch outbound rules until you are very sure of what you are doing.
- Now click on ```Create security group``` button.

This way you can create a security group under default VPC.
