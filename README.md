**AWS Cloud Cost Optimization - Identifying Stale Resources**
Identifying Stale EBS Snapshots
In this example, we'll create a Lambda function that identifies EBS snapshots that are no longer associated with any active EC2 instance and deletes them to save on storage costs.

**Description:**
The Lambda function fetches all EBS snapshots owned by the same account ('self') and also retrieves a list of active EC2 instances (running and stopped). For each snapshot, it checks if the associated volume (if exists) is not associated with any active instance. If it finds a stale snapshot, it deletes it, effectively optimizing storage costs.

**Important**
Add policy for snapshots function :
* Delete snapshots, describe snapshots
* Describevolumes, describeinstances

**Reference**
https://youtu.be/OKYJCHHSWb4?si=YB_mpL0rWsNC3FHA


**Shell scripting for jenkins upload jenkins in S3**
 configure:
 Add cli user and policy to access s3
 chmod 777 (file name)
 ./fimename
