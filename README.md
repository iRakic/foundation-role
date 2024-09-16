Foundation role
===============

This Ansible role sets common settings on systems like timezone and hostname. It helps standardize foundational configurations across your infrastructure.

Installation
============
To use this role, add it to your requirements.yml:
```yaml
- src: https://github.com/iRakic/foundation-role
  name: irakic.foundation
```
Then install it with:
```shell
ansible-galaxy install -r requirements.yml
```

Requirements
------------

There is no additonal dependency for this role.

Role Variables
--------------

* hostname
* timezone 
  

Dependencies
------------

There is no additonal dependencies for this role.

Example Playbook
================
Here's how to use the role in your playbook:

```yaml
- hosts: servers
  become: yes
  vars:
    hostname: "myserver.example.com"
    timezone: "Europe/Belgrade"
  roles:
    - role: irakic.foundation
```

License
-------

BSD