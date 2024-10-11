# Elastic SIEM Lab Project

## Overview
In this project, I set up an Elastic SIEM environment using Elastic Cloud and a Kali Linux VM. The goal was to forward security event logs from the Kali machine to Elastic and monitor them through Kibana's dashboards. I also used Elastic Defend to enhance monitoring and added custom dashboards for visualization. This lab provided hands-on experience in using Elastic SIEM for security monitoring and incident response.

## Objectives
- Set up an Elastic Cloud SIEM instance.
- Install and configure Elastic Agent (Elastic Defend) on a Kali Linux VM to collect logs.
- Generate security events on the Kali VM using tools like Nmap.
- Query and analyze logs in Elastic SIEM.
- Create visual dashboards and set up security alerts.

## Lab Environment
- **Operating System**: Kali Linux (via VirtualBox)
- **Elastic Stack Version**: Elastic Cloud with Elastic Defend integration
- **Tools Used**: Elastic Agent (Elastic Defend), Kibana dashboards, Nmap

## Setup and Configuration

### 1. Elastic Cloud Setup
- Created a free Elastic Cloud account and deployed Elasticsearch and Kibana.
- Configured Elastic Cloud for security event monitoring.

![Virtual Box Setup](https://github.com/MegaByteKnight/Elastic-SIEM-Lab-Project/blob/main/images/Virtualbox%20Kali.jpg)

### 2. Kali Linux VM Setup
- Set up Kali Linux in VirtualBox, verified network connectivity, and updated the system.

### 3. Elastic Agent (Elastic Defend) Configuration
- Installed Elastic Agent on the Kali VM for log collection.
- Verified that logs were forwarded to Elastic SIEM in real-time.

![Kali Elastic Defend Install](https://github.com/MegaByteKnight/Elastic-SIEM-Lab-Project/blob/main/images/Kali%20elastic%20defend%20install.jpg)

### 4. Generating Security Events
- Used Nmap to simulate network scans and generate log data.
- Executed multiple Nmap scans to detect open ports and services.

![ip and sudo nmap](https://github.com/MegaByteKnight/Elastic-SIEM-Lab-Project/blob/main/images/nmap.jpg)

### 5. Monitoring with Kibana
- Created custom dashboards in Kibana to visualize system logs and Nmap scan data.
- Set up visualizations for login attempts, network activity, and system performance.

![Standard Dashboard](https://github.com/MegaByteKnight/Elastic-SIEM-Lab-Project/blob/main/images/Custom%20Dashboard1.jpg)
![Custom Dashboard for rules](https://github.com/MegaByteKnight/Elastic-SIEM-Lab-Project/blob/main/images/Custom%20Dashboard2.jpg)

### 6. Creating Alerts
- Configured Kibana to trigger alerts based on specific security events (e.g., Nmap scans, sudo commands).
- Set up email notifications for alerts triggered by suspicious activity.

![Rule creation in Elastic](https://github.com/MegaByteKnight/Elastic-SIEM-Lab-Project/blob/main/images/Elastic%20Rule%20creation.jpg)

## Challenges Faced
- Configuring the Elastic Agent to communicate with Elastic Cloud.
- Handling delays in event logs appearing on the Elastic console.

## Lessons Learned
- Practical experience setting up Elastic SIEM and Elastic Defend.
- Creating meaningful security dashboards using Kibana.
- Gained an understanding of Elastic’s alerting capabilities for incident detection.

## Future Enhancements
- Implement more advanced detection rules for specific attack vectors.
- Integrate logs from other sources like Windows event logs.
- Automate responses to specific alerts using Elastic's action framework.

## References
- Elastic Stack Official Documentation
- Elastic Defend Guide
- Nmap Documentation

## Conclusion
Completing this lab deepened my understanding of real-time security monitoring using Elastic Defend and Kibana. This hands-on project enhanced my ability to create dashboards, analyze logs, and configure security alerts in a real-world SIEM environment.
