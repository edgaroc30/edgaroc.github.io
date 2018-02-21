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
```
