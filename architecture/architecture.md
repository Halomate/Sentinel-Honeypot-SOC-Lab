# Lab Architecture

This lab simulates a simple cloud Security Operations Center environment using Microsoft Azure and Microsoft Sentinel.

Components used:

- Azure Virtual Machine (Windows honeypot)
- Azure Virtual Network
- Network Security Group
- Azure Monitoring Agent
- Log Analytics Workspace
- Microsoft Sentinel SIEM

Data Flow:

Internet  
↓  
Azure VM (Honeypot)  
↓  
Security Logs Generated  
↓  
Azure Monitoring Agent  
↓  
Log Analytics Workspace  
↓  
Microsoft Sentinel  

Security events from the VM are forwarded to Sentinel where they can be analyzed using KQL queries.
