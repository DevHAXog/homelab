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

🖥️ Installing XenServer
This image captures the initial phase of installing XenServer on my dedicated hardware for virtualization. While the screen might be subtle here, it marks the beginning of building out a powerful and flexible homelab environment.

XenServer offers robust virtualization capabilities, and after running into Proxmox install issues, it became the right tool for the job. Looking forward to using it to manage my growing collection of security-focused VMs and labs. 💻⚙️
![image1](https://github.com/user-attachments/assets/074b5c85-d473-4905-b9e4-a3d968464bbb)

After getting XenServer installed on my hardware, the next step was to install XenCenter—the management console that allows you to interact with your XenServer environment via a GUI. XenCenter makes it easy to create, configure, and monitor virtual machines, manage storage, and apply patches.

This is a critical piece for managing my homelab infrastructure efficiently. With XenCenter, I can oversee all my VMs and test environments from a single pane of glass. 🖥️📡
![image0](https://github.com/user-attachments/assets/9a4e8029-8b4d-45b8-a8cf-213d48b4abb5)


To streamline ISO access across my virtualization environment, I created a network share for my VM_ISOs folder. This allows my XenServer host (or any other VM hypervisor) to mount and access ISO images directly over the network, saving time and reducing the need for manual file transfers.

This setup is especially useful when spinning up new virtual machines from different hosts or when managing multiple hypervisors in a lab environment.

🔧 Pro tip: Ensure permissions and password protection are configured properly to keep shared resources secure.
![image](https://github.com/user-attachments/assets/13567fc4-7cfa-4660-a09c-9c9d5d33a8e2)

Creating a VM group involves organizing multiple virtual machines under a single logical unit. 
This will allow for easier management, bulk operations, and streamlined deployment processes across environments such as development, testing, or production.

![image](https://github.com/user-attachments/assets/9c2a89be-2626-4f81-b2f7-5a0f2754cc5a)

Configured a Kali Linux virtual machine optimized for OSINT and basic penetration testing tasks. The VM is allocated 2 virtual CPUs, structured as 1 socket with 2 cores, along with 4,032 MB (4 GB) of memory.
This setup is intentionally lightweight, as most standard OSINT and penetration testing activities don’t require extensive system resources. However, if I were to engage in more resource-intensive operations—such as password or hash cracking, I would scale up the CPU and memory allocations accordingly to meet performance demands.
![image](https://github.com/user-attachments/assets/7c31b9fd-e496-412f-96e7-61240f5a6f69)

This screenshot captures the installation process of Kali Linux Purple, a defensive/offensive security distro tailored for blue and purple team operations. Here, the installer is scanning the installation media — a standard step before package selection and base system installation begins.
Kali Purple is a great addition to my lab for OSINT, threat emulation, and blue team experimentation. Looking forward to diving into its built-in tools and expanding my hands-on skills in detection, monitoring, and analysis. 👨‍💻🔍
![image](https://github.com/user-attachments/assets/87c60d56-1d41-452a-867d-1a1744f95b3e)

