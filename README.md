# ansible-mysql-replicated
Ansible deployment of master-master replicated Mysql on Ubuntu 14.04

## Description

The is dual replication, writes to either server will be replicated to the other. 
Both sides are master and slave. 

## To create in vagrant:
Vagrant uses "hostmanager" plugin. Before running, install with: vagrant plugin install vagrant-hostmanager

`vagrant up`

Mysql service available at:

`mysql1.internal.tld:3306`

and

`mysql2.internal.tld:3306`

username: root pass: password

edit `inventory/group_vars/all.yml` to change passwords

