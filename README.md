# multi_tier
#### This is for setting up a multi tier achitecture ie a webserver, a relational database, and a load balancer using ansible. In this demo i installed wordpress on multiple ec2 instances as webserver and used AWS RDS as a backend database for it and used Haproxy to balance the load between the webservers.
*Prerequisites*
1. You must have an AWS account
2. You must have an ec2 key configured
3. You must configure dynamic inventory for the ec2 instances

*Instructions*
1. Update roles/launch_ec2_rds/var/main.yml file
2. run the command ansible-playbook site.yml --private-key /path/to/key.pem
