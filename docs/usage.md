# Usage

---
You can use the Terraform plug-in to execute any terraform script related to the AWS cloud services.


### **Examples**

You can use this plug-in to create an EC2 instance.

![Image 1](media/StepTerraform.png)


We can have the contents of the EC2.tf file as below

```
provider "aws" {
region = "us-east-1"
}

resource "aws_instance" "example" {
ami           = "ami-01816d07b1128cd2d"
instance_type = "t2.micro"
subnet_id     = "subnet-id*******"

tags = {
Name = "instance-name-xyz"
}

associate_public_ip_address = false
security_groups = ["sg-id******"]
}
```
