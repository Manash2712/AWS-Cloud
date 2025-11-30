### Solution

- First lets search for elastic ip in search bar, and select elastic ips.
- Then click on allocate elastic ip
- Leave everything default and under tags click on add new tag.
- In key put name and in value put ```xfusion-eip```
- Then click on allocate.
- Once its allocated on the elastic ips screen you can edit its name to ```xfusion-eip```.

#### Notes:
- An AWS Elastic IP (EIP) is a static, public IPv4 address designed for cloud environments that can be programmatically associated with and remapped to different resources, such as EC2 instances. Its primary benefit is to provide a consistent, public-facing endpoint for your applications that doesn't change, even if the underlying instance fails or needs to be replaced.

#### Key features and benefits
- Static IP: Unlike the dynamic public IP addresses assigned to instances, an Elastic IP does not change when you stop and start an instance. 
- Flexibility: You can quickly remap the Elastic IP from one instance to another within your AWS account, which is useful for failover or maintenance without updating DNS records. 
- Instance failure: In the event of an instance failure, you can instantly reassign the EIP to a healthy instance, minimizing downtime and maintaining a consistent public endpoint for your users. 
- Management: You can allocate, associate, and disassociate an Elastic IP using the AWS Management Console or programmatically through the AWS SDK. 
- Cost: You do not get charged for an Elastic IP if it is associated with a running instance. However, you will be charged a small fee for an Elastic IP that is not associated with an instance. 

#### How it works
- Allocate: You allocate a static public IPv4 address from AWS and it becomes yours until you release it. 
- Associate: You then associate this Elastic IP address with a specific EC2 instance or network interface. The instance's default public IP (if it had one) is released. 
- Remap: If the instance becomes unavailable, you disassociate the Elastic IP from it and associate it with a different, healthy instance. This allows traffic to be redirected to the new instance while using the same IP address. 
