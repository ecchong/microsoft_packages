microsoft_packages
=========

This role configure Microsoft repo and install Microsoft packages on RHEL. 

Requirements
------------

Role Variables
--------------
- microsoft_packages_repository_key: URL of Microsoft key
      Default: https://packages.microsoft.com/keys/microsoft.asc
- microsoft_packages_rhel_repo: URL of Microsoft RHEL repo
      Default: https://packages.microsoft.com/rhel/7/prod/
- microsoft_packages_list: List of packages to be installed.
      Default: undefined

Dependencies
------------

Example Playbook
----------------
  - name: install mssql-cli
    include_role:
      name: microsoft_packages
    vars:
      microsoft_packages_list:
      - mssql-cli

License
-------

BSD

Author Information
------------------

Eric Chong
- ecchong@gmail.com
- echong@redhat.com
