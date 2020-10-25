# AWS-Cloud-Formation-Linux-Setup-Script

This is a cloud formation script to perform a complete Linux server setup for website hosting.

The script performs the following tasks.
* Add a key-value pair to login into EC2 instance with SSH keypair.
* Add USF CIDR block so that only user from USF can log in to EC2 instance
* Match the AMI according to the current region.
* Perform Nginx web server installation and setup index.html for the website with appropriate access permission.
* Fetch public DNS name from instance metadata and embedded into index.html files
* Display DNS name and IP address on output stack.
