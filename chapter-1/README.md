
# Ansible for DevOps Chapter 1

This documentation is based on the Ansible for DevOps Series by Network Nuts

## Prerequisites:
1. 3 Ubuntu 22.04 Virtual Machines
2. Internet Connectivity on VMs
3. Basic Linux Knowledge 


## 1. Installing Ansible

Install Network Manager, Libvirt, Qemu

```bash
  sudo apt-add-repository ppa:ansible/ansible
  sudo apt update
  sudo apt install ansible
```

## 2. Create Inventory and Ansible Config

```bash
  ansible-config init -t all --disabled -f ini > ansible.cfg
```

## 3. Running the Playbook

```bash
  ansible-playbook playbook.yml -i inventory
```
