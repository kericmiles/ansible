rtt.onboarding
=========

Sets up automation account and preps machine for Ansible automation

Requirements
------------

Ubuntu 16.04

Role Variables
--------------

- ansible_password
  <br>Hashed password, currently set to "RTT@Ansible", use mkpasswd --method=SHA-512 to generate new password hash

Dependencies
------------

- None

Example Playbook
----------------
    - hosts: linux
      roles:
        - {role: rtt.onboarding, ansible_password: <passwordHash>}

License
-------

BSD

Author Information
------------------

Author: Keric Miles
