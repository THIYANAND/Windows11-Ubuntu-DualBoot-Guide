# 📂 Recommended Partition Layout

While modern installers handle this automatically, here is the recommended layout if you choose the "Manual" (Something Else) method:

*   **EFI Partition (Already exists):** Keep your existing 100-500 MB partition (System Reserved). Do not delete this!
*   **Root ( / ):** 30 GB to 100 GB. This is where the OS and apps live. (File system: `ext4`)
*   **Home ( /home ):** Remaining space. This is where your personal files live. (File system: `ext4`)
*   **Swap:** 4 GB - 8 GB. Use this if you hibernate or have limited RAM. (File system: `swap`)