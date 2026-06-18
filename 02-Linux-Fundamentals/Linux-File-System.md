# Linux File System

## Overview

The Linux file system is organised into a hierarchical directory structure that starts from the root directory (`/`). Every file, directory, application, and device on a Linux system exists somewhere within this structure.

Unlike Windows, which uses drive letters such as `C:\` and `D:\`, Linux stores everything under a single directory tree beginning at the root.

Understanding the Linux file system is an essential skill for cybersecurity professionals because system logs, configuration files, user accounts, and security tools are all stored in specific locations.

---

## Why It Matters in Cybersecurity

A cybersecurity analyst regularly needs to:

- Locate log files during incident investigations.
- Identify configuration files that may have been modified.
- Analyse user directories for suspicious activity.
- Review system files for signs of compromise.
- Understand where applications and services store their data.

Strong knowledge of the Linux file system helps security professionals investigate, troubleshoot, and secure Linux systems more effectively.

---

# Linux Directory Structure

Below are some of the most important directories you will encounter on a Linux system.

```text
/
├── bin
├── boot
├── dev
├── etc
├── home
├── lib
├── media
├── mnt
├── opt
├── proc
├── root
├── run
├── sbin
├── srv
├── sys
├── tmp
├── usr
└── var
```

Each directory has a specific purpose, making Linux organised, secure, and efficient.

## / (Root)

The root directory (`/`) is the top of the Linux file system. Every file and directory on the system starts from here.

---

## /home

The `/home` directory stores personal files and folders for normal users.

Example:

```text
/home/mohsin
```

---

## /root

The `/root` directory is the home folder for the root (administrator) account.

---

## /etc

The `/etc` directory contains important system configuration files used by Linux and installed applications.

---

## /bin

The `/bin` directory contains essential command-line programs that are available to all users.

Examples include:

- ls
- cp
- mv
- cat
- pwd

---

## /sbin

The `/sbin` directory contains system administration commands that are mainly used by the root user.

Examples include:

- fsck
- reboot
- shutdown
- ip

---

## /usr

The `/usr` directory contains installed applications, shared libraries, documentation and utilities.

Most software installed on Linux is stored here.

---

## /var

The `/var` directory stores files that change frequently.

Examples include:

- System logs
- Cache
- Mail queues
- Databases

---

## /tmp

The `/tmp` directory is used for temporary files created by applications.

These files may be deleted automatically when the system restarts.

---

## /dev

The `/dev` directory contains device files that represent hardware connected to the system.

Examples include:

- Hard drives
- USB devices
- Terminal devices

---

## /proc

The `/proc` directory is a virtual file system containing information about running processes and the Linux kernel.

Cybersecurity professionals often use this directory when investigating running processes and system activity.

---

## /opt

The `/opt` directory is commonly used for optional third-party software packages.

---

# Cybersecurity Relevance

Understanding the Linux file system is a fundamental skill for cybersecurity professionals.

During security investigations, analysts regularly need to:

- Locate system log files.
- Review user directories.
- Examine configuration files.
- Investigate suspicious processes.
- Identify malware persistence locations.
- Analyse compromised systems.

Knowing where important files are stored allows faster incident response and more effective threat hunting.

# Practical Exercise

The following screenshot shows the root directory structure from my Kali Linux virtual machine.

![Linux Root Directories](02-Linux-Fundamentals/Images/Linux-root-directories.png.jpg)
