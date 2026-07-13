# Splunk-Security-Lab
Security monitoring lab demonstrating log ingestion from a Metasploitable VM to a Splunk SIEM.

```mermaid
graph LR
A[Metasploitable VM] --> B[VirtualBox Network]
B --> C[Splunk Enterprise]
C --> D[Splunk Web Dashboard]
```

### Technical Challenges & Solutions
* **Network Connectivity:** Resolved communication barriers between the Host-Only network adapter and the VM's network interface by verifying IP configurations (`ip addr`).
* **Log Ingestion:** Troubleshooting `sourcetype` case sensitivity issues (`Linux:Syslog` vs `linux_syslog`) to ensure accurate log indexing.

### Core Competencies
* **SIEM Administration:** Managing log ingestion pipelines.
* **Network Troubleshooting:** Analyzing traffic flow between virtualized environments.
* **SPL (Splunk Processing Language):** Writing queries to filter and visualize logs (e.g., `sourcetype="Linux:Syslog" | timechart count`).
