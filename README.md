# Ansible role: letsencrypt
Install free and trusted SSL/TLS certificates from Let's Encrypt.

## Requirements
None.

## Role Variables
|Key|Type|Description|Default|
|:--|:---|:----------|:------|
|letsencrypt_domains|Dict|See below.|{}|
|letsencrypt_webservice_type|String|nginx or apache|nginx|

## Dependencies
None.

## Example playbook

```yaml
- hosts: all
  roles:
    - { role: letsencrypt }
  vars:
    letsencrypt_domains:
      example.com:
        email: "admin@example.com"
```
