#### `06-Recovery/reinstall-grub.md`
```markdown
# 💻 Reinstalling GRUB via Terminal (Chroot)

If Boot-Repair fails, you can manually reinstall GRUB from a Live USB terminal. 

*(Note: Replace `nvme0n1` with your actual drive identifier found via `lsblk`)*
    ```bash
    sudo mount /dev/nvme0n1pX /mnt         # Mount your root partition
    sudo mount /dev/nvme0n1pY /mnt/boot/efi # Mount your EFI partition
    for i in /dev /dev/pts /proc /sys /run; do sudo mount -B $i /mnt$i; done
    sudo chroot /mnt
    grub-install /dev/nvme0n1
    update-grub
    exit
    Reboot safely.
    ```