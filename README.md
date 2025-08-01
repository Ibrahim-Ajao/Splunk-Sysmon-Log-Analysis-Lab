# Splunk-Sysmon-Log-Analysis-Lab


This project simulates the work of a SOC Analyst by using Windows Sysmon to generate logs and Splunk to analyze them. It's designed as a beginner-friendly hands-on project that builds core cybersecurity skills in threat detection, log analysis, and SIEM alerting.

---

## 📌 Objectives

- Learn to install and configure **Splunk** on a Windows VM
- Deploy **Sysmon** to collect detailed system logs
- Forward logs to Splunk and analyze them using queries
- Create alerts and dashboards to detect suspicious behavior

---

## 💻 Tools Used

| Tool      | Purpose                        |
|-----------|--------------------------------|
| Splunk    | SIEM/log analysis platform     |
| Sysmon    | Detailed system activity logs  |
| Windows 10| Virtual machine lab environment|
| PowerShell| Log simulation                 |
| MITRE ATT&CK| Threat behavior mapping      |

---

## 📁 Folder Contents

| Folder         | Description                            |
|----------------|----------------------------------------|
| `setup/`       | Installation & configuration guides    |
| `analysis/`    | Detection queries, alerts, dashboards  |
| `reports/`     | Sample log analysis report             |
| `screenshots/` | Evidence of work (UI, logs, dashboards)|
| `resources/`   | Sysmon config, reference links         |

---

## 🔄 Workflow Overview

1. Set up a Windows VM (VirtualBox/VMware)
2. Install Splunk Enterprise (Free trial)
3. Install Sysmon + config file
4. Configure Splunk to ingest Sysmon logs
5. Analyze logs using Splunk queries
6. Build dashboards & configure alerts
7. Document your findings

---

## 🕵️ Sample Detection Use Cases

| Use Case                    | Splunk Query Example |
|-----------------------------|----------------------|
| PowerShell encoded command  | `index=sysmon CommandLine="*enc*"` |
| Process Creation (Event 1)  | `index=sysmon EventCode=1` |
| Rare Parent-Child Process   | `index=sysmon Image="*cmd.exe" ParentImage!="explorer.exe"` |

---

## 📸 Screenshots

Include screenshots showing:
- Sysmon Event Logs
- Splunk Search Results
- Created Alerts
- Dashboards (e.g., Top Processes)

---

## 📄 Sample Report Included

Under `/reports`, you’ll find:
- A sample log analysis report
- Attack scenario explanation
- Detection steps and conclusion

---

## 📚 Learning Outcomes

By completing this lab, you will:
- Understand endpoint telemetry using Sysmon
- Learn SIEM ingestion and search logic
- Detect common attack patterns using logs
- Practice incident triage in a simulated setup

---

## 📎 Useful Links

- [Splunk Downloads](https://www.splunk.com/en_us/download.html)
- [Sysmon Documentation](https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon)
- [SwiftOnSecurity Sysmon Config](https://github.com/SwiftOnSecurity/sysmon-config)
- [MITRE ATT&CK Matrix](https://attack.mitre.org/)

---

## 👤 Author

**Ajao Ibrahim Adewale**  
Aspiring SOC Analyst | Google Cybersecurity Certificate Graduate  
📧 your.email@example.com  
🔗 [GitHub Portfolio](https://github.com/yourusername)

---

