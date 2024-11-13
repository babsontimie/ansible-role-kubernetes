Ansible Role: Kubernetes.multi
=========

Ansible role to install and configure kubernetes cluster on 
RedHat/Debian based systems.
Intended only for dev and testing purposes.

Requirements
------------
This role is tested on the following OS:
- Rocky Linux 9
- CentOS 9 Stream
- Ubuntu 22.04 / 24.04 
- Debian 11 / 12


Role Variables
--------------
The following variables are used in this role:
The default values are set in `defaults/main.yml`.
```bash
kubernetes_version: "" # Default is 1.30
crio_version: "" # Default is 1.30
container_runtime: "" # Can be either containerd or crio. Default is crio. 
```
You can override these variables in your playbook.

```yaml
---
- name: Install kubernetes
  hosts: all
  become: true
  roles:
    - Talhajuikar.kubernetes.multi
  vars:
    container_runtime: "containerd"
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

MIT

Author Information
------------------

For more information, visit [talhajuikar.cloud](https://talhajuikar.cloud).
