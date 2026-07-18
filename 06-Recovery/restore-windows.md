#### `06-Recovery/restore-windows.md`

# 🪟 Restoring the Windows Bootloader

If you decide to delete Ubuntu and want your PC to boot directly into Windows again without the GRUB menu:

1. Boot from a **Windows 11 Installation USB**.
2. Click **"Repair your computer"** > **Troubleshoot** > **Command Prompt**.
3. Run the following commands:
   ```cmd
   bootrec /fixmbr
   bootrec /fixboot
   bootrec /scanos
   bootrec /rebuildbcd
   ```
Restart your PC. You can now safely delete the Ubuntu partitions from Windows Disk Management.