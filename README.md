# ec2monitoring
 # Purpose
Create Monitoring alert for instance to trigger alert to PD and email on instance state
Create Monitoring Dashboard for the instance to show metrics on CPU Utilzation and DiskWriteBytes.
## Files
```
ec2monitor.yaml
```
This CFN will require following parameter:
* - Stack Name
* - instanceid

# Purpose
Create an instance usingi a keypair, with EIP and configure dashboard and monitoring for that instance

## Files
```
cfnTemplate.yaml
```
This CFN will require following parameter:
* - Stack Name
* - instancename
* - environment (dev or prod)

