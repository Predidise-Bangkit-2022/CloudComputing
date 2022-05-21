Go to cloud.google.com

Go to my Console

Choose your Project

Choose Networking > VPC network

Choose "Firewall"

Choose "Create Firewall Rule"

To apply the rule to select VM instances, select Targets > "Specified target tags", and enter into "Target tags" the name of the tag. This tag will be used to apply the new firewall rule onto whichever instance you'd like. Then, make sure the instances have the network tag applied.

Set Source IP ranges to allow traffic from all IPs: 0.0.0.0/0

To allow incoming TCP connections to port (for example:9090), in "Protocols and Ports", check “tcp” and enter 9090

Click Create (or click “Equivalent Command Line” to show the gcloud command to create the same rule)

reference: https://cloud.google.com/vpc/docs/using-firewalls
