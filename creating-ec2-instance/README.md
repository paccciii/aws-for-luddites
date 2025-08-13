## Here, we are going to create a simple ec2 instance:

# Creating an EC2 Instance with Terraform

This guide explains how to create and delete an EC2 instance using Terraform.  
It shows each step with screenshots.

---

## 1. AWS Dashboard Before Starting

Here is the AWS EC2 dashboard before creating the instance.

![AWS Dashboard Before Creation](images/aws_dashboard_before_creation.png)  
*This is the AWS dashboard after the instance is created.*

---

## 2. Initialize Terraform

Run the command:

```bash
terraform init
```
![terraform init](images/terraform_init_ec2.png)

This command downloads the necessary Terraform plugins and sets up the working directory.

## 3. Plan the Terraform Changes

Run the command:

```bash
terraform plan
```
![terraform plan](images/terraform_plan_ec2.png)  

This shows what Terraform will create, without making any changes yet.

## 4. Apply the Terraform Plan

Run the command:
```bash
terraform apply
```
![terraform apply](images/terraform_apply_ec2.png)  

This command creates the EC2 instance in AWS.

## 5. AWS Dashboard After Creation

![AWS Dashboard Creation](images/aws_dashboard_created.png)  

You can now see the new EC2 instance in the AWS dashboard.

## 6. Destroy the Terraform Resources

Run the command:

```bash
terraform destroy
```
![AWS Dashboard Delete](images/terraform_destroy_ec2.png)  
This command will delete the EC2 instance.
  

## 7. Destroy Confirmation

![AWS Dashboard Delete2](images/terraform_destroy2_ec2.png)
Terraform asks for confirmation before deleting the resources.

## 8. AWS Dashboard After Deletion

![AWS Dashboard after deletion](images/aws_dashboard_destroyed.png)
The EC2 instance is now deleted from AWS.

## Conclusion

You have now seen how to create and delete an EC2 instance using Terraform.
The steps are:

    Initialize Terraform

    Plan the changes

    Apply to create the instance

    Destroy to remove the instance