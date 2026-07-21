> ![Image](https://github.com/user-attachments/assets/e427dccf-4983-4535-9a3f-0241faa0c467)

> [!NOTE]
> ```
> Replaces the GPU driver on Redmi Note 8 with an optimized build for better graphics performance and stability.
> ```

> [!IMPORTANT]
> Features ✨:
> 1. Driver variant selection via volume key during installation.
> 2. Backs up original system driver files before replacing.
> 3. Restores original driver automatically on uninstall.

> [!TIP]
> 1. Supports `Magisk` `KernelSU` `KernelSU Next` `APatch` `SukiSU` and their variants.
> 2. Only supports Android `10 SDK 29` and Android `11 SDK 30`.
> 3. Only supports `aarch64 (arm64-v8a)` architecture.
> 4. To verify the active GPU driver after reboot, two methods are available:
>    - **Method 1** — Using a visual app:
>      Install [GPU Viewer (GLView)](https://play.google.com/store/apps/details?id=com.realtechvr.glviewpro) and open it after reboot. Navigate to the **GL** tab and check the **Renderer** and **Version** fields to confirm the applied driver.
>    - **Method 2** — Using ADB or Termux:
>      ```sh
>      dumpsys SurfaceFlinger | grep "GLES:" | sed 's/GLES: //'
>      ```
>      The output will display the active OpenGL ES driver string, for example:
>      ```
>      Qualcomm, Adreno (TM) 610, OpenGL ES 3.2 V@0615.0 ...
>      ```
>      The version string at the end reflects the currently loaded driver build.
>    > Both methods require the device to be rebooted after module installation.
> 5. If the driver is not applied after reboot, install **Meta** to enable system file overlay support:
>    - [Download Meta — Hybrid Mount](https://github.com/Hybrid-Mount/meta-hybrid_mount/releases)

> [!WARNING]
> 1. If you do not fully understand what a modification does, do not apply it.
> 2. Always have a recovery solution ready — TWRP, ADB, or fastboot — before proceeding.
> 3. Rooted devices with custom ROM may behave differently. Proceed with extra caution.
> 4. System modifications can be unpredictable. What works on one device may break another.
> 5. Any modification applied to the system is your decision. Think before you act.
> 6. The developer takes no responsibility for any damage, data loss, or device malfunction caused by the use of these works.
> 7. Redistribution, modification, or repackaging of these works without explicit permission from the author is strictly prohibited.

> [!CAUTION]
> Disclaimers 🛡️:
> - Use at your own risk. No guarantees are made regarding stability, compatibility, or safety. Always back up your data before installing anything.
> - These works are tested on specific devices only. Behavior on other devices may vary significantly.
> - The author reserves the right to discontinue, modify, or remove any module or plugin at any time without prior notice.