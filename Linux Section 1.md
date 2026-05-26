# Linux Operating System

## What is Linux?

Linux is an open-source operating system where users interact with the OS using:

- CLI (Command Line Interface) in Linux
- GUI (Graphical User Interface) in Windows

An Operating System acts as a central layer between the user and the hardware.

---

# History of Operating Systems

| Year | Technology |
|---|---|
| 1960 | Unix (Open Source) |
| 1970 | Minix (Not fully Open Source) |
| 1980 | Windows |
| 1990 | Linux Kernel |

Linux became a popular choice because it is:

- Open Source
- Free to use
- Community Driven
- Secure and Stable

---

# Linux Kernel

The Linux Kernel is the core part of Linux.

It interacts directly with hardware like an engine inside a car.

### Linux Architecture

```text
CLI/Binary
↓
System Libraries
↓
System Utilities
↓
Kernel
↓
Hardware
```

---

# Kernel Responsibilities

The Kernel manages:

- Process Management
- Memory Management
- File System
- Network Management

---

# Hardware Components

Linux interacts with hardware components such as:

- CPU
- RAM
- Disk
- Network Devices

---

# Layers of Linux

## 1. Shell

Examples:
- Bash
- Zsh
- Fish

The shell allows users to communicate with the operating system.

---

## 2. System Libraries

Examples:
- glibc
- libc
- OpenSSL

Libraries help software communicate with the kernel.

---

## 3. System Utilities

Examples:
- ls
- grep
- systemctl

Utilities are commands used for system management and operations.

---

# Linux Distributions

Linux distributions are customized versions of Linux with different tools and package managers.

Everything is mostly common across distributions.

## Popular Linux Distributions

- Ubuntu
- RedHat
- Debian
- Alpine
- Fedora

---

# Setup Linux on Windows

Install WSL (Windows Subsystem for Linux)

```bash
wsl --install
```

---

# Package Managers

Package Managers help to:

- Install Packages
- Upgrade Packages
- Remove Packages
- Manage Dependencies

---

## APT Package Manager

APT is commonly used in Ubuntu and Debian-based systems.

### List Packages

```bash
apt list
```

Lists all available packages.

---

### Install Package

```bash
apt install python3
```

This installs Python3 from authorized repositories.

---

### Update Packages

```bash
apt update
```

Updates package information from repositories.