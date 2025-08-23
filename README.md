# Description

This is automation to setup https://github.com/rizface/uptime-monitoring in my local and vm

# Prerequisite
- Install Ansible
- SSH Private Key


# How To

## Run The Playbook
```shell
ansible-playbook -i inventory.ini --ask-vault-pass uptime.yml --limit uptime-host -e version=v0.0.4
```

## Create New Secret
```
ansible-vault create <filename.yml>
```

## Encrypt Existing Secret
```
ansible-vault encrypt <filename.yml>
```

## Decrypt Existing Secret
```
ansible-vault decrypt <filename.yml>
```