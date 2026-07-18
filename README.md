# 🪟 Windows 11 & 🐧 Ubuntu 26.04 LTS Dual Boot Guide

![OS](https://img.shields.io/badge/OS-Windows_11-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![OS](https://img.shields.io/badge/OS-Ubuntu_26.04_LTS-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![Open Source](https://img.shields.io/badge/Open_Source-❤️-red?style=for-the-badge)
![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-brightgreen?style=for-the-badge)

Welcome to the **Windows 11 & Ubuntu 26.04 LTS Dual Boot Guide**! This open-source documentation project is designed to help users install and maintain a stable dual-boot environment without common installation or boot-related issues. 

Whether you are a beginner, student, developer, or professional, this repository provides a step-by-step guide covering the entire process—from preparing a Windows system to successfully installing Ubuntu alongside it while preserving data and ensuring reliable boot management.

---

## 📖 About the Project

Unlike traditional installation tutorials, this repository emphasizes troubleshooting, recovery procedures, and best practices collected from practical experience. Every topic is documented with clear explanations, screenshots, terminal commands, and recovery methods.

We focus on solving real-world problems encountered during dual-boot installation, including:
- GRUB bootloader issues
- UEFI and Secure Boot configuration
- GPT partitioning
- BitLocker and Fast Startup conflicts
- Windows time synchronization issues
- Driver installation & post-installation optimization

---

## ✨ Key Features

- **🚀 Complete Step-by-Step Guide:** Safe and comprehensive Windows 11 + Ubuntu 26.04 LTS installation.
- **💾 Safe Disk Partitioning:** Learn to manage space without risking data loss (UEFI, GPT, and EFI config).
- **🛠️ GRUB Management:** Installation, recovery, and deep-dive troubleshooting.
- **🚑 Rescue & Recovery:** Windows recovery, boot restoration procedures, and solutions for common installation errors.
- **⚙️ Post-Install Polish:** Driver installation, hardware compatibility, and system optimization for battery life and performance.
- **🖼️ Visual & Clear:** Easy-to-follow documentation enriched with screenshots and thorough command explanations.
- **🤝 Community-Driven:** Open-source improvements and updates driven by practical user experiences.

---

## 🎯 Project Goals

1. **Reduce Installation Failures:** Make the dual-boot setup process smooth and error-free.
2. **Provide Reliable Solutions:** Serve as a definitive guide for frequently encountered dual-boot issues.
3. **Empower New Users:** Help new Linux users confidently migrate or experiment with Ubuntu.
4. **Build a Knowledge Base:** Maintain a continuously updated resource backed by the open-source community.
5. **Promote Linux Adoption:** Make trying Linux alongside Windows simpler, safer, and more accessible for everyone.

---

## 📁 Repository Structure

Navigate through the folders below to follow the guide chronologically, or jump straight to the section you need help with.

```text
Windows11-Ubuntu26.04-DualBoot-Guide/
│
├── README.md                 # You are here!
│
├── 01-Requirements/          # What you need before starting
│   └── requirements.md
│
├── 02-Before-Installing/     # Pre-flight checks on Windows
│   ├── backup.md
│   ├── disable-bitlocker.md
│   ├── disable-fast-startup.md
│   └── bios-settings.md
│
├── 03-Partitioning/          # Making space for Linux
│   ├── shrink-volume.md
│   ├── partition-layout.md
│   └── ntfs-errors.md
│
├── 04-Ubuntu-Installation/   # The main installation phase
│   ├── installation.md
│   ├── manual-partitioning.md
│   └── secure-boot.md
│
├── 05-After-Installation/    # Post-install fixes and optimizations
│   ├── grub.md
│   ├── windows-not-showing.md
│   ├── time-sync.md
│   ├── wifi.md
│   ├── nvidia.md
│   ├── battery.md
│   ├── touchpad.md
│   └── updates.md
│
├── 06-Recovery/              # What to do if things go wrong
│   ├── grub-repair.md
│   ├── boot-repair.md
│   ├── reinstall-grub.md
│   └── restore-windows.md
│
├── screenshots/              # Visual aids used across the guide
│
└── LICENSE                   # Project licensing details