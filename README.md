# ansible_linux
Ansible Linux Playground

This should be a playground for ansible. Ideally it should help to setup and streamline my local ubuntu setup in a quick and easy way.

Guides to follow:

- <https://docs.ansible.com/ansible/latest/installation_guide/index.html>

## Getting started

If you have followed the installation guide and setup ansible correctly you should run following command:

```bash
# via ansible-playbook
ansible-playbook --connection=local local.yaml
ansible-playbook -i inventory.yaml --connection=local local.yaml --ask-become-pass
# with ansible
ansible desktop -m ping -i inventory.yaml --connection=local
```
