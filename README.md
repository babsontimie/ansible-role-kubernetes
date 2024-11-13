Ansible Role: Kubernetes.multi
=========

Ansible role to install and configure kubernetes cluster on 
RedHat/Debian based systems.
Intended only for dev and testing purposes.

Requirements
------------

Role Variables
--------------

```yaml
```


Example Playbook
----------------

```yaml
---
- name: Install kubernetes
  hosts: all
  become: true
  roles:
    - Talhajuikar.kubernetes.multi
```

License
-------

BSD

Author Information
------------------

For more information, visit [talhajuikar.cloud](https://talhajuikar.cloud).
