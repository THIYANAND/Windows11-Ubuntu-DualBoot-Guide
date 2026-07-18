# 🔐 Step 2: Disable BitLocker Device Encryption

Windows 11 often enables **BitLocker** or "Device Encryption" by default. You **must** disable or suspend this before partitioning your drive. If BitLocker is active, Ubuntu cannot safely shrink your Windows partition, and changing boot settings might lock you out of Windows entirely.

## How to Check and Disable BitLocker

### Method A: For Windows 11 Pro / Enterprise Users
1. Click the **Start Menu**, type `Manage BitLocker`, and press **Enter**.
2. If it says **BitLocker is ON**, click **Turn off BitLocker**.
3. Confirm your choice and wait for the decryption process to finish. (This can take anywhere from a few minutes to an hour depending on your drive speed and data size).

### Method B: For Windows 11 Home Users (Device Encryption)
1. Open Windows **Settings** (Win + I).
2. Go to **Privacy & security** > **Device encryption**.
3. Toggle the switch to **Off**.
4. Wait for the decryption process to complete.

> **⚠️ CRITICAL BACKUP:** Even if you turn it off, it is highly recommended to back up your BitLocker Recovery Key. Log into your Microsoft Account online at [account.microsoft.com/devices/recoverykey](https://account.microsoft.com/devices/recoverykey) and save the 48-digit key on your phone or a piece of paper.

---

### ⏭️ Next Step
With your drive decrypted, you now need to [Disable Fast Startup](disable-fast-startup.md).