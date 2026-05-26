# # 🔐 Identity Governance & The Lifecycle (Joiner, Mover, Leaver)

## 📌 Project Overview
Managing the digital identity lifecycle is a critical security and compliance requirement for modern enterprises. This project simulates an enterprise-grade Identity Governance and Administration (IGA) solution by automating the core phases of the identity lifecycle: Joiner (onboarding), Mover (cross-departmental transfers/promotion), and Leaver (offboarding).

By integrating an on-premises ecosystem with cloud-native identity providers, this project demonstrates how to enforce the principle of least privilege, eliminate manual provisioning bottlenecks, mitigate "privilege creep," and ensure secure, immediate de-provisioning.

---

## 🎯 Objectives
- Automate Identity Lifecycles: Implement automated Joiner, Mover, and Leaver workflows using data-driven logic from a simulated HR source.
- Establish Hybrid Identity Synchronization: Bridge the gap between on-premises infrastructure and cloud identity environments.
- Enforce Governance and Least Privilege: Ensure role-based access control (RBAC) adjusts dynamically when a user's corporate status or department changes.
- Secure Offboarding: Create a foolproof, automated "Leaver" protocol that revokes access across all integrated cloud and on-premises platforms simultaneously.

---

## 🛠️ Technologies & Tools Used
- Directory Services: Active Directory Domain Services (AD DS)
- Cloud Identity Providers (IdPs): Microsoft Entra ID, Okta  
- Automation & Scripting: PowerShell 
- Identity Sync Tools: Microsoft Entra Cloud Sync, Okta Active Directory Agent
- Virtualization: VMware Workstation Pro 
- Operating Systems: Windows Server 2025 (Domain Controller), Windows 11 Pro (Admin Workstation)
- Custom Domain Namespace: iamcloud.online

---

## 🏗️ Lab Architecture

- 1 Domain Controller (Windows Server)
- (Optional) 1–2 Client Machines (Windows 10/11)
- Domain: `yourdomain.local`
- Users organized into departments (HR, IT, Finance)

*(Insert diagram screenshot here)*

---

## ⚙️ Key Configurations

### 🔹 Active Directory Setup
- Installed AD DS role
- Promoted server to Domain Controller
- Configured domain: `yourdomain.local`

📸 *[Insert screenshot]*

---

### 🔹 User & Group Management
- Created Organizational Units (OUs)
- Added users and security groups
- Assigned permissions based on roles

📸 *[Insert screenshot]*

---

### 🔹 Group Policy Implementation
- Enforced password policies
- Configured account lockout policies
- Restricted user environments (e.g., control panel access)

📸 *[Insert screenshot]*

---

### 🔹 PowerShell Automation
- Scripted bulk user creation
- Automated account management tasks


###############################

Enterprise Hybrid Identity Architecture: Multi-Cloud Federated Access (Okta & Microsoft Entra ID)

## 📌 Executive Summary
Modern enterprise environments demand centralized, secure, and automated identity lifecycles. This project demonstrates the engineering and deployment of a resilient, production-grade **Hybrid Identity Pipeline**. Using an on-premises Active Directory forest as the single source of truth, this architecture establishes secure, real-time identity provisioning to the world's leading cloud Identity Providers (IdPs): **Okta** and **Microsoft Entra ID**. 

By layering **SAML 2.0 Federated Single Sign-On (SSO)** onto the pipeline, this project simulates a real-world enterprise infrastructure—reducing user friction, mitigating identity silos, and closing security gaps across third-party SaaS environments.

---

## 🏗️ Architectural Topology & Data Flow


