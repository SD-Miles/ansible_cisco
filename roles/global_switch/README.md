Role Name
=========

This role applies the configuration items common to all Cisco switches, regardless of their position in the topology, provided they are running supported versions of IOS or IOS-XE.

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

Module depencies are listed under "requirements." There are no role dependencies configured, but it assumes that all switches already conform to the configuration in the following role:
  - global

Example Playbook
----------------

Since there are no variable or templates within the role, invocation is as simple as running it against an inventory, like so:

    - hosts: switches
      roles:
        - global_switch

License
-------

BSD

Author Information
------------------

Written by Steven Miles.