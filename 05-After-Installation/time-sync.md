#### `05-After-Installation/time-sync.md`

# 🕒 Fixing the Windows & Ubuntu Time Sync Issue

When dual-booting, you might notice that Windows displays the wrong time after booting from Ubuntu. This happens because Ubuntu uses UTC for the hardware clock, while Windows uses Local Time.

The Fix (Run this in Ubuntu terminal):
    ```bash
    timedatectl set-local-rtc 1 --adjust-system-clock

Restart into Windows, correct the time once, and they will remain perfectly synced moving forward.