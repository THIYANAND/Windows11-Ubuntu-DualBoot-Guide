# 🕒 Fixing the Windows & Ubuntu Time Sync Issue

When dual-booting, you might notice that Windows displays the wrong time after booting from Ubuntu. This happens because Ubuntu uses UTC for the hardware clock, while Windows uses Local Time.

## The Fix

Run the following command in the Ubuntu terminal:

```bash
sudo timedatectl set-local-rtc 1 --adjust-system-clock
```

Restart into Windows, correct the time once (if necessary), and both operating systems should remain synchronized moving forward.