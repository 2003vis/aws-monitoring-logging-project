# AWS Monitoring & Logging System

This project simulates a real-world cloud monitoring setup using AWS services.
An EC2 instance is monitored using CloudWatch alarms. When CPU utilization exceeds a defined threshold, an automated email notification is triggered via SNS. CloudTrail is enabled to log all account activities for auditing and security.

# Architecture Diagram
AWS Services Used

Amazon EC2 – Virtual Server

Amazon CloudWatch – Monitoring & Metrics

Amazon SNS – Email Notifications

AWS CloudTrail – Activity Logging

# Implementation Steps
EC2 Instance Setup

Launched Ubuntu EC2 instance (t2.micro)

Configured security groups (SSH & HTTP)

Installed Apache Web Server

SNS Email Configuration
Created SNS topic: CPU-Alert-Topic

Subscribed email endpoint

Confirmed email subscription

CloudWatch Alarm Setup

Selected EC2 → CPUUtilization metric

Set threshold: Greater than 36%

Attached SNS topic for notifications

# Troubleshooting Scenario
Checked CloudWatch metrics

Logged into EC2 via SSH

Used top command to identify high resource process

Terminated stress process

Verified CPU returned to normal
