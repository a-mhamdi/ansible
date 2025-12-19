# README #

## Overview

**Ansible** is an open-source automation tool that simplifies configuration management, application deployment, and task automation. 

## Installation

### Install Ansible on Ubuntu/Debian
```zsh
sudo apt update
sudo apt install ansible
```

### Check Ansible Version
```zsh
ansible --version
```

### Run Ad-hoc Commands
```zsh
ansible [host-pattern] -m [module] -a "[module options]"
```

```zsh
# Run a simple command on all hosts
ansible -i hosts.ini all -m command -a "uptime"
```

### Update Hosts
```zsh
ansible-playbook -i hosts.ini upd_usdge.yml -K
```

### Reboot Hosts
```zsh
ansible-playbook -i hosts.ini reboot_shutdown.yml --tags "reboot" -K
```

