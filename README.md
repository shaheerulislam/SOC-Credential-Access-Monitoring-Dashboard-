SOC Credential Access Monitoring Dashboard (Splunk)

 Overview
This project is a Splunk-based Security Operations Centre (SOC) dashboard built to monitor Windows Security Event Logs. It focuses on credential access activity, user behaviour analysis, and system-level monitoring to support SOC investigation and triage workflows.
The dashboard simulates a real-world SOC environment where analysts detect and investigate authentication events using SPL queries and visual analytics.

 Key Features
Real-time Windows Security Event Log monitoring
Credential access activity tracking
User behaviour analysis using log parsing
Host and system-level activity visibility
Basic anomaly detection using event aggregation
SOC-style dashboard visualisation (charts, tables, single values)

Technologies Used
Splunk Enterprise
Windows Event Logs (Security Logs)
SPL (Search Processing Language)
Regex-based field extraction
Dashboard visualisation (Line charts, Bar charts, Tables, Single value)


Dashboard Components
Total Events Panel – Displays total security events
Event Trend Panel – Shows activity over time
User Activity Panel – Analyses user-level behaviour
Host Activity Panel – Displays system-level distribution
Anomaly Panel – Highlights high-frequency user activity


Key Learning Outcomes
Working with raw Windows Security logs in Splunk
Extracting fields using SPL and regex
Building SOC-style detection dashboards
Understanding authentication event analysis
Identifying limitations in unstructured log data


Limitations
No full CIM normalization applied
Some fields required manual extraction from raw logs
No advanced correlation rules or alerting configured
Dataset contains mixed structured and unstructured logs


Future Improvements
Add Splunk CIM data model integration
Implement brute-force detection (EventCode 4625)
Add alerting and automation rules
Integrate threat intelligence feeds
Enhance anomaly detection logic

Author
Shaheer Ul Islam
Cybersecurity / SOC Analyst Enthusiast
