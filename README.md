# ☁️ Google Cloud Security Incident Response & Remediation Project

## 📖 Overview

This project demonstrates the investigation, containment, remediation, and recovery of a simulated cloud security incident in a Google Cloud Platform (GCP) environment.

The objective was to identify security vulnerabilities, analyze the impact of a data breach, implement remediation measures, and validate compliance improvements using cloud security best practices. The project involved working with Security Command Center findings, securing cloud resources, hardening infrastructure configurations, and verifying the effectiveness of remediation actions.

---

## 🎯 Project Objectives

- Investigate security findings related to a cloud security breach.
- Identify vulnerable cloud resources and security misconfigurations.
- Contain and recover compromised infrastructure.
- Implement cloud security best practices.
- Reduce the attack surface of the environment.
- Improve security visibility through logging and monitoring.
- Verify remediation efforts through compliance reporting.

---

## 🏢 Incident Scenario

A major security breach was detected within a Google Cloud environment. Security investigations revealed multiple critical vulnerabilities across cloud resources, including publicly accessible storage, exposed administrative services, overly permissive firewall configurations, and insecure virtual machine settings.

The objective was to investigate the incident, contain the threat, recover affected resources, remediate vulnerabilities, and improve the overall security posture of the cloud environment.

---

## 🔍 Security Investigation & Analysis

The investigation was conducted using Google Cloud Security Command Center (SCC) and PCI DSS compliance reports.

### Key Findings

| Finding | Severity |
|----------|----------|
| Public Bucket ACL | High |
| Public IP Address Exposure | High |
| Open SSH Port | High |
| Open RDP Port | High |
| Firewall Logging Disabled | Medium |
| Full API Access Enabled | Medium |
| Default Service Account Usage | Medium |
| Secure Boot Disabled | Medium |

These findings revealed multiple security weaknesses that increased the risk of unauthorized access, data exposure, and infrastructure compromise.

---

## 🖥️ Compute Engine Recovery

To recover from the compromised environment:

- Stopped the compromised virtual machine.
- Created a replacement VM using a clean snapshot.
- Removed public internet exposure by disabling the external IP address.
- Configured controlled network access using security tags.
- Enabled Shielded VM Secure Boot.
- Deleted the compromised virtual machine.

### Security Benefits

✔️ Eliminated compromised infrastructure

✔️ Restored workloads from a trusted source

✔️ Reduced external attack vectors

✔️ Improved workload integrity and resilience

---

## 🗄️ Cloud Storage Security Hardening

Cloud Storage permissions were reviewed and secured by:

- Preventing public access to the storage bucket.
- Removing public permissions and anonymous access.
- Switching from Fine-Grained Access Control to Uniform Bucket-Level Access.
- Enforcing centralized IAM-based access management.

### Security Benefits

✔️ Eliminated public data exposure

✔️ Improved access governance

✔️ Enforced least-privilege principles

✔️ Strengthened storage security controls

---

## 🔥 Firewall Security Improvements

Firewall configurations were reviewed and hardened by:

- Restricting SSH access through Google Cloud Identity-Aware Proxy (IAP).
- Creating a dedicated firewall rule for controlled administrative access.
- Removing overly permissive firewall rules.
- Restricting unnecessary network exposure.
- Enabling firewall rule logging.

### Security Benefits

✔️ Reduced attack surface

✔️ Improved administrative access control

✔️ Minimized unauthorized access attempts

✔️ Enhanced network security posture

---

## 📊 Compliance Verification

After remediation activities were completed:

- PCI DSS compliance findings were reviewed.
- Critical security vulnerabilities were validated as remediated.
- Security controls were verified.
- Compliance posture was improved.

### Outcome

✔️ High-severity vulnerabilities addressed

✔️ Improved cloud security posture

✔️ Enhanced monitoring and audit visibility

✔️ Strengthened overall security governance

---

## 🛠️ Technologies & Services Used

- Google Cloud Platform (GCP)
- Security Command Center (SCC)
- Compute Engine
- Cloud Storage
- Identity and Access Management (IAM)
- VPC Firewall Rules
- Identity-Aware Proxy (IAP)
- PCI DSS Compliance Reporting

---

## 🧠 Skills Demonstrated

- Cloud Security Operations
- Incident Response
- Security Monitoring & Analysis
- Vulnerability Assessment
- Infrastructure Hardening
- Identity & Access Management
- Firewall Security
- Compliance Validation
- Risk Assessment
- Security Best Practices

---

## 📄 Project Deliverables

- Security Incident Investigation
- Vulnerability Analysis
- Infrastructure Recovery
- Cloud Security Hardening
- Compliance Verification
- Technical Security Report

---

## 📁 Repository Structure

```text
.
├── README.md
├── Google_Cloud_Security_Incident_Report.pdf
└── screenshots/
```

---

## 🎓 Key Learning Outcomes

This project provided practical experience in responding to a cloud security incident from investigation through remediation and verification. It reinforced the importance of secure cloud configurations, proactive monitoring, least-privilege access control, compliance validation, and defense-in-depth security strategies.

---

## ⚠️ Disclaimer

This project was completed in a controlled educational cloud environment for learning and portfolio development purposes. No real-world production systems or customer data were involved.

---

## 👨‍💻 Author

**Seelam Narrammagari Amogh**

B.Tech – Cyber Security  
Vignan's Institute of Information Technology


*"Securing cloud environments through continuous learning, practical experience, and security-first thinking."*