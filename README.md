## About me

As an Information Security professional and passionate technology enthusiast, I've built and maintain an advanced homelab infrastructure that serves as my personal playground for exploring cutting-edge technologies and honing my IT and security skills. My setup is designed with a focus on security, performance, flexibility, and high availability, leveraging a range of powerful tools and platforms.


## Homelab setup

My homelab journey is a continuous learning experience, pushing me to explore new technologies, overcome challenges, and develop a deep understanding of modern IT infrastructure. It's not just a hobby; it's a dynamic environment where I can experiment with enterprise-grade solutions, enhance my skills in areas ranging from network security to home automation, and stay at the forefront of technological advancements. 

The combination of high-speed networking, robust virtualization, advanced security measures, and automation tools allows me to create a homelab that rivals many professional setups, providing an invaluable platform for learning and innovation. Whether it's optimizing network performance, implementing new security protocols, or exploring the latest in home automation, my homelab is always evolving, reflecting my passion for technology and my commitment to continuous learning and improvement.

<p align="center">
<img src="https://github.com/user-attachments/assets/4c286a28-22a1-4796-8a36-5d4740cdb220" alt="Alt Text" width="400" height="400">
</p>


## Infrastructure and Virtualization

At the core of my homelab is Proxmox, a robust virtualization platform that allows me to efficiently manage multiple virtual machines and containers. This setup provides the flexibility to run various services while optimizing hardware resources. 


### Proxmox VMs
- OPNsense Firewall
- Cockpit Project (LXC) - Debian
- Cockpit Project (LXC) - Ubuntu
- Ubuntu DEV and PROD environments
- TrueNAS Core for hot storage
- Windows 11
- Windows 11 LTS
- Kali Linux
- HAOS


### Bare Metal Servers
- Truenas Core - Primary Backup
- Truenas Core - Secondary Backup


## Network Architecture

My network infrastructure is built on a high-speed 10GbE backbone, ensuring lightning-fast data transfer between servers and critical devices. This setup significantly reduces latency and improves overall system performance, especially for data-intensive tasks and storage operations.
To enhance security and network segmentation, I've implemented VLANs throughout my homelab. This allows me to isolate different types of traffic and create logical separations between various services, such as IoT devices, guest networks, and management interfaces.

## Network Security and Remote Access

Securing my network is paramount, which is why I've implemented OPNsense as my firewall solution. This open-source, FreeBSD-based firewall offers advanced features like intrusion detection, traffic shaping, and VPN capabilities. For secure remote access, I rely on WireGuard VPN, a modern and efficient protocol that allows me to safely connect to my homelab from anywhere in the world.
To further enhance my network security and improve browsing experience, I've deployed AdGuard Home. This powerful DNS sinkhole blocks ads and trackers at the network level, providing a cleaner and safer internet experience for all devices on my network.


## Security Monitoring and Password Management

I've integrated Wazuh, an open-source security monitoring solution, to provide real-time threat detection and response capabilities across my homelab infrastructure. For password management, I self-host Bitwarden, ensuring that my sensitive credentials are stored securely and easily accessible when needed.


## Containerization

To streamline deployment and configuration, I've embraced Docker containerization. Docker enables me to package and run applications in isolated environments, ensuring consistency and easy scalability. 


## Homelab Automation

Using Ansible allows me to define my infrastructure as code, facilitating quick deployments and maintaining consistency across my environment. 
n8n's ability to interact with APIs and databases makes it particularly useful for integrating different services within my homelab ecosystem. For instance, i have created automations that trigger actions based on events and set up notifications for important server and calendar events. 


## Home Automation

My homelab extends into home automation, where I use Home Assistant to integrate various smart devices and create custom automations. This central hub manages everything from lighting and climate control to energy monitoring, enhancing the comfort and efficiency of my living space.


## Backup Strategies and High Availability

Recognizing the importance of data protection, I've implemented a comprehensive backup strategy. This includes:
- Regular snapshots of critical VMs and containers
- Backup replication using rclone to encrypt and sync on a separate local server
- Offsite backups remote location

To ensure high availability for critical services, I've set up:
- Proxmox clusters with live migration capabilities
- Load balancing for web services using HAProxy
- Redundant storage with TrueNAS using ZFS RAID configurations
- Automated failover for network and key services


