# LAMP-Installation-Using-Ansible
This repository contains ansible playbook to automate the installation of LAMP(Linux,Apache, Mysql/MariaDB, PHP)
# overview 
This project uses Ansible to install the following:
- nginx
- apache
- MariaDB
- php
# Prerequisites
Before running the playbook script, you will need to have the following:
- control node 
- managed host(s)
- install git on control node
- install ansible on control node
# To get started:
Clone this repository to your control node:
```
git clone https://github.com/0xf2y/LAMP-Installation-Using-Ansible
```
Create hosts file 
```
touch inventories/hosts 
```
Put your managed hosts IP to `hosts` file

Run the following command to start installation:
``` 
ansible-playbook playbook.yaml -i inventories/hosts
```
To test installation:
```
curl <managed-host-IP>
```
