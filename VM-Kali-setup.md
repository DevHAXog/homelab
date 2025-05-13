
---

# **Home Lab Setup: XenServer & Kali Linux VM**  

## **XenServer Installation & Configuration**  
After encountering installation issues with Proxmox, I switched to **XenServer** for virtualization. The setup was smooth and well-suited for my homelab needs.  

### **Key Steps:**  
1. **Installed XenServer** on dedicated hardware.  
2. **Deployed XenCenter** (management GUI) to configure VMs, storage, and networking.  
3. **Created a network ISO share** for centralized VM installation media.  

#### **Screenshots:**  
- **XenServer Installation**  
  ![XenServer Install](https://github.com/user-attachments/assets/074b5c85-d473-4905-b9e4-a3d968464bbb)  
- **XenCenter Management Console**  
  ![XenCenter](https://github.com/user-attachments/assets/9a4e8029-8b4d-45b8-a8cf-213d48b4abb5)  
- **Network ISO Share Setup**  
  ![ISO Share](https://github.com/user-attachments/assets/13567fc4-7cfa-4660-a09c-9c9d5d33a8e2)  

---

## **Kali Linux VM Configuration**  
### **VM Specifications:**  
- **OS:** Kali Linux Purple (offensive/defensive security distro)  
- **vCPUs:** 2 (1 socket, 2 cores)  
- **RAM:** 4 GB (4,032 MB)  
- **Use Case:** OSINT, penetration testing, and security research.  

#### **Installation & Optimization:**  
- Lightweight setup for standard tasks (scalable for hash cracking if needed).  
- Screenshot: **Kali Purple Installation**  
  ![Kali Install](https://github.com/user-attachments/assets/87c60d56-1d41-452a-867d-1a1744f95b3e)  
- Screenshot: **VM Hardware Allocation**  
  ![Kali VM Config](https://github.com/user-attachments/assets/7c31b9fd-e496-412f-96e7-61240f5a6f69)  

---

### **Links**  
- [XenServer Official Site](https://www.xenserver.com)  

---
