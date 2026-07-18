#### `05-After-Installation/battery.md`
```markdown
# 🔋 Improving Battery Life on Ubuntu

Linux can sometimes drain laptop batteries faster than Windows. Install **TLP**, an advanced power management tool, to optimize battery life automatically.

1. Open a terminal and run:
   ```bash
   sudo apt update
   sudo apt install tlp tlp-rdw
2. Start the service:
    ```bash
    sudo tlp start

TLP will now run quietly in the background every time you boot.