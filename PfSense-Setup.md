
# **pfSense Firewall Configuration Guide**

## **Initial Setup and Interface Configuration**

### **1. WAN Interface Setup**
Configured the WAN interface with DHCP to automatically obtain an IP address from the upstream network. This serves as the firewall's external connection.

![WAN Interface Configuration](https://github.com/user-attachments/assets/96d30e7e-73a6-45e8-8d5d-904e2c3bad09)
*The WAN interface was set to DHCP mode for automatic IP assignment from the ISP or upstream router.*

### **2. LAN Interface Configuration**
Assigned a static IP address (**Redacted**/24) to the LAN interface, which will serve as the default gateway for all internal lab devices.

![LAN Interface Configuration](https://github.com/user-attachments/assets/4747515b-a099-41b0-92e5-322c255a4abb)
*The LAN interface was configured with a static IP to provide consistent internal routing.*

## **Advanced Configuration**

### **3. DNS Server Settings**
Configured the following DNS settings:
- Primary DNS: 8.8.8.8 (Google DNS)
- Secondary DNS: Left Blank
- Enabled DNS forwarding to ensure reliable name resolution

![DNS Configuration](https://github.com/user-attachments/assets/d3c7d2a9-9e54-451e-a7ab-39addcf67494)
*DNS settings were optimized for both reliability and security.*

### **4. Firewall Rule Configuration**
Implemented basic firewall rules:
- Default deny policy for incoming WAN traffic
- Explicit allow rules for outbound LAN traffic
- ICMP (ping) enabled for network diagnostics

![Firewall Rules](https://github.com/user-attachments/assets/e2ee56b0-8ace-4a6b-b87f-d20cdd25ed4a)
*The firewall rules were configured to balance security with necessary functionality.*

### **5. System General Setup**
Configured essential system parameters including:
- Hostname: EdgeWall
- Domain: pflocal.com
- Timezone: UTC
- WebGUI protocol: HTTPS

![System General Configuration](https://github.com/user-attachments/assets/caa6568f-1c8a-4850-ad1e-9f5972d808f7)
*Basic system parameters were configured to establish proper identification and secure access.*

## **Verification and Testing**
1. Verified internet connectivity through the WAN interface
2. Confirmed LAN devices could access the internet through NAT
3. Tested DNS resolution from internal clients
4. Verified firewall rules were blocking unwanted traffic while allowing legitimate connections

## **Next Steps**
- Configure VLANs for network segmentation
- Set up VPN access for remote management
- Implement intrusion detection/prevention systems
- Create more granular firewall rules for specific services

## **Troubleshooting Notes**
- If WAN connectivity fails, verify physical connections and DHCP settings
- For DNS issues, check the resolver configuration and test with alternative DNS servers
- Firewall rule conflicts can be diagnosed by checking the system logs

