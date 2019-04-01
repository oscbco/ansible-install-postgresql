Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

postgresql_key: Repository key
postgresql_repository: Repository
postgresql_version: Version to install

Dependencies
------------


Example Playbook
----------------

    - hosts: servers
      roles:
      - {
          role: install-postgresql,
          postgresql_key: https://www.postgresql.org/media/keys/ACCC4CF8.asc,
          postgresql_repository: deb http://apt.postgresql.org/pub/repos/apt/ jessie-pgdg main,
          postgresql_version: postgresql-11.2
        }

License
-------

MIT

Author Information
------------------

oscbco.dev
