# 🚀 Terraform AWS VPC & EC2 Setup

![Terraform](https://img.shields.io/badge/Terraform-v1.5-blue?style=flat-square) 
![AWS](https://img.shields.io/badge/AWS-Cloud-orange?style=flat-square) 
![Modules](https://img.shields.io/badge/Modules-Reusable-green?style=flat-square)

---

## 🌟 Project Overview

This project demonstrates **AWS infrastructure automation using Terraform**, following **modular, reusable, and real-world best practices**.

You will learn how to create:

- Custom **VPC** with public & private subnets across multiple Availability Zones 🌐  
- **Internet Gateway (IGW)** for public subnet access 🚪  
- **NAT Gateway + Elastic IP** for private subnet outbound traffic 🔁  
- Separate **Route Tables & Associations** for traffic flow 🛣️  
- **Security Groups** with controlled inbound/outbound rules 🔐  
- **EC2 Instance** deployed in custom VPC using Terraform module outputs 🚀  

---

## 📂 Folder Structure
```
Terraform-Aws-Vpc-Ec2-setup/
├── Modules/
│ ├── network/ # VPC, subnets, routes
│ ├── security/ # Security Group module
│ └── Ec2-Instance/ # EC2 instance module
├── screenshots/ # Project screenshots
├── main.tf # Root Terraform config
├── variables.tf # Root variables
├── outputs.tf # Root outputs
├── provider.tf # AWS provider config
└── README.md # Project documentation
```

---

## ⚡ Key Learnings

- Terraform **module isolation** & communication using `variables` and `outputs`  
- Correct usage of `count` and `[*]` **splat expressions**  
- Designing **reusable & scalable IaC code**  
- Hands-on experience with **AWS VPC networking, NAT, IGW, route tables, and EC2**  

---

## 🖥️ Screenshots

📌 All screenshots are in the `screenshots/` folder.

![Terraform Apply](screenshots/ 
<img width="1920" height="1080" alt="Screenshot (169)" src="https://github.com/user-attachments/assets/e3044ec9-7bb9-40f0-a361-7756bdf871d0" />
)  
![VPC & Subnets](screenshots/ 
<img width="1920" height="1038" alt="Screenshot (172)" src="https://github.com/user-attachments/assets/6ccf1933-9c52-4a1b-9971-2bd1c8d885a3" />
)  
![Route Tables & NAT Gateway](screenshots/<img width="1903" height="982" alt="Screenshot (174)" src="https://github.com/user-attachments/assets/7872dea6-7fbc-4803-b707-bb0f4f713f9f" />
)  
![Modules Block](screenshots/<img width="1920" height="1080" alt="Screenshot (170)" src="https://github.com/user-attachments/assets/e660d05f-6311-42ba-9f1c-8510dbe89f2a" />
)  


---

## 🚀 How to Run

1. **Clone the repository**
```bash
git clone https://github.com/Sk-Nagul-09/Terraform-Aws-Vpc-Ec2-setup.git
cd Terraform-Aws-Vpc-Ec2-Setup

```

2. Configure AWS credentials

``` bash
aws configure
```
3. Initialize Terraform

``` bash
terraform init
```

4. Plan and Apply
```bash
terraform plan
terraform apply
```
5. Verify Outputs

```bash
terraform output
```
🌐 Next Steps / Improvements

  Add Application Load Balancer (ALB)
  
  Configure Auto Scaling Groups (ASG)
  
  Integrate with CI/CD pipeline
  
  Add Terraform remote state for team collaboration
