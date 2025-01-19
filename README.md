# AWS-Cloud-Cost-Optimization-identifying-Stale-Resources
Identifying Stale EBS Snapshots

In this, we'll create a Lambda function that identifies EBS snapshots that are no longer associated with any active EC2 instance and deletes them to save on storage costs.
The Lambda function fetches all EBS snapshots owned by the same account ('self') and also retrieves a list of active EC2 instances (running and stopped). For each snapshot, it checks if the associated volume (if exists) is not associated with any active instance. If it finds a stale snapshot, it deletes it, effectively optimizing storage costs.
# *Features-
- Snapshot Analysis: Identify snapshots that are no longer associated with active resources.
- Cost Insights: Calculate the potential cost savings of removing stale snapshots.
- Automation Support: Ready-to-use scripts for cleaning up unused snapshots.

