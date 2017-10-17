[![Build Status](https://img.shields.io/travis/quocvu/nodejs-ansible.svg)](https://travis-ci.org/quocvu/nodejs-ansible)
[![Ansible Role](https://img.shields.io/ansible/role/19878.svg)](https://galaxy.ansible.com/quocvu/nodejs-ansible)

nodejs-ansible
==============

Setup NVM, NodeJS, and NPM for development purpose. NVM allow developers to
run multiple version of NodeJS on the same computer.

Requirements
------------

Ansible and an internet connection

Role Variables
--------------

* `nvm_version` is the version of the NVM installer. Check <https://github.com/creationix/nvm> for the most recent version.
* `node_versions` is the list of node versions to install via NVM. We recommend installing at least one stable version.
* `npm_global_packages` is the list of the NPM packages to be installed globally

Dependencies
------------

none

Example Playbook
----------------

To install NodeJS development environment, add the following in your playbook:

```
- hosts: servers
  roles:
    - { role: quocvu.nodejs-ansible }
```

License
-------

MIT

Author Information
------------------

Quoc Vu  
https://github.com/quocvu
https://linkedin.com/in/quocvu  
