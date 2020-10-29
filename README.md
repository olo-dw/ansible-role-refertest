Ansible Role Refertest
======================

This Ansible role installs and configures Refertest (Official website: https://www.acpqualife.com/refertest).

Requirements
------------

* Java 8
* Mysql 5.7
* Tomcat 9

Role Variables
--------------

Mandatory:

* refertest_package_url: Package download URL
* refertest_license_key: 'LICENSE_KEY'
* refertest_owner_name: 'YourCompany'

Default:

```
refertest_db_host: 'localhost'
refertest_db_port: 3306
refertest_db_name: 'refertest'
refertest_db_user: 'Refertest_user'
refertest_db_password: 'Refertest'
refertest_server: 'localhost'
```

Example Playbook
----------------

```
    - hosts: servers
      roles:
         - role: ansible-role-refertest
```

License
-------

MIT

Author Information
------------------

This role was created in 2020 by Olivier Locard on the behalf of Deveryware.
