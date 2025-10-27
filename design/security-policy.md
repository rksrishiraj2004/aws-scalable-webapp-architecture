# Security Policy – AWS Scalable Web Application Architecture

This document outlines the security measures implemented in the AWS architecture to protect data, control access, and maintain compliance.

---

## 1. Identity & Access Management (IAM)
- Implemented least privilege access control.
- Created dedicated IAM roles for EC2 and RDS.
- Enabled Multi-Factor Authentication (MFA) for all users.
- Restricted root account access.

---

## 2. Network Security
- Configured Virtual Private Cloud (VPC) with public and private subnets.
- Applied Security Groups and Network ACLs for traffic filtering.
- ALB restricted to HTTPS (port 443) with SSL certificate.
- AWS WAF used for additional protection against attacks.

---

## 3. Data Protection
- Enabled KMS encryption for data at rest (S3, EBS, and RDS).
- Enforced SSL/TLS for data in transit.
- Enabled S3 block public access and versioning.

---

## 4. Monitoring & Logging
- CloudWatch and CloudTrail enabled for event tracking.
- AWS Config used to monitor configuration changes.
- Alerts configured for unauthorized access or configuration drift.

---

## 5. Backup & Disaster Recovery
- Automated RDS backups enabled.
- S3 cross-region replication for redundancy.
- Periodic recovery tests performed to validate data integrity.

---

✅ *Outcome:* A secure, compliant, and resilient AWS environment adhering to best practices.
