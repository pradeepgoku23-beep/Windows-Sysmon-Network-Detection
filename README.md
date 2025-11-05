# Windows Sysmon Network Event Monitoring Lab

## 📌 Project Overview
This project focuses on monitoring **network events on a Windows system using Sysmon**.  
The objective is to detect suspicious outbound and inbound connections — an important skill for SOC Analysts.

This lab demonstrates:
- Installation & configuration of Sysmon
- Understanding Sysmon logs
- Detecting network activity using Sysmon (Event ID 3)
- Basic network threat analysis using Windows Event Viewer

---

## 🛠️ Tools & Environment
| Component | Details |
|---------|--------|
Windows VM | Windows 11 Virtual Machine
Event Logging | Sysmon (System Monitor)
Sysmon Config | Sysmon Modular config file
Attack Simulation | Nmap scanning
Log Review | Event Viewer (Windows Security + Sysmon Logs)

---

## 🎯 Learning Objectives
- Understand Sysmon logging and event IDs
- Detect network-based suspicious activity
- Identify process-to-network relationships
- Gain hands-on SOC monitoring skills

---

## 🚀 Steps Performed

### 1️⃣ Installed Sysmon
### 2️⃣ Verified Sysmon Installation
- Checked **Sysmon Event Logs**
- Confirmed logs under:  
`Applications and Services Logs → Microsoft → Windows → Sysmon → Operational`

### 3️⃣ Performed Network Activity Simulation
Executed:
- Basic **internet browsing**
- **Nmap scan** from Kali to Windows VM
- Verified Sysmon logs for network events

### 4️⃣ Monitored Sysmon Network Logs
Focused on **Event ID 3 – Network Connection**

Observed fields:
- Source IP / Port
- Destination IP / Port
- Process initiating connection
- Protocol used

---

## 📎 Evidence / Screenshots
| Screenshot | Description |
|-----------|-------------|
Event Viewer | Sysmon Network Event ID 3 logs
Nmap scan output | External scanning activity
Sysmon process & network logs | Connection logs evidence

*(Screenshots are available in the `screenshots/` folder)*

---

## ✅ Key Takeaways
- Sysmon provides deep visibility into system-level events
- **Event ID 3** is crucial for detecting lateral movement & C2 traffic
- Nmap scans are easily visible in Sysmon logs
- Useful for SOC monitoring and threat hunting tasks

---

## 📚 Future Enhancements
If needed later, can extend this project by:
- Sending Sysmon logs to Splunk
- Creating a Splunk threat-hunting dashboard

---

## 👨🏻‍💻 Project Status
✔ Completed (Sysmon + Event Viewer)  
🔜 Optional upgrade: Add Splunk monitoring

