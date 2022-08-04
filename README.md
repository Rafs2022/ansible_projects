# ansible_projects

This is my Practice Ansible Automation Repo!

I am using a CentOS7 VM and an UBUNTU server VM
for all automated Ansible configurations.

Step 1:

Setup basic inventory file.

added ip addresses of both my VMs

Step 2:

Test connection to VMs

$ ansible all --key-file ~/.ssh/ansible -i inventory -m ping

- use the -u [username] (for remote connection)

Step 3:

Created ansible.cfg file to define inventory file, and private key location.

Now we can test connection to VMs with:

$ ansible all -m ping

Step 4:

Created 2 playbooks to Install and Remove apache packages on the Ubuntu Server.
