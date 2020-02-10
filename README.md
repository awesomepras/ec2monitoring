# ec2monitoring
 # Purpose
Create Monitoring alert for instance to trigger alert to email on instance state changes
Create Monitoring Dashboard for the instance to show metrics on CPU Utilzation and DiskWriteBytes.
## Files
```
ec2monitor.yaml
```
This CFN will require following parameter:
* Stack Name
* instancename
* Source IP to allow connection
* SSH keypairname
* Subnet ID
* VPC
* Email address for notification

# Purpose
Create an instance usingi a keypair, with EIP and configure dashboard and monitoring for that instance


