# OSUpdate.yml

Applies the OS updates for the host.  Once that is done, it reboots

To run the playbook, include this role in the top level playbook

```
- hosts: all
  become: true

  roles:
     - role:  OSUpdate

```