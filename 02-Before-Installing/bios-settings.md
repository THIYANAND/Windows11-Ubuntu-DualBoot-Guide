# ⚙️ Step 4: Configure BIOS / UEFI Settings

To allow Ubuntu to install and boot properly alongside Windows 11, you need to adjust a few settings in your motherboard's BIOS/UEFI.

## 1. How to Enter BIOS
1. Restart your Windows PC.
2. As soon as the screen turns on, rapidly and repeatedly press your manufacturer's BIOS key until the BIOS screen appears.
   * **Common BIOS Keys:** `F2`, `F12`, `F10`, `DEL`, or `ESC` (varies by brand).

## 2. Essential BIOS Changes

Navigate through your BIOS menus (usually using arrow keys or your mouse) and make the following changes:

| Setting | Action | Why? |
| :--- | :--- | :--- |
| **Secure Boot** | Disable | While Ubuntu supports Secure Boot, third-party drivers (like Wi-Fi or NVIDIA GPU drivers) often fail to install if it is left on. |
| **SATA Operation / Storage Mode** | Change from `RAID` to `AHCI` | Ubuntu cannot detect your NVMe or SATA SSD if it is configured to Intel RST/RAID mode. *(See Warning Below)* |
| **Boot Order / Priority** | Set USB Drive to #1 | Allows the system to boot from your Ubuntu installation USB instead of Windows. |

> **🚨 IMPORTANT WARNING ABOUT AHCI:** 
> If your system is currently in **RAID** mode and you simply switch it to **AHCI**, Windows 11 will crash (Blue Screen of Death) on the next boot because it lacks the right storage drivers. 
> *If your system is already in AHCI, you can ignore this.*
> *If you need to switch from RAID to AHCI, you must boot Windows into Safe Mode once immediately after changing the setting so it can install the AHCI drivers. Search our troubleshooting guide for "Switching RAID to AHCI safely" if you need help.*

## 3. Save and Exit
Once the settings are configured, go to the **Save & Exit** tab (or press `F10`), save your changes, and reboot.

---

### ⏭️ Next Step
Your PC is now fully prepped! Move on to the [03-Partitioning](../03-Partitioning/shrink-volume.md) phase to make space for Ubuntu.