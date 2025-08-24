# 🛡️ Azure Honeypot SOC Project


---

## Introduction  
In this project, I built a **basic home SOC in Microsoft Azure** from scratch. Using a free Azure subscription, I deployed a **Windows VM honeypot**, exposed it to the internet, and ingested its logs into **Azure Log Analytics Workspace**. I then integrated **Microsoft Sentinel** to analyze real-world attack traffic and visualize malicious activity.  

This project demonstrates **log analysis, threat detection, and SOC operations** in a real-world cloud environment.  

---

## Project Steps  

### 1. Azure Resource Setup  
- Created a Windows Virtual Machine (honeypot).  
- Configured networking to allow inbound RDP traffic, exposing the VM to attackers.  

**Resource Group Overview**  
![Azure Resource Group Overview](./5dc376ff-caf3-4be9-815c-b7156f73b8f1.png)  

---

### 2. Log Analytics Workspace (LAW)  
- Centralized all log data into LAW.  
- Connected the VM’s security logs for collection and monitoring.  

---

### 3. Microsoft Sentinel Integration  
- Linked Sentinel with LAW.  
- Built detection rules for failed login attempts.  
- Queried logs with **KQL (Kusto Query Language)**.  

---

### 4. Attack Analysis & Visualization  
- Queried failed RDP logins targeting the honeypot.  
- Identified IP sources and geolocations.  
- Built a **Sentinel attack map** to visualize attacker origins in real-time.  

**Attack Map (Microsoft Sentinel)**  
![Attack Map in Sentinel](./8100f694-5514-4a8d-8f95-d5e0b0ce528c.png)  

---

## Key Findings  
- Exposed systems are **immediately targeted** by brute-force attacks.  
- Sentinel provides **real-time visibility** into malicious activity.  
- KQL queries are critical for filtering and investigating security events.  
- Hardening measures (firewalls, NSGs, IP restrictions) drastically reduce alerts.  

---

## Skills Gained  
- 🔹 Configuring **Azure + Microsoft Sentinel** for SOC monitoring  
- 🔹 Centralizing logs with **Log Analytics Workspace**  
- 🔹 Writing and executing **KQL queries**  
- 🔹 Building attack maps and threat visualizations  
- 🔹 Applying **defensive security controls** in Azure  

---

## Conclusion  
This lab provided hands-on SOC experience in a cloud environment. By intentionally exposing a honeypot VM, I was able to capture **real attacker traffic**, investigate it using Sentinel, and validate the effectiveness of **security hardening techniques**.  

This project highlights practical skills in:  
- **Threat detection**  
- **Log analysis**  
- **SOC monitoring workflows**  
- **Cloud security engineering**  

---

## 
---

## 🔗 References  
- [Cyber Home Lab from ZERO and Catch Attackers! Free, Easy, and REAL (Microsoft Sentinel 2025)](https://www.youtube.com/watch?v=g5JL2RIbThM)
- [Microsoft Sentinel Documentation](https://learn.microsoft.com/en-us/azure/sentinel/)  
- [KQL Query Language](https://learn.microsoft.com/en-us/azure/data-explorer/kusto/query/)  
- [Azure Log Analytics](https://learn.microsoft.com/en-us/azure/azure-monitor/logs/log-analytics-tutorial)  

---

