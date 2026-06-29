# Architecture Overview

The lab is based on Proxmox VE and runs multiple Ubuntu Server virtual machines.

## Components

- Proxmox VE hypervisor
- Ubuntu Ansible control node
- Ubuntu Server 01 (application host)
- Ubuntu Server 02 (test host)
- Checkmk monitoring system

## Flow

Ansible is used to manage configuration, patching, and monitoring setup across all Ubuntu systems.

                 ┌─────────────────┐
                 │   Proxmox VE    │
                 └────────┬────────┘
                          │
         ┌────────────────┼────────────────┐
         │                │                │
 ┌─────────────┐  ┌─────────────┐  ┌─────────────┐
 │ RHEL-01     │  │ RHEL-02     │  │ Icinga VM   │
 │ Web Server  │  │ App Server  │  │ Monitoring  │
 └──────┬──────┘  └──────┬──────┘  └─────────────┘
        │                │
        └────────┬───────┘
                 │
        ┌────────────────┐
        │ Ansible Node   │
        │ Playbooks/Git  │
        └────────────────┘
