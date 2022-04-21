Cisco Distribution Switch
=========

This role applies configuration items common to all Cisco distribution-level switches--most especially, the building ACLs, which are the same at each site. The tasks will OVERWRITE any existing configuration, so proceed with caution and make sure you have good config backups.

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

Module depencies are listed under "requirements." There are no role dependencies configured, but it assumes that all switches already conform to the configurations in the following roles:
  - global
  - global-switch
  - access-switch

Example Playbook
----------------

Since there are no variable or templates within the role, invocation is as simple as running it against an inventory, like so:

    - hosts: distro_switches
      roles:
        - distro-switch

License
-------

BSD

Author Information
------------------

Written by Steven Miles.