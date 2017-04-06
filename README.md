Ansible role: Let's encrypt
=========

Install free and trusted SSL/TLS certificates from Let's Encrypt.

Requirements
------------

None.

Role Variables
--------------

    letsencrypt_domains: {}

Dependencies
------------

+ shomatan.repo-epel

Example Playbook
----------------

    - hosts: servers
      roles:
        - role: shomatan.letsencrypt
          letsencrypt_domains:
            example.com:
              email: "admin@example.com"

License
-------

MIT

Author Information
------------------
