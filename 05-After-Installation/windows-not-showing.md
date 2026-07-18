#### `05-After-Installation/windows-not-showing.md`
```markdown
# 👻 Windows 11 Not Showing in GRUB

If Ubuntu boots directly and skips the GRUB menu, or if Windows is missing from the list:

1. Open a terminal and install `os-prober`:
   ```bash
   sudo apt install os-prober
   ```

1. Edit the GRUB file:
    ```bash
   sudo nano /etc/default/grub
   ```
   
2. Add or uncomment the following line at the bottom:

3. Plaintext
    GRUB_DISABLE_OS_PROBER=false
4. Save and exit, then update GRUB:

    ```bash
   sudo update-grub
   ```