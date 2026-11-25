SSH Log Analysis Using Splunk
About the Project
This project is a hands-on SOC investigation using Splunk to analyze SSH authentication logs. I created a sample dataset containing 6,000 SSH events and used Splunk to explore login activity, identify unusual patterns, and investigate potentially suspicious authentication behavior.

The main goal was to understand how a SOC analyst uses logs to identify suspicious activity instead of relying on predefined attack labels.
Tools Used
- Splunk Enterprise
- SPL (Search Processing Language)
- Windows
- JSON
Dataset
The dataset contains 6,000 SSH events, including successful logins, failed logins, authentication timeouts, connection events, and session activity.

The logs were ingested into Splunk and analyzed using different SPL queries.
Investigation
During this project, I worked on the following:
- Ingesting JSON logs into Splunk and validating extracted fields.
- Analyzing failed SSH login attempts by source IP.
- Identifying IP addresses generating high volumes of activity.
- Detecting repeated authentication failures within a 5-minute time window.
- Comparing failed and successful authentication activity.
- Investigating login patterns and suspicious source IPs.
- Building a dashboard to visualize SSH authentication activity.
Dashboard
I created a Splunk dashboard to make SSH activity easier to monitor and investigate.

Dashboard panels include:
- Total SSH Events
- Authentication Outcomes
- SSH Login Activity Over Time
- Top Source IPs
- Top Target Servers
- Top Targeted Usernames
- Repeated Authentication Failures
- Successful Login Details
- Recent SSH Events
What I Learned
While working on this project, I learned how to ingest logs into Splunk, write SPL queries, use statistical commands to analyze authentication activity, group events into time windows, and investigate suspicious patterns.

I also learned that repeated login failures alone do not confirm an attack. Authentication activity needs to be correlated with source IPs, targeted accounts, successful logins, timestamps, and other evidence before drawing a conclusion.
Project Purpose
This project was created for practical cybersecurity learning, with a focus on SOC Analyst skills, log analysis, detection, and investigation.

All logs used in this project are synthetic and intended for educational purposes only.