# ⚠️ Troubleshooting NTFS Errors
If Windows "Disk Management" refuses to shrink your volume:
1. **Disable Hibernation:** Open CMD as Admin and type: `powercfg /h off`
2. **Run CheckDisk:** Type `chkdsk c: /f /r` in CMD as Admin and restart the PC.
3. **Defragment:** Use the built-in Windows "Defragment and Optimize Drives" tool.