# Jabber Playbook

This [Ansible Playbook](http://docs.ansible.com) installs and configures the
prosody jabber server on a Centos 6 machine.  

## Introduction
This playbook should be seen as a guide to setting up an own secure jabber
server.

### Target Auditory
Users with some basic knowledge of managing Linux systems

### Purpose of this project
We want to promote standardized, free and open source communication platforms
to be hosted by anyone.

## Requirements

- You should have a machine with a fresh Centos (6.5) installation, root access
  and functioning ssh public key authentification (see `ssh-copy-id`).

- You should have `ansible` installed via your distributions package manager.

### Debian/Ubuntu/...
```bash
aptitude install ansible
```

### Fedora 
```bash
yum install ansible
```

## How to use it
Checkout this project and it's submodules:
```bash
git clone https://github.com/xsrc/jabber xsrc-jabber-playbook
cd xsrc-jabber-playbook
git submodule update --init
```
Wdit the host file in the root directory and execute:

```bash
ansible-playbook -i hosts main.yml
```

## Author
Bahtiar `kalkin` Gadimov
