# AWS-Resource-Tracker-Project-
AWS Resource Tracker
This project is an automated solution for tracking AWS resources. Built using a shell script, it integrates with a cron job for daily updates, providing detailed insights into AWS resources like Lambda functions, IAM users, S3 buckets, and EC2 instances.

Key Features:
Resource Tracking:

Lambda Functions: Lists all deployed Lambda functions and their configurations.
Command: aws lambda list-functions
IAM Users: Retrieves all IAM users to monitor access and roles.
Command: aws iam list-users
S3 Buckets: Lists all S3 buckets and displays storage usage and permissions.
Command: aws s3 ls
EC2 Instances: Lists EC2 instances and provides status, type, and region details.
Command: aws ec2 describe-instances
Automation:

A cron job schedules the script to run daily, ensuring real-time updates without manual intervention.
Insights and Usage:

Summarizes key metrics such as the total number of resources, their status, and configurations for better management.
Outputs results in a structured, easy-to-read format (e.g., JSON or plain text).
How to Use:

Clone the repository.
Configure AWS CLI with your credentials: aws configure.
Schedule the script using a cron job (crontab -e)
