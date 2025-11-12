# activedirectory
Using Active Directory via Windows Server
Video Link to watch the lab project: https://youtu.be/XlRqgagB5bg

## **Active Directory & Domain Controller Home Lab Project**

### **Objective**

To demonstrate proficiency in deploying and managing an on-premises Active Directory environment using Windows Server 2022, including domain setup, organizational unit design, user management, group policy configuration, and remote administration.

---

### **Environment Setup**

* **Platform:** Virtualized environment using VirtualBox / VMware
* **Server OS:** Windows Server 2022 (Domain Controller)
* **Client OS:** Windows 10 and Windows 11 (virtual machines)
---

### **Phase 1: Lab Architecture Design**

1. **Created virtual network** with internal NAT and host-only adapters for communication between all virtual machines.
2. **Deployed Windows Server 2022 VM** with 4GB RAM and assigned a static IP address.
3. **Configured hostname** to identify the Domain Controller within the network.

---

### **Phase 2: Install & Configure Active Directory Domain Services (AD DS)**

1. **Installed the Active Directory Domain Services (AD DS)** role using Server Manager.
2. **Promoted the server to a Domain Controller** and created a new forest
3. **Configured DNS integration** during promotion to manage internal name resolution.
4. **Installed and configured DHCP Server role** for automatic IP assignment to client devices.
5. **Created DHCP scope** with proper DNS, gateway, and domain name options.

---

### **Phase 3: Organizational Structure Design**

1. **Created Organizational Units (OUs)** to logically separate users and devices:
2. **Used PowerShell scripts** to automate creation of 1000+ bulk user accounts.

---

### **Phase 4: Domain Joining & Client Configuration**

1. **Deployed two Windows 10/11 client VMs** configured to use the Domain Controller as their DNS server.
2. **Joined all client machines** to the domain through System Properties.
3. **Tested login** using standard domain user accounts to verify successful domain integration.

---

### **Phase 5: Group Policy Management**

1. **Created and linked Group Policy Objects (GPOs)** for:

   * Password complexity and expiration policies
   * Software restriction rules
2. **Tested policy enforcement** by logging into domain-joined clients and confirming settings applied as expected.

---

### **Phase 6: Remote Support & Administrative Scenarios**

1. **Practiced common help desk tasks** including:

   * Password resets and account unlocks in Active Directory Users and Computers (ADUC)
   * Adding users to security groups
   * Remote software installation
   * Troubleshooting user connectivity and permission issues

---

### **Outcome**

Successfully configured a fully functional on-premises Active Directory environment simulating enterprise network operations, demonstrating capabilities in:

* Directory and identity management
* Group Policy administration
* DHCP/DNS configuration
* Remote troubleshooting and user support

---

### **Key Skills Demonstrated**

* Windows Server 2022 Administration
* Active Directory Domain Services (AD DS)
* DNS & DHCP Management
* Group Policy Object (GPO) Configuration
* PowerShell Scripting for User Automation

---
