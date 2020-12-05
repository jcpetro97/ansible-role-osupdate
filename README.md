# OSUpdate.yml

Applies the OS updates for the host.  Once that is done, it reboots

To run the playbook, include this role in the top level playbook

```
- hosts: all
  become: true

  roles:
     - role:  OSUpdate

```

**NOTE:** When you run this role inside a playbook, If you need to skip the update checks, do the following:

`ansible-playbook <playbook name>.yml -u <username> --extra-vars="Check=no"`