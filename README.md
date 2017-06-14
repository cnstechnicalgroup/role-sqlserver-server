Role: role.sqlserver
========

Ansible role install SQL Server, SQL Server Agent

Requirements
------------

* CentOS7 

Role Variables
--------------

In the current version, you can specify the following variables:

| Name                  | Default |                                                              |
|-----------------------|---------|--------------------------------------------------------------|
| sa_password           |   ---   | system administrator password for SQL Server install .  |


Dependencies
------------

This package has no dependencies.

License
-------

GPLv2

Author Information
------------------

Created by CNS Technical Group (https://www.cnstechgroup.com/)

Examples
--------

```yaml
---
- name: role.sqlserver-server role 
  hosts: dbservers
  sudo: yes
  roles: 
  - cns.role-sqlserver-server
  gather_facts: no
  environment:
   SA_PASSWORD: "{{sa_password}}"

```
