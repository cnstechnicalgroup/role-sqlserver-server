Role: cnstechnicalgroup.sqlserver-server
========

Ansible role install SQL Server, SQL Server Agent

Requirements
------------

* CentOS7 
* Ubuntu Xenial Xenus

Role Variables
--------------

In the current version, you can specify the following variables:

| Name                  | Default |                                                              |
|-----------------------|---------|--------------------------------------------------------------|
| sa_password           |   ---   | system administrator password for SQL Server install .  |


Dependencies
------------

This package has no dependencies.


Requirements
------------

The target server must have at least 4GB of available RAM. 


License
-------

GPLv2

Author Information
------------------

Created by CNS Technical Group (https://www.cnstechgroup.com/)

Documentation
------------------

Install example (https://github.com/cnstechnicalgroup/ansible-sqlserver/blob/master/documents/sqlserver_role_install.md)

Examples
--------

```yaml
---
- name: cnstechnicalgroup.sqlserver-server role 
  hosts: dbservers
  sudo: yes
  roles: 
    - cnstechnicalgroup.sqlserver-server
  gather_facts: yes
  environment:
    SA_PASSWORD: "{{sa_password}}"
    ACCEPT_EULA: "Y"


```
