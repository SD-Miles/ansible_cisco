Cisco Access Switch
=========

This role applies configuration items common to all Cisco access switches--most especially, the VLANs. The main task file determines which VLANs are configured at which sites. The tasks will OVERWRITE any existing configuration, so proceed with caution and make sure you have good config backups. DHCP snooping is also included in this role.

Since Cisco IOS doesn't have a robust ACL commend or remark function, all list items are commented in the `define_acls.yml` task. You MUST comment all changes to maintain current documentation.

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
  - ansible_user.
I also assume SSH key authentication is enforced.

Dependencies
------------

Module depencies are listed under "requirements." There are no role dependencies configured, but it assumes that all switches already conform to the configurations in the following roles:
  - global
  - global-switch

Example Playbook
----------------

Since there are no variable or templates within the role, invocation is as simple as running it against an inventory, like so:

    - hosts: switches
      roles:
        - access-switch

License
-------

BSD

Author Information
------------------

Written by Steven Miles.
