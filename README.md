# ansible_linux

Ansible Linux Playground

This should be a playground for ansible. Ideally it should help to setup and streamline my local ubuntu setup in a quick and easy way.

Guides to follow and inspired by:

- <https://docs.ansible.com/ansible/latest/installation_guide/index.html>
- <https://github.com/LearnLinuxTV/ansible_course/tree/main>

## Getting started

If you have followed the installation guide and setup ansible correctly you should run following command:

```bash
# via ansible-playbook
ansible-playbook --connection=local local.yaml
ansible-playbook -i inventory.yaml --connection=local local.yaml --ask-become-pass
# with ansible
ansible workstation -m ping -i inventory.yaml --connection=local
```

## Installing a role from Galaxy (eg. kind)

You might find same usefull playbook in the galaxy. (see <https://docs.ansible.com/ansible/latest/galaxy/user_guide.html>).
To install it run following first:

```bash
# search for roles
ansible-galaxy role search kind
# for a single role
ansible-galaxy role install xanmanning.kind
# or via requirements file
ansible-galaxy role install -r requirements.yaml
```

## About testing ansible

If you step into the topic of testing ansible (what you really should do) you might read following topic about molecule:

- <https://www.goncharov.xyz/it/ansible-testing-en.html>
