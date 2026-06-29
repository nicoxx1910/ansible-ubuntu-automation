# Case Study  
## Ubuntu Automation & Monitoring Lab (Ansible + Checkmk)

---

## 👤 Overview

This case study describes a small infrastructure automation and monitoring environment built for hands-on practice in Linux system administration, automation, and observability.

The environment simulates a real-world DevOps setup using Ubuntu Server, Ansible for automation, and Checkmk for monitoring.

---

## 🎯 Objective

The main goal of this project was to design and implement a reproducible Linux environment that demonstrates:

- Automated system administration
- Standardized server configuration
- Centralized monitoring
- Infrastructure-as-code principles

---

## 🏗️ Environment Design

The lab is built on a Proxmox virtualization platform running multiple Ubuntu Server virtual machines.

### Architecture

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
```

---

## ⚙️ Technologies Used

- Ubuntu Server 22.04 / 24.04
- Ansible (Automation & Configuration Management)
- Checkmk (Infrastructure Monitoring)
- Git (Version Control)
- Proxmox VE (Virtualization)

---

## 🔧 Implementation Details

### 1. Automation Layer (Ansible)

Ansible is used to manage:

- System patching
- Baseline configuration
- Monitoring agent deployment

All configurations are designed to be idempotent and reusable.

---

### 2. Baseline Configuration

Standardized configuration includes:

- Common packages installation
- Timezone configuration
- SSH service setup

---

### 3. Monitoring (Checkmk)

Checkmk is used for:

- Host availability monitoring
- CPU, memory, and disk usage tracking
- Service monitoring via agent-based checks

---

## 🧠 Design Principles

- Infrastructure-as-Code approach
- Separation of roles and responsibilities
- Reproducible system state
- Automation-first mindset
- Minimal manual configuration

---

## 📈 Outcome

The project demonstrates practical skills in:

- Linux system administration (Ubuntu)
- Infrastructure automation with Ansible
- Monitoring and observability with Checkmk
- Git-based workflow management
- Structured infrastructure design

---

## 🚀 Key Learnings

- Importance of idempotent automation
- Role-based Ansible structure improves maintainability
- Monitoring is essential in any real-world infrastructure
- Small lab environments can simulate production patterns

---

## 👤 Author

Linux System Administrator (Fachinformatiker Systemintegration)  
Focus: Linux, Automation, Infrastructure, Monitoring