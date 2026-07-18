# 🎛️ Customizing GRUB Bootloader

GRUB is the menu that appears when you turn on your PC, asking whether you want to boot into Ubuntu or Windows.

**To change the default OS or timeout:**
1. Open a terminal (`Ctrl + Alt + T`).
2. Edit the GRUB configuration file:
   ```bash
   sudo nano /etc/default/grub

**Steps do in the terminal**
1. Change GRUB_TIMEOUT=10 to your preferred number of seconds.

2. To make Windows the default, change GRUB_DEFAULT=0 to GRUB_DEFAULT=saved.

3. Save (Ctrl + O, Enter) and exit (Ctrl + X).

3. Update GRUB to apply changes:
```bash
   sudo update-grub