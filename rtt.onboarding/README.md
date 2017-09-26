rtt.onboarding
=========

Sets up automation account and preps machine for Ansible automation. The key can be replaced under files/id_rsa.pub.

Requirements
------------

Tested on Ubuntu 16.04 and Centos 7

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
Keric Miles
https://github.com/kericmiles/ansible
