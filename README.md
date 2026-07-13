# Splunk-Security-Lab
Security monitoring lab demonstrating log ingestion from a Metasploitable VM to a Splunk SIEM.

```mermaid
graph LR
A[Metasploitable VM] --> B[VirtualBox Network]
B --> C[Splunk Enterprise]
C --> D[Splunk Web Dashboard]
