🚨 Incident Simulation: High CPU Usage
📸 CPU Spike Detected (Initial Condition)

High CPU utilization was intentionally generated using multiple background processes to simulate abnormal system activity such as cryptomining or denial-of-service behavior.

📸 CloudWatch Alarm Triggered (Detection)

AWS CloudWatch detected that CPU usage exceeded the defined threshold (70%) and triggered an alert, transitioning the alarm state from:

➡️ OK → ALARM

📸 Alert Notification Received (SNS Email)

An automated email alert was sent via Amazon SNS, demonstrating real-time notification and escalation capabilities used in Security Operations Centers (SOC).

📸 CPU Recovery After Mitigation (Response)

The abnormal activity was mitigated by terminating the resource-intensive processes:

pkill yes

CPU utilization returned to normal levels, indicating successful response.

📸 Alarm Returned to Normal (Recovery)

CloudWatch confirmed system recovery by transitioning the alarm state from:

➡️ ALARM → OK

🧠 Key SOC Skills Demonstrated
Monitoring cloud infrastructure using AWS CloudWatch
Configuring alert thresholds for anomaly detection
Detecting abnormal system behavior
Investigating system performance using Linux tools (top)
Executing incident response actions
Validating recovery through monitoring systems
🎯 Summary

This lab demonstrates a complete Security Operations Center (SOC) workflow:

➡️ Detection → Alerting → Investigation → Response → Recovery

Simulating and responding to abnormal system activity in a cloud environment reflects real-world cybersecurity operations and incident handling.
