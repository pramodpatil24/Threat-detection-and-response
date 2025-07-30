# 🛡️ Automated Threat Detection & Response 

This simulates real-world cloud security incidents and demonstrates automated threat detection and response using AWS-native services. Infrastructure is provisioned with Terraform and integrates GuardDuty, AWS Config, Security Hub, CloudTrail, and Lambda.

> ⚙️ Designed as a portfolio project to showcase hands-on cloud security and DevSecOps engineering skills.

---

## 🚀 Key Features

- **AWS GuardDuty** detects port scans and other suspicious behavior
- **AWS Lambda** automatically isolates compromised EC2 instances
- **AWS Config** enforces compliance with encryption and network hardening rules
- **MITRE ATT&CK-aligned threat simulation**

---

## 🧰 Tech Stack

| Tool            | Purpose                         |
|-----------------|----------------------------------|      
| AWS EC2         | Target + attacker VMs            |
| AWS GuardDuty   | Threat detection                 |
| AWS Lambda      | Automated incident response      |
| AWS Config      | Compliance monitoring            |
| Python (Boto3)  | Lambda scripting                 |
| EventBridge     | Event-driven automation          |

---

## 🗺️ Architecture

![Architecture Diagram](images/architecture.png)

> *This diagram shows the flow from threat detection → Lambda response → EC2 isolation.*

---

## 🧱 Project Structure


## 🧪 Lab Walkthrough


## 📸 Screenshots

### 🔍 GuardDuty Finding – Port Scan Detection
GuardDuty identifies reconnaissance activity (`Recon:EC2/Portscan`) triggered by an Nmap scan.
![GuardDuty Port Scan](images/guardduty_finding.png)

---

### 🚨 Lambda Auto-Remediation – CloudWatch Logs
Lambda function is triggered automatically and removes ingress rules from the compromised EC2 instance.
![Lambda Logs](images/lambda_logs.png)

---

### 🔒 Quarantined EC2 Instance – Tag & Isolation
EC2 instance is tagged with `Quarantine=True` and its security group ingress rules are revoked.
![EC2 Quarantine](images/ec2_quarantine.png)

---

### 🧩 Security Hub – CIS AWS Foundations Benchmark
Security Hub shows enabled CIS benchmark and findings summary, validating compliance monitoring.
![Security Hub Compliance](images/security_hub_summary.png)

---

### ✅ AWS Config – S3 Bucket Encryption Rule
Config rule `s3-bucket-server-side-encryption-enabled` detects unencrypted S3 buckets in real-time.
![AWS Config Rule](images/aws_config_encryption_rule.png)

---

## 🎯 Skills Demonstrated

* Cloud Security Engineering (GuardDuty, Config, IAM, Security Hub)
* DevSecOps Automation with Terraform + Lambda
* Incident Response (detection → action flow)
* AWS Governance & Compliance (CIS, NIST)
* Real-world threat simulation with MITRE ATT\&CK mapping

---

## 👋 Author

**PRAMOD PATIL**
🔗 [LinkedIn](https://www.linkedin.com/in/pramod-patil742000/)

---

