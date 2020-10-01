Role Name
=========

An ansible role to set up dy.fi dynamic DNS service updater

Requirements
------------

This is only for Finnish users.

users

Role Variables
--------------

The variables used in this role are described in the table below. There are no default values for them, because there are no sensible defaults available. 

| Name           | Description                        |
| -------------- | -----------------------------------|
| `dyfi_user` | Your dy.fi username |
| `dyfi_password` | Your dy.fi password |
| `dyfi_host` | Your dy.fi hostname for the host. Currently this role supports only one hostname per client |

Dependencies
------------

No dependencies

Example Playbook
----------------


    - hosts: server
      roles:
         - role: ansible-role-dyfi
      vars: 
         dyfi_user: <your_dyfi_username>
         dyfi_password: <your_dyfi_password>
         dyfi_hostname: <your_dyfi_hostname>
         

License
-------

BSD

Author Information
------------------

Toni Martikainen
