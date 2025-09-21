Role Name
=========

This Ansible role installs the necessary components on Red Hat to allow X11 forwarding. 

Requirements
------------

Access to repository for installing packages.
Open ports for X11 communication on your firewalls.

Role Variables
--------------

I used tags to provide an install and remove functionality. Quite frequently I need to temporarily setup X11 for the Oracle DBAs so that they can install Oracle or some Oracle product. This role makes it easy to install and remove the X11 components.

I did put "- never" on all of the tasks so that we can't accidentally modify a server. If you leave off the 'install' or 'remove' tag, the role won't make any changes to the server.

Tags:
 install
 remove
 never

To-Do
-----
Add Ubuntu and other Linux variants to the X11 installer.  My immediate need is for Red Hat, so I had to focus on that.

Dependencies
------------

None.

Example Playbook
----------------

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
