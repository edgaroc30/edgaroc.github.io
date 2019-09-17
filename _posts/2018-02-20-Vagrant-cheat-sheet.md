A couple of useful commands when using Vagrant


```bash

# Destroys a machine completly 
vagrant destroy [name]

# Starts a machine
vagrant up

# Initialize a machine
vagrant init 

# Displays all the running boxes
vagrant global-status 

# Runs the provision file for that machine
vagrant provision

# Prunes all the zombie Virtual machines (When there are no running machines in virtualbox but one stills shows up)
vagrant global-status --prune 

# Updates the boxes
vagrant box update

# Simple way to copy a single file from VM to host
vagrant ssh -c "sudo cat /path/to/file/file" > file
  -Example:
vagrant ssh -c "sudo cat /srv/apache/conf/extra/httpd-vhosts.conf" > httpd-vhosts.conf

# Using vagrant-scp plugin
vagrant scp <some_local_file_or_dir> [vm_name]:<somewhere_on_the_vm>
  - Example:
vagrant scp default:/srv/apache/conf apache

# Install Vagrant plugin

vagrant plugin install name-of-the-plugin

```
