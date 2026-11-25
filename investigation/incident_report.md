SSH Authentication Investigation Report

Investigation Overview

I analyzed SSH authentication logs in Splunk to identify unusual login activity and investigate potentially suspicious behavior.

Investigation Details

Log Source: SSH authentication dataset
Platform: Splunk Enterprise
Dataset: 6,000 events
Event Types: Authentication success, authentication failure, timeout, connection events, and session events.

Analysis Performed

I reviewed SSH events, compared successful and failed authentication attempts, examined source IP addresses, identified frequently targeted servers and usernames, and checked for repeated authentication failures within 5-minute time intervals.

I also created a Splunk dashboard containing 9 panels to visualize SSH activity and make the investigation easier.

Findings

The investigation highlighted source IP addresses with unusually high volumes of SSH activity. I examined the authentication events, timestamps, destination IPs, and usernames associated with the observed activity to identify patterns that required further investigation.

Repeated authentication failures were treated as suspicious indicators requiring further investigation, rather than proof of a confirmed attack.

Conclusion

The analysis helped identify unusual SSH authentication patterns and demonstrated how Splunk can be used to monitor, analyze, and investigate SSH login activity. Additional evidence, including server context and validation of successful sessions, would be required to confirm unauthorized access.

This investigation was conducted using a synthetic dataset for educational purposes.