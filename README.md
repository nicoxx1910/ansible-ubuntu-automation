# Ubuntu Automation Lab (Ansible)

This repository contains Ansible playbooks for automating Ubuntu-based Linux systems in a small homelab environment.

## Focus Areas

- Ubuntu Server administration
- Infrastructure automation with Ansible
- System hardening and baseline configuration
- Monitoring integration (Checkmk)
- Git-based configuration management

## Environment

- Proxmox VE (virtualization platform)
- 1 Ansible control node (Ubuntu)
- 2 Ubuntu Server VMs
- 1 Monitoring system (Checkmk agent)

## Technologies

- Ubuntu Server 22.04/24.04
- Ansible
- Checkmk agent
- Git
- Proxmox VE

## Playbooks

| Playbook | Description |
|----------|-------------|
| patching.yml | System updates & security patches |
| baseline.yml | Basic server configuration |
| checkmk-agent.yml | Install & configure Checkmk monitoring agent |

## Usage

```bash
ansible-playbook playbooks/patching.yml
```

---

## Goal

The goal of this project is to demonstrate practical Linux administration skills using Ubuntu, with a strong focus on automation, monitoring, and reproducible infrastructure.