# Ansible role: letsencrypt
Install free and trusted SSL/TLS certificates from Let's Encrypt.

## Requirements
None.

## Role Variables
|Key|Type|Description|Default|
|:--|:---|:----------|:------|
|letsencrypt_domain|String|Domain name.||
|letsencrypt_contact|String|e-mail address.||
|letsencrypt_webservice_type|String|nginx or apache|nginx|

## Dependencies
None.

## Example playbook

```yaml
- hosts: all
  roles:
    - { role: letsencrypt }
  vars:
    letsencrypt_domain: "example.com"
    letsencrypt_contact: "admin@example.com"
```
