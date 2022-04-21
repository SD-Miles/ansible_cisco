Cisco Global
=========

This role applies most of the configuration items common to all Cisco network switches and routers in the organization, provided they are running supported versions of IOS or IOS-XE.

Requirements
------------

Requires this module from Ansible Galaxy:  cisco.ios

Role Variables
--------------

No variables are stored in the role itself, but it assumes the following variables from the inventory file:
  - ansible_connection
  - ansible_network_os
  - ansible_become
  - ansible_become_method
  - ansible_user

Dependencies
------------

Module depencies are listed under "requirements." There are no role dependencies.

Example Playbook
----------------

Since there are no variable or templates within the role, invocation is as simple as running it against an inventory, like so:

    - hosts: all
      roles:
        - global

License
-------

BSD

Author Information
------------------

Written by Steven Miles.