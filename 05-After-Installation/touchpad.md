#### `05-After-Installation/touchpad.md`
```markdown
# 🖱️ Touchpad Gestures & Troubleshooting

Ubuntu uses `libinput` by default, which supports basic multi-touch gestures. If your touchpad feels unresponsive or lacks palm rejection:

1. Ensure your system is fully updated.
2. If you want advanced gestures (like macOS/Windows precision gestures), install `touchegg`:
   ```bash
   sudo add-apt-repository ppa:touchegg/os
   sudo apt update
   sudo apt install touchegg