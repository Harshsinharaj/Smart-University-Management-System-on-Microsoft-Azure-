# Smart University Management System on Microsoft Azure

**Developed By:** Harsh Raj (Computer Science Student)  
**University:** Lovely Professional University, Punjab-144411, India  
**Course:** INT 327 - Cloud Infrastructure and Resource Management

---

## 📌 Overview

A secure, scalable, cloud-based **Smart University Management System** using **Microsoft Azure** and **Terraform (Infrastructure as Code)**. This enterprise-level architecture demonstrates modern cloud engineering practices with focus on security, governance, and disaster recovery.

---

## 🏗️ Architecture Components

### Infrastructure Deployed
- **1** Resource Group
- **3** Virtual Networks (VNets)
- **3** Subnets
- **3** Network Security Groups (NSGs)
- **3** Linux Virtual Machines
- **3** Storage Accounts
- **1** Public IP
- **1** Recovery Services Vault

### VNet Configuration
- **Campus-VNet:** 10.0.0.0/16
- **Subnets:** Admissions, Library, IT, Finance, Hostel (10.0.x.0/24)

---

## 🔐 Security Implementation

- **NSGs** for network-level security
- **SSH** restricted to specific IPs
- **Role-Based Access Control (RBAC)** with Microsoft Entra ID
- **Department-wise access isolation**
- **SAS tokens** for secure temporary storage access
- **Zero Trust security model**

### Identity & Access Management
| Group | Access | Roles |
|-------|--------|-------|
| Engineering | VM1 + Storage1 | VM Contributor |
| Business | VM2 + Storage2 | Storage Blob Data Contributor |
| Operations | VM3 + Storage3 | VM Contributor |

---

## 💾 Storage & Data Management

- **3 Storage Accounts** (one per department)
- **Data Isolation** by department
- **SAS Token** access (time-limited, permission-controlled)
- **Blob Storage** for documents, PDFs, images

---

## 🎯 Key Features

✅ Department-wise network segmentation  
✅ Secure identity management (Entra ID)  
✅ RBAC-based access control  
✅ Azure Policy governance (VM size restrictions)  
✅ Automated daily backups with 7-day retention  
✅ Infrastructure as Code (Terraform)  
✅ 19 resources deployed with zero manual errors  

---

## 🛠️ Azure Services Used

| Service | Purpose |
|---------|---------|
| Resource Group | Central management |
| VNet & Subnets | Network infrastructure |
| Entra ID | Identity management |
| RBAC | Access control |
| Virtual Machines | Department servers |
| Storage Accounts | Secure data storage |
| Azure Policy | Governance & compliance |
| Recovery Vault | Backup & disaster recovery |

---

## 📂 Virtual Machines

| VM Name | Department | OS |
|---------|-----------|-----|
| Admissions-VM | Admissions | Windows Server |
| IT-VM | IT | Ubuntu |
| Finance-VM | Finance | Windows Server |
| Library-VM | Library | Ubuntu |

---

## 🔄 Backup & Disaster Recovery

- **Automated daily backups**
- **7-day retention policy**
- **Recovery Services Vault** for business continuity
- **VM-1 backup enabled**

---

## 📚 Real-World Applications

This architecture is applicable to:
- Universities & Colleges
- Schools & Training Institutes
- Corporate Organizations
- Enterprise Cloud Deployments

---

## 📋 References

- 📸 **Screenshots:** [Google Drive](https://drive.google.com/drive/folders/1hCSj8-kPNdwD0UA6A0zcwClGd1-yLBE7?usp=sharing)
- 🎥 **Video Demo:** [Google Drive](https://drive.google.com/file/d/14A3mFKl94YU9OFykUaaO19FnZNaAx7qZ/view?usp=drive_link)

---

## 👤 Developer Info

**Name:** Harsh Raj  
**Email:** harshrajb46@gmail.com  


---

## 📝 Conclusion

This project demonstrates an **enterprise-level cloud architecture** implementing:
- Secure networking
- Identity & access control
- Virtualization
- Storage systems
- Governance & compliance
- Backup & recovery
- Infrastructure automation

All reflecting real-world cloud engineering practices used in modern organizations.

---

**Status:** ✅ Successfully deployed to Azure & pushed to GitHub
