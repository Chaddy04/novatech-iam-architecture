# NovaTech IAM Architecture (AWS)

## 🏢 Project Overview

This project simulates an organization (NovaTech Solutions) with ~75 employees transitioning to AWS. The goal is to design a secure and scalable IAM structure using best practices.

---

## 🎯 Objectives

* Implement role-based access control (RBAC)
* Enforce least privilege access
* Simulate departmental access in a real-world environment

---

## 🏗️ IAM Structure

### Departments:

* Engineering Team
* HR Team
* Finance Team
* Support Team

### Groups Created:

* Engineering-Team → EC2 & S3 Access
* HR-Team → S3 Read-Only Access
* Finance-Team → Billing Access
* Support-Team → CloudWatch Read-Only

---

## 👥 Users (Simulated)

* john.engineer
* mary.hr
* david.finance
* lisa.support

---

## 🔐 Security Implementation

* MFA enabled for admin IAM user (`richard.admin`)
* Strong password policy enforced
* Root account restricted to emergency use only

> Note: In a real production environment, MFA would be enforced for all users.

---

## 🧠 Key Learnings

* Importance of least privilege
* Role-based access control simplifies management
* IAM misconfiguration can lead to major security risks

---

## 🚧 Challenges Faced

* IAM login issues (resolved by using IAM sign-in URL)
* Understanding policy assignment per department

---

## 📌 Future Improvements

* Implement custom IAM policies
* Restrict S3 access to specific buckets
* Enforce MFA across all users
