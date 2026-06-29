# Ubuntu Automation & Monitoring Lab (Ansible + Checkmk)

> Infrastructure automation and monitoring lab based on Ubuntu Server, Ansible, and Checkmk.

---

## 🧭 Overview

This project demonstrates a small but realistic Linux infrastructure setup using Ubuntu Server, automated with Ansible and integrated with Checkmk for monitoring.

The focus is on:
- Linux system administration (Ubuntu Server)
- Infrastructure automation with Ansible
- Configuration management (IaC-style approach)
- Monitoring integration using Checkmk
- Reproducible and documented infrastructure

---

## 🏗️ Architecture

The lab is based on a Proxmox virtualization environment running multiple Ubuntu Server VMs.

```text
                 ┌─────────────────┐
                 │   Proxmox VE    │
                 └────────┬────────┘
                          │
         ┌────────────────┼────────────────┐
         │                │                │
 ┌─────────────┐  ┌─────────────┐  ┌─────────────┐
 │ Ubuntu-01   │  │ Ubuntu-02   │  │ Checkmk VM  │
 │ Web Server  │  │ App Server  │  │ Monitoring  │
 └──────┬──────┘  └──────┬──────┘  └─────────────┘
        │                │
        └────────┬───────┘
                 │
        ┌────────────────┐
        │ Ansible Node   │
        │ Automation     │
        └────────────────┘