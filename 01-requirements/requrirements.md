# 📋 System Requirements & Prerequisites

Before starting the dual-boot process, ensure you have everything needed for a smooth and successful installation. Preparing these items in advance will help prevent errors and mid-installation interruptions.

---

## 💻 Hardware Requirements

To comfortably run both Windows 11 and Ubuntu 26.04 LTS, your system should meet the following specifications:

*   **Processor:** 2 GHz dual-core processor or better (64-bit required).
*   **Memory (RAM):** 4 GB minimum (8 GB or more highly recommended for smooth multitasking).
*   **Storage Space:** 
    *   **Absolute Minimum:** 25 GB of unallocated free space.
    *   **Recommended:** 50 GB to 100+ GB of free space on your Windows drive (or a secondary drive) to accommodate the OS, software, and future updates.
*   **USB Flash Drive:** A blank USB drive with at least **8 GB** of capacity (Note: All data on this drive will be erased during the setup process).
*   **Power Source:** If you are using a laptop, ensure it is plugged into a charger. A power failure during partitioning or installation can cause severe system damage.

---

## 🛠️ Software & Tools

You will need to download a few essential files and tools while you are still booted into Windows 11. 

| Software / Tool | Description | Download Link |
| :--- | :--- | :--- |
| **Ubuntu 26.04 LTS ISO** | The official operating system image file. | [Download Ubuntu](https://ubuntu.com/download/desktop) |
| **Rufus** | A lightweight utility used to create a bootable USB drive (Windows only). | [Download Rufus](https://rufus.ie/) |
| **BalenaEtcher** | An alternative, user-friendly tool to flash the ISO to your USB (cross-platform). | [Download BalenaEtcher](https://etcher.balena.io/) |

> **Note:** We recommend **Rufus** for this guide as it offers specific settings for UEFI and GPT partition schemes, which pair best with modern Windows 11 systems.

---

## 🧠 Knowledge & Prep

*   **Time:** Set aside roughly **1 to 2 hours** to complete the entire process, including downloading files, partitioning, and installing.
*   **Administrator Access:** You must have Administrator privileges on your current Windows 11 account to shrink partitions and change system settings.

---

### ⏭️ Next Step
Once you have verified your hardware and downloaded the Ubuntu ISO and Rufus, you are ready to prepare your Windows system. 

Proceed to [02-Before-Installing / Backup](../02-Before-Installing/backup.md) to safeguard your data.