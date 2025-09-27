
[![Publish to Ansible Galaxy](https://github.com/ulrich-sun/ansible-roles-kubernetes/actions/workflows/publish.yaml/badge.svg)](https://github.com/ulrich-sun/ansible-roles-kubernetes/actions/workflows/publish.yaml)

# ansible-role-kubernetes
Rôle Ansible pour déployer un cluster Kubernetes (master + worker) avec containerd.

## Installation

```bash
ansible-galaxy install ulrich-sun.ansible-role-kubernetes
```

## Variables

k8s_version: Version Kubernetes à installer
pod_network_cidr: CIDR du réseau Pod
cri_socket: Socket CRI

## Exemple d’utilisation
```bash
- hosts: master
  roles:
    - role: ulrich-sun.ansible-role-kubernetes
```