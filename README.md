Role Name
=========

This Ansible role installs the necessary components on Red Hat to allow X11 forwarding. 

Requirements
------------

Access to repository to installing packages.
Open ports for X11 communication on your firewalls.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

---
- name: Install X11
  hosts: all
  become: yes
  roles:
    - ~/ansible_roles/inst-x11

License
-------

MIT

Author Information
------------------

Just a *nix admin trying to save a little time with some Automation.

# inst-x11
