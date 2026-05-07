SOC Credential Access Monitoring Dashboard (Splunk)

Overview
This project is a Splunk-based Security Operations Centre (SOC) dashboard designed to monitor and analyse Windows Security Event Logs, with a focus on credential access activity, user behaviour, and system-level authentication patterns.
It simulates a real-world SOC environment where security analysts investigate authentication events, identify unusual user activity, and support incident triage using log-based detection techniques.


Objectives
Monitor Windows Security Event Logs in a SOC environment
Analyse credential access and authentication activity
Identify user behaviour patterns and anomalies
Visualise security events for SOC triage and investigation
Build practical detection logic using Splunk SPL queries


Technologies Used
Splunk Enterprise
Windows Security Event Logs (WinEventLog:Security)
SPL (Search Processing Language)
Regex-based field extraction
Dashboard visualisation (Single Value, Line Chart, Bar Chart, Tables)

Dashboard Structure
Panel 1 – Total Security Events
Provides a high-level overview of all ingested Windows Security events.

Panel 2 – Event Trend Analysis
Displays event activity over time to identify spikes or unusual patterns.

Panel 3 – User Activity Analysis
Extracts and analyses user accounts from authentication logs using regex-based parsing.

Panel 4 – System / Host Activity
Shows event distribution across hosts to support system-level monitoring.

Panel 5 – Anomaly / High Activity Detection
Highlights users with unusually high activity levels to support potential threat investigation.


SOC Use Case
This dashboard demonstrates how SOC analysts monitor Windows authentication activity to detect:
Credential access behaviour
User login patterns
System account activity (e.g., SYSTEM, service accounts)
Unusual spikes in authentication events
Early indicators of suspicious behaviour

Detection Logic Approach
Uses Splunk SPL to query Windows Security logs
Applies regex to extract user information from raw log data
Aggregates events to identify behavioural patterns
Uses time-based analysis for trend detection
Groups activity by user and host for investigation

Detection Coverage
Credential access monitoring
User authentication analysis
System-level activity tracking
High-frequency event detection
Basic anomaly identification based on event volume

Key Learning Outcomes
Working with raw Windows Security logs in Splunk
Extracting structured data from unstructured logs
Building SOC-style dashboards using SPL
Understanding authentication and logon event analysis
Identifying limitations of non-CIM normalised data

Limitations
No full CIM data model integration
Some fields require manual extraction from raw logs
No automated alerting configured
Dataset contains mixed structured/unstructured events

Future Improvements
Implement Splunk CIM data model for normalization
Add brute-force detection (EventCode 4625 monitoring)
Introduce alerting and correlation rules
Integrate threat intelligence feeds
Enhance anomaly detection logic with risk scoring

Author
Shaheer Ul Islam
SOC Analyst / Cybersecurity Enthusiast

Summary
This project demonstrates practical SOC monitoring capabilities using Splunk, focusing on credential access detection, user behaviour analysis, and security event visualisation to support incident response workflows.
