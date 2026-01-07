# AZ-104 Secure Hub-and-Spoke Network Architecture (Azure)

## 📌 Project Overview
This project demonstrates the design and deployment of a **secure hub-and-spoke network architecture in Microsoft Azure**.  
The environment eliminates public VM exposure while enabling **private administration and private PaaS access**, aligning with **enterprise security best practices** and **AZ-104 exam objectives**.

---

## 🎯 Objectives
- Implement a **hub-and-spoke VNet architecture**
- Secure VM access without public IPs
- Enable private connectivity to Azure PaaS services
- Apply network security controls using NSGs
- Use Azure-native secure access services

---

## 🧱 Architecture

---

## 🔐 Security Design
- **No public IPs** assigned to virtual machines
- **Azure Bastion** used for secure RDP/SSH access over HTTPS (443)
- **Network Security Groups (NSGs)** restrict inbound traffic
- **Private Endpoint** enables private access to Azure Storage
- **Private DNS integration** ensures internal name resolution

---

## 🛠️ Technologies Used
- Azure Virtual Networks (VNets)
- VNet Peering
- Azure Bastion
- Network Security Groups (NSGs)
- Azure Virtual Machines
- Azure Storage Accounts
- Private Endpoints
- Private DNS Zones

---

## 🚀 Deployment Steps (High-Level)
1. Create a resource group
2. Deploy Hub VNet with Bastion subnet
3. Deploy Spoke VNet with workload subnet
4. Configure bidirectional VNet peering
5. Deploy private VM (no public IP)
6. Deploy Azure Bastion in Hub VNet
7. Apply NSG rules to restrict traffic
8. Create storage account with public access disabled
9. Configure private endpoint and DNS integration
10. Validate private connectivity and access

---

## ✅ Validation
- VM accessible only via Azure Bastion
- No inbound internet traffic allowed
- Storage account reachable only through private endpoint
- All traffic remains on Azure’s private backbone

---

## 📚 AZ-104 Exam Alignment
This project covers:
- VNet peering concepts (non-transitive)
- Secure administrative access patterns
- Private endpoints vs service endpoints
- NSG rule design
- Hub-and-spoke architecture use cases

---

## 📝 Resume Bullet
> Designed and deployed a secure hub-and-spoke Azure network using VNet peering, Azure Bastion, NSGs, and Private Endpoints to eliminate public VM exposure while enabling private PaaS access.

---

## 🔮 Future Enhancements
- Add Azure Firewall with UDRs
- Implement VPN or ExpressRoute connectivity
- Convert deployment to Bicep or Terraform
- Add monitoring with Azure Network Watcher

---

## 👤 Author
Kobe Butts  
Aspiring Cloud Engineer | AZ-104 Candidate
# azure-hub-and-spoke-secure-network
Secure hub-and-spoke Azure network using Bastion, NSGs, and Private Endpoints
