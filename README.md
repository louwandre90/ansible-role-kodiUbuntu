ansible-role-kodiUbuntu
=========
[![Travis](https://img.shields.io/travis/louwandre90/ansible-role-kodiUbuntu.svg?style=flat-square)](https://travis-ci.org/louwandre90/ansible-role-kodiUbuntu.svg?branch=master)
[![Ansible Role](https://img.shields.io/badge/role-louwandre90.kodiUbuntu-blue.svg?style=flat-square)](https://galaxy.ansible.com/louwandre90/kodiUbuntu/)

This role installs Kodi v16 on Ubuntu.

Installation is done via apt and some basic configuration is done after installation. 

Requirements
------------
Configuration is done according to a specific directory structure setup by the following role: 

    louwandre90.mediaDirs

Role Variables
--------------

The following defaults are set:

    username: jarvis

To pass different variables:

    ansible-playbook playbook.yml --extra-vars="username=myuser"
    
Dependencies
------------
This role depends on:

    louwandre90.mediaDirs

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: louwandre90.kodiUbuntu }

License
-------

BSD

Author Information
------------------

This role was created in 2016 by Andre Louw.
