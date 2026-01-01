Terraform_Task_2

---

````markdown
# Terraform AWS EC2 Multi-Region Nginx Setup

## Task Description
Create two AWS EC2 instances in different regions and install Nginx on both using Terraform.

---

## Technologies Used
- AWS EC2
- Terraform
- AWS CLI

---

## Steps to Complete Task

1. **Setup AWS CLI**  
Configure AWS CLI with your credentials:
```bash
aws configure
````

2. **Install Terraform**
   Download and install Terraform on your machine.

3. **Write Terraform Configuration**

* Define AWS providers for two regions (e.g., `ap-south-1` and `us-east-1`).
* Create EC2 instances in each region.
* Use user-data scripts to install and start Nginx on boot.

4. **Initialize Terraform**

```bash
terraform init
```

5. **Apply Terraform Configuration**

```bash
terraform apply
```

Type `yes` to confirm.

6. **Verify Deployment**

* Check EC2 instances in AWS Console.
* Access Nginx using the public IP addresses in your browser.

---

## Important Notes

* Make sure security groups allow inbound HTTP (port 80) and SSH (port 22) traffic.
* Use EC2 Instance Connect or SSH key pairs to access instances if needed.
* Nginx installation happens automatically through user-data on instance start.

---

## Cleanup

Remove all resources created by Terraform:

```bash
terraform destroy
```

---

## Summary

This task helps understand:

* Managing multiple AWS regions with Terraform providers
* Automating EC2 provisioning and software installation
* Basic AWS networking and security group configuration

---

Would you like me to generate this as a file you can download?
```
