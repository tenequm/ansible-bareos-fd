Ansible Role: Bareos-fd
=========

A role for Bareos file daemon installation on Debian 8 systems.


Role Variables
--------------
Define Bareos Filedaemon client name:

    fd_client_name: client-fd
Define Bareos director name:
    
    fd_dir_name: bareos-dir
Define password that corresponds the one on Director side config:

    fd_dir_pass: secret
Define if Xtrabackup plugin should be installed (Default: true):

    fd_add_xtrabackup_plugin: true

Decide if custom configuration files should be added (Default: false):

    fd_add_config: false

Define Bareos Filedaemon plugins directory (Default: /usr/lib/bareos/plugins):

    fd_plugins_dir: ""

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: tenequm.bareos-fd }

License
-------

MIT

Author Information
------------------

This role was created in 2017 by [Mykhaylo Kolesnik](http://github.com/tenequm).
