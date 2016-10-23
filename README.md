memcache
=========

[![Build Status](https://travis-ci.org/jebovic/ansible-memcache.svg?branch=master)](https://travis-ci.org/jebovic/ansible-memcache) [![Ansible Galaxy](https://img.shields.io/badge/galaxy-jebovic.memcache-blue.svg?style=flat)](https://galaxy.ansible.com/jebovic/memcache)

Install and configure memcache

Role Variables
--------------

```yaml
# Memcached basic configuration
memcache_log_file: /var/log/memcached.log
memcache_memory_size: 64
memcache_port: 11211
memcache_user: memcache
memcache_listen_address: 127.0.0.1
memcache_max_connections: 1024
```

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - { role: jebovic.memcache }
```

Tags
----

* memcache_config : only update config and restart service

License
-------

MIT

Author Information
------------------

Jérémy Baumgarth https://github.com/jebovic
