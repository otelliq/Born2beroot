# Born2beroot

> A hands-on introduction to Linux system administration and virtualization by provisioning and hardening a first virtual machine (42 School project).

![Topic](https://img.shields.io/badge/topic-virtualization%20%26%20sysadmin-informational)
![OS](https://img.shields.io/badge/os-Linux-lightgrey)
![Project](https://img.shields.io/badge/42%20School-Born2beroot-black)

## Overview

**Born2beroot** is a foundational DevOps / sysadmin project focused on creating a secure, well-configured Linux virtual machine.

The goal is to practice the real-world basics you’d use in production environments:

- installing a Linux distribution in a VM
- configuring users, groups, sudo policies
- applying security best practices (password policy, firewall, SSH hardening)
- understanding services, logging, and monitoring

**Repository:** `otelliq/Born2beroot`  
**Default branch:** `main`

## Key features (what you typically implement in this project)

> This repository currently contains only a `signature.txt` artifact (likely the VM image signature / submission proof). The list below describes the typical deliverables for *Born2beroot*.

- Virtual machine provisioning (VirtualBox / UTM / VMware)
- Linux installation (commonly Debian or Rocky)
- SSH server configuration and safe remote access
- Sudo setup and restricted administrative actions
- Firewall configuration (e.g., UFW / firewalld)
- Password policy enforcement and user management
- Basic monitoring / logging (depending on the rubric)

## Screenshots

> No screenshots provided yet.

Suggested screenshots to add:
- VM login screen / terminal
- `uname -a` and OS version
- `ss -tulpn` / open ports
- Firewall status output

## Installation / Setup

This project is VM-based. A common workflow:

1. Install a hypervisor:
   - VirtualBox (cross-platform)
   - UTM (macOS)
   - VMware
2. Create a new VM and attach your Linux ISO.
3. Install Linux and complete base configuration.
4. Apply hardening steps required by the rubric (SSH, firewall, password policy, sudo).

## Usage

Because the VM image itself isn’t stored here, the best way to “use” the project is to document and demonstrate the configuration from inside the VM.

Typical commands you may showcase:

```bash
# OS + kernel
uname -a

# Users and groups
id <user>
getent group sudo

# Firewall
sudo ufw status

# SSH
sudo systemctl status ssh
ss -tulpn | grep :22
```

## Project structure

```text
.
├── README.md
└── Born2beroot/
    └── signature.txt
```

## License

No license file is currently included in this repository.

If you want this documentation to be reusable, consider adding a `LICENSE` file.
