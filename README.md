# Description

This is automation to setup https://github.com/rizface/uptime-monitoring in my local and vm

# Prerequisite
- Install Ansible
- SSH Private Key

# How To
```shell
ansible-playbook -i inventory.ini --ask-become-pass uptime.yml --limit uptime-host -e version=v0.0.4
```