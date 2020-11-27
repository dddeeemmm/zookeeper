zookeeper
=========

    Install and config zookeeper ( standalone | cluster ) + sasl

Role Variables
--------------

    zookeeper_version: 3.6.2
    zookeeper_install: true
    
    zookeeper_time_tick:             2000
    zookeeper_limit_init:            10
    zookeeper_limit_sync:            5
    zookeeper_client_cnxns_max:      60
    zookeeper_autopurge_snap_retain: 3
    zookeeper_autopurge_interval:    1
    
    zookeeper_sasl: true
    
    zookeeper_admin_name:     admin
    zookeeper_admin_password: admin-secret

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: zookeeper }

License
-------

    MIT

Author Information
------------------

    Dmitrij Petrov
