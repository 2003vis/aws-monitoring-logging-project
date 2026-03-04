# aws-monitoring-logging-project
This project demonstrates real-time monitoring of an EC2 instance using CloudWatch alarms and automated email alerts using SNS. CloudTrail is enabled for logging AWS activities.

Architecture

Step 1 – Launch EC2 Instance
Created an Ubuntu EC2 instance and configured security groups.

Step 2 – Install Apache Web Server
Installed Apache and verified it using public IP.

Step 3 – Configure SNS Email Alert
Created SNS topic and email subscription for alert notifications.

Step 4 – Create CloudWatch Alarm
Configured CPUUtilization alarm with threshold > 36% and attached SNS topic.

Step 5 – Enable CloudTrail
Enabled CloudTrail to log all account activities.
