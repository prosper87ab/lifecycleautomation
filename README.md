# # 🔐 Active Directory Home Lab Project

## 📌 Project Overview
This project simulates a real-world enterprise IT environment using Active Directory. The goal was to demonstrate how user identities are created, managed, secured, and governed within a Windows domain environment.

The lab replicates common IT Help Desk and IAM responsibilities such as user provisioning, group-based access control, and policy enforcement using Group Policy Objects (GPOs).

---

## 🎯 Objectives
- Deploy and configure Active Directory Domain Services (AD DS)
- Create and manage users, groups, and Organizational Units (OUs)
- Implement Group Policy Objects (GPOs) for security and control
- Simulate real-world IT support tasks (password resets, account lockouts, etc.)
- Automate administrative tasks using PowerShell

---

## 🛠️ Technologies & Tools Used
- Windows Server 2019 / 2022  
- Active Directory Domain Services (AD DS)  
- Group Policy Management (GPO)  
- Microsoft Azure (Virtual Machines) *(or VirtualBox/VMware)*  
- PowerShell (for automation)  
- Remote Desktop Protocol (RDP)

---

## 🏗️ Lab Architecture
Describe your setup here in simple terms:

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

```powershell
# Example snippet
New-ADUser -Name "John Doe" -GivenName "John" -Surname "Doe"




