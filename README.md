[![CircleCI](https://circleci.com/gh/ansible-roles-mamono210/wp_cli/tree/main.svg?style=svg)](https://circleci.com/gh/ansible-roles-mamono210/wp_cli/tree/main)

Role Description
=========

Installs [WP-CLI](https://wp-cli.org) for CentOS7.

Requirements
------------

Before running this role, the following packages must be installed on the target system.

* Extra Packages for Enterprise Linux ([EPEL](https://docs.fedoraproject.org/en-US/epel/))
* [Remi's RPM repository](https://rpms.remirepo.net)
* [PHP](https://www.php.net)
* [Apache HTTP Server](https://httpd.apache.org)

Role Variables
--------------

None

Dependencies
------------

None

Example Playbook
----------------

```YAML
---
- hosts: all
  become: true
  roles:
    - geerlingguy.repo-epel
    - geerlingguy.repo-remi
    - mamono210.httpd_install
    - mamono210.php
    - wp_cli
```

License
-------

BSD
