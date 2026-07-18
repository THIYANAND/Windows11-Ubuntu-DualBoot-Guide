# ⚡ Step 3: Disable Fast Startup

**Fast Startup** is a Windows feature that puts your PC into a hybrid hibernation state instead of fully shutting it down. 

**Why disable it?** When Fast Startup is enabled, Windows locks the NTFS partition (your `C:` drive) to resume quickly. If Ubuntu tries to read or mount a locked Windows drive during installation, it can cause partition errors, read-only file system issues, or GRUB bootloader failures.

## How to Disable Fast Startup in Windows 11

1. Press `Win + R` to open the Run dialog.
2. Type `control` and press **Enter** to open the **Control Panel**.
3. Change the "View by" setting (top right) to **Large icons**.
4. Click on **Power Options**.
5. On the left sidebar, click **Choose what the power buttons do**.
6. Click the blue text that says **Change settings that are currently unavailable** (requires Administrator privileges).
7. Under the *Shutdown settings* section, **uncheck** the box next to **Turn on fast startup (recommended)**.
8. Click **Save changes**.

> **Note:** Disabling this might make your Windows boot a few seconds slower, but it is strictly necessary for a healthy dual-boot environment.

---

### ⏭️ Next Step
Now it's time to prepare your motherboard. Proceed to [Configure BIOS/UEFI Settings](bios-settings.md).