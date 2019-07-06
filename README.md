# ansible-role-server-yum-check-update

Ansible role to check for linux package updates.  

## Distros tested

* CentOS & RHEL 7.x

## Default Settings

* **debug_enabled_default**: true|false (default false)
* **server_yum_check_managed**: true

## Example Playbook server-yum-check-update.yml

Below example playbook will check for OS updates.

```yaml
---
- hosts: '{{inventory}}'
  become: yes
  roles:
  - server-yum-check-update
```

## Usage

```bash
ansible-playbook server-yum-check-update.yml --extra-vars "inventory=all-dev" -i hosts-dev
```
