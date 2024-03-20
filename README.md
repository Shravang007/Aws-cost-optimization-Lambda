# Aws-cost-optimization-Lambda

AWS Cloud Cost Optimization - Identifying Stale Resources:-

Identifying Stale EBS Snapshots
In this project, we'll create a Lambda function that identifies EBS snapshots that are no longer associated with any active EC2 instance and deletes them to save on storage costs.

Description:
The Lambda function fetches all EBS snapshots owned by the same account ('self') and also retrieves a list of active EC2 instances (running and stopped). For each snapshot, it checks if the associated volume (if exists) is not associated with any active instance. If it finds a stale snapshot, it deletes it, effectively optimizing storage costs.

Steps Involved in this Project:

1. Create an EC2 instance with EBS Volume
2. Create a Snapshot and attach it with Volume,
3. Create a Lambda_Function that checks the EC2,
4. Configure Lambda Function with appropriate IAM Role and Policies to perform the task 
5. Deploy Lambda function and test it with Python Boto3 code which is perform get the details of EC2 and perform deletion task if snapshot not associate with EC2

   
