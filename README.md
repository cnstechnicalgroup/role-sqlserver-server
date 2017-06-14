Role: role.sqlserver
========

This role installs and configures SQL Server, SQL Server Agent and Always-On Availability Groups ReadOnly Scaling.

Requirements
------------

CentOS7. 

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

Created by CNS Technical Group (https://www.cnstechnicalgroup.com)

Examples
--------

```yaml
---
- name: role.sqlserver-server role 
  hosts: all
  roles:
    - role.sqlserver-server
```
