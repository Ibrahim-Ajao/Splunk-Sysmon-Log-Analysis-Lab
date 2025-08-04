# Splunk-Sysmon-Log-Analysis-Lab

##  Objectives

- To install and configure **Splunk** on a Windows VM
- Deploy **Sysmon** to collect detailed system logs
- Forward logs to Splunk and analyze them using queries
- Create alerts and dashboards to detect suspicious behavior

---

##  Tools Used

| Tool      | Purpose                        |
|-----------|--------------------------------|
| Splunk    | SIEM/log analysis platform     |
| Sysmon    | Detailed system activity logs  |
| Windows 10| Virtual machine lab environment|
| PowerShell| Log simulation                 |
| MITRE ATT&CK| Threat behavior mapping      |

---

## steps

1. Set up a Windows VM using VirtualBox
2. Install Splunk Enterprise 
3. Install Sysmon + config file
4. Configure Splunk to ingest Sysmon logs
5. Analyze logs using Splunk queries
6. Build dashboards & configure alerts

---

##  Sample Detection Use Cases

| Use Case                    | Splunk Query Example |
|-----------------------------|----------------------|
| PowerShell encoded command  | index=endpoint CommandLine="*enc*" |
| Process Creation (Event 1)  | index=endpoint EventCode=1 |
| Rare Parent-Child Process   | index=endpoint Image="*cmd.exe" ParentImage!="explorer.exe" |

---
