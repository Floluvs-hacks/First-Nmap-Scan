# First-Nmap-Scan
# My First Nmap Scan: Exploring the Basics of Network Enumeration

One of the most exciting milestones in my cybersecurity learning journey was running my first **Nmap (Network Mapper)** scan. It wasn’t just about typing commands into a terminal,it was about unlocking visibility into networks, devices, and services. This hands on experience gave me a solid foundation in network enumeration and reconnaissance; two essential pillars of ethical hacking.

##  What is Nmap?

Nmap is a powerful open-source tool used for network discovery and security auditing. With Nmap, you can:

>Discover active hosts on a network
>Identify open ports
>Detect services and their versions
>Perform OS fingerprinting
>Audit network security configurations

It’s widely used by system administrators and cybersecurity professionals to map out networks and spot vulnerabilities before attackers do.

##  Step 1: Simple Ping Scan
My first command was a basic **ping sweep** to find live hosts:
bash
nmap -sn 192.168.1.0/24
**This scan helped identify which devices were currently active on my local network, a crucial first step in any network enumeration process.**

## Step 2: Basic Port Scan
Next, I performed a basic TCP scan on one of the discovered hosts:
bash
nmap 192.168.1.1
**This showed me which ports were open. For example, port 80 (HTTP) or 22 (SSH). Open ports indicate running services, and knowing this helps assess what’s exposed to the network.**

## Step 3: Service and Version Detection
To learn more about what was running behind those ports, I used:
bash
nmap -sV 192.168.1.1
**This command revealed detailed information such as the software and version behind each open port (e.g., Apache 2.4.41), allowing me to evaluate potential vulnerabilities based on known issues with specific versions.**

**My Final thoughts?**
Understanding Nmap’s output is as important as running the scan itself and also Enumeration is the foundation of both offensive and defensive cybersecurity.

