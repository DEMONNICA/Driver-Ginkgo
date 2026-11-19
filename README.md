> ![Image](https://github.com/user-attachments/assets/e427dccf-4983-4535-9a3f-0241faa0c467)

> [!NOTE]
> ```
> Replaces the GPU driver on Redmi Note 8 with an optimized build for better graphics performance and stability.
> ```

> [!IMPORTANT]
> Features ✨:
> 1. Driver variant selection via volume key during installation.

> [!TIP]
> 1. Supports `APatch` `KernelSU` `Magisk` and their forks.
> 2. Only supports Android `10 SDK 29` and Android `11 SDK 30`.
> 3. Only supports `Redmi Note 8 Ginkgo`.
> 4. To verify the active GPU driver after reboot, use [GPU Viewer (GLView)](https://play.google.com/store/apps/details?id=com.realtechvr.glviewpro) or run in Termux:
>    ```sh
>    dumpsys SurfaceFlinger | grep "GLES:" | sed 's/GLES: //'
>    ```
> 5. <details>
>    <summary>Use a metamodule for compatibility with this module</summary>
>
>    [Hybrid Mount](https://github.com/Hybrid-Mount/meta-hybrid_mount) | [NoMount](https://github.com/maxsteeel/nomount) | [ZeroMount](https://github.com/Enginex0/zeromount) | [Mountify](https://github.com/backslashxx/mountify)
>
>    </details>

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