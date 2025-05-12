## VM Server setup
---
After encountering installation issues with Proxmox, I decided to pivot to XenServer for my virtualization platform.
XenServer provided a smoother setup experience and met my requirements for managing virtual machines effectively.
---
## VMs

I'm currently running a small lab environment with two main virtual machines, with plans to expand in the future as my projects grow:

Kali Linux Purple – Focused on OSINT and penetration testing tasks

Windows Server – Set up for Active Directory and Windows enterprise environment practice

BackBox Linux – Dedicated to pure OSINT workflows and tooling
 
---
## Links

- https://www.xenserver.com
  
- https://www.xenserver.com
  
- https://www.backbox.org

---
## Pictures

Installing XenServer
![image1](https://github.com/user-attachments/assets/074b5c85-d473-4905-b9e4-a3d968464bbb)

Install XenCenter to communicate with XenServer
![image0](https://github.com/user-attachments/assets/9a4e8029-8b4d-45b8-a8cf-213d48b4abb5)

Creating a Network share for VM ISOs
![image](https://github.com/user-attachments/assets/13567fc4-7cfa-4660-a09c-9c9d5d33a8e2)

Creating a vm group
![image](https://github.com/user-attachments/assets/9c2a89be-2626-4f81-b2f7-5a0f2754cc5a)

Configured a Kali Linux virtual machine optimized for OSINT and basic penetration testing tasks. The VM is allocated 2 virtual CPUs, structured as 1 socket with 2 cores, along with 4,032 MB (4 GB) of memory.
This setup is intentionally lightweight, as most standard OSINT and penetration testing activities don’t require extensive system resources. However, if I were to engage in more resource-intensive operations—such as password or hash cracking, I would scale up the CPU and memory allocations accordingly to meet performance demands.
![image](https://github.com/user-attachments/assets/7c31b9fd-e496-412f-96e7-61240f5a6f69)


