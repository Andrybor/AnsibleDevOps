# AnsibleDevOps
Contain playbook that install nginx service on web machine and postgresql on db and deploy single html page with linked css styles.
Production folder contains buid and prod services that deploying java application on Tomcat.
For testing you need 3 linux remote machines that connected and configured with each other by ssh.
After adding configuration to Ansible config file you need to enter this command ansible-playbook build.yaml and go to ip of remote machine "..."/hello-world-war.
Don't forget to open 8080 port on machine where tomcat deployed.

Version[2] [Updated] Added roles :
 1. Builder  - build java application from dockerfile
 2. Deployer - deploy war on tomcat

Hosts need be configured in hosts ansible files.
To run -> ansible-playbook roles.yml
