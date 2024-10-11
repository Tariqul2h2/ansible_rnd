# Ansible Playbook for Nginx Installation on ServerA 
This Ansible playbook installs `Nginx` on a server designated as `ServerA`, configures the firewall to allow `HTTP` traffic, and deploys a sample `index.html` file.

## Requirements
* Ansible installed on your control machine.
* Access to the target server (ServerA) with necessary privileges.
* Python and the required packages installed on the target server.

## Playbook Structure
The playbook consists of the following tasks:

### Installing Nginx
Uses the apt module to install the latest version of Nginx.

### Allowing HTTP Traffic
Configures firewalld to allow incoming traffic on port 80 (HTTP).

### Copying index.html
Copies a local index.html file to the default web root directory (/var/www/html/).


## Run the playbook

To run this playbook, use the following command:

### Syntax check
```
ansible-playbook installnginx.yaml --syntax-check
```

### Dry run
```
ansible-playbook installnginx.yaml -C
```
### Run the playbook
```
ansible-playbook installnginx.yaml
```
