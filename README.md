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
- Created a free Elastic Cloud account.
- Deployed Elasticsearch and Kibana on Elastic Cloud.
- Configured the deployment for security event monitoring.

### 2. Kali Linux VM Setup
- Set up Kali Linux in VirtualBox.
- Verified network connectivity and updated the system.

### 3. Elastic Agent (Elastic Defend) Configuration
- Installed Elastic Agent on the Kali VM to collect and forward logs.
- Verified the agent was running and forwarding data to Elastic SIEM.
- Monitored system logs and security events in real-time.

### 4. Generating Security Events
- Used Nmap to generate network scan logs, simulating common security events.
- Executed multiple Nmap scans to trigger alerts for open ports and services.

### 5. Monitoring with Kibana
- Created custom dashboards in Kibana to visualize system activity and Nmap scan logs.
- Set up visualizations for login attempts, network activity, and system performance.

### 6. Creating Alerts
- Configured alerts within Kibana to trigger based on security events, such as Nmap scans.
- Set up notifications for specific event triggers.

## Screenshots
Include screenshots of dashboards and alert configurations to showcase the lab setup.

- **Dashboard Overview**
<img a images/Custom Dashboard.jpg
- **Nmap Scan Visualization**

- **System Performance Monitoring**


## Challenges Faced
- Configuring the Elastic Agent on Kali Linux to communicate with Elastic Cloud.
- Monitoring delays in event logs appearing on the Elastic Cloud console.

## Lessons Learned
- Gained practical experience setting up and configuring Elastic SIEM.
- Learned how to visualize logs and create meaningful dashboards for security monitoring.
- Improved understanding of Elastic Defend and its capabilities for threat detection.

## Future Enhancements
- Experiment with more advanced detection rules in Kibana.
- Integrate additional data sources, such as Windows event logs.
- Automate responses to certain security alerts using Elastic's action framework.

## How to Reproduce This Lab

### Set Up the Environment
- Set up a Kali Linux VM in VirtualBox.
- Create an Elastic Cloud account and configure the SIEM environment.

### Install and Configure Elastic Agent
- Install Elastic Agent on the Kali VM.
- Ensure logs are being forwarded to the Elastic Cloud SIEM.

### Visualize and Monitor Data
- Use Kibana to create custom dashboards and set up security alerts.

## References
- Elastic Stack Official Documentation
- Elastic Defend Guide
- Nmap Documentation

## Conclusion
Completing this Elastic SIEM lab helped deepen my understanding of real-time security monitoring and incident detection. By working with Elastic Defend and Kibana, I learned how to create meaningful visualizations and alerts, which are essential for modern security operations.
