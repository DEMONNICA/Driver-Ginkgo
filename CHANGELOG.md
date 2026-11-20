> `Changelog:`
> - All significant changes to this project will be documented in this file.
---

> [8.0.0]
>
> - Added author verification (`@illumi`) to `verify_module_id` in `verify.sh`.
> - Added RAM/storage variant check to `device_info` — only Redmi Note 8 variants 3GB/32GB, 4GB/64GB, and 6GB/128GB are supported.
> - Changed `detect_root_all` — simplified to detect only APatch, KernelSU, and Magisk based on `/data/adb/ap`, `/data/adb/ksu`, and `/data/adb/magisk` paths. Root variants are no longer distinguished.
> - Changed `device_info` — RAM and storage are now detected and shown as `RAM: 6GB total | 128GB storage`, rounded up to the nearest standard size via `round_up_gb`.
> - Changed `service.sh` to match `detect_root_all` detection order (APatch → KernelSU → Magisk) and the 4-line APatch `.method` format.
> - Changed `print_random_devil_message` — added `Baal`, removed `Lucius`, and demon names sorted alphabetically.
> - Changed driver directory structure from `Q-378` and `Q-415` to `Q/378` and `Q/415`, updated `SELECTED_DIR` in `customize.sh`.
> - Removed package manager (`pm`), `aapt`, and `ksud` based root detection from `detect_root_all`.
> - Removed backup of original system files from `customize.sh` and `restore_system_files` from `uninstall.sh` — the module is systemless, so original files are never modified and return when the module is removed.
---

> [7.0.0]
>
> - Added GPU driver verification guide to `README.md` — two methods via GLView app and `dumpsys SurfaceFlinger | grep "GLES:" | sed 's/GLES: //'`.
> - Added Hybrid Mount reference to `README.md` under TIP section.
> - Fixed `busybox chcon` in `uninstall.sh` — SELinux context was incorrectly applied to the backup file instead of the restored system file.
> - Removed feature 6 (thumbnail cache verification) from `README.md` IMPORTANT section.
> - Removed `zip=$(clean_path "$zip")` from `extract()` in `verify.sh`.
---

> [6.6.6]
>
> - Added `FolkLite` (`mi.yuki.folk`) detection to `detect_root_all`.
> - Added `set_donate_link` to `customize.sh`.
> - Added volume key driver selection for Android 10 (`Q-378` / `Q-415`).
> - Added automatic driver selection for Android 11 (`R`).
> - Added backup of original system files before driver is applied.
> - Added automatic restore of system files on uninstall via `uninstall.sh`.
> - Added GPU driver info to `module.prop` description via `service.sh`.
> - Added numbered comments throughout all scripts for better readability.
> - Changed license from GNU General Public License to Apache License 2.0.
> - Changed the structure of `README.md` for a better impression.
> - Changed `customize.sh` and `verify.sh` for better future performance.
> - Changed `detect_root_all` to match latest root manager variants.
> - Changed `set_donate_link` timezone detection with multiple fallbacks.
> - Changed `verify.sh` to match standard structure across all modules.
> - Fixed `local var=$(...)` declarations for better shell compatibility.
> - Fixed `post_install_actions` missing `NAME_MODULE` definition.
> - Fixed `MODDIR` missing closing quote in `uninstall.sh`.
> - Removed `SKIPUNZIP=1` and `DEBUG=false` from `customize.sh`.
> - Removed legacy `service.sh` props and `pkill surfaceflinger` logic.
---

> [6.5.0]
>
> - Changed `detect_all_root` to make detection more extensive.
> - Changed `module.prop` description to be more professional.
---

> [6.0.0]
>
> - Changed module banner.
> - Changed all previous version code to be more robust.
> - Removed `system.prop` — now created automatically.
---

> [5.0.0]
>
> - Added module banner for KernelSU Next.
> - Added LMK and `process_reclaim` optimizations to make things a bit better.
> - Changed `uninstall.sh` to be more effective and efficient.
> - Changed `README.md` to be more professional.
> - Fixed other minor issues.
> - Removed the `animation_scale` part, which was not working properly.
> - Removed the `icon.png` part, now only 1 icon is used.
---

> [4.0.0]
>
> - Added UI / Graphics / Animations and GPU / Vulkan / Skia tweaks.
> - Added Scheduler / I/O and RAM Management tweaks.
> - Added Thermal / CPU Tuning and Touch Response tweaks.
> - Changed `uninstall.sh` — updated existing code and added new code.
> - Changed `service.sh` to be faster and more optimal.
---

> [3.0.0]
>
> - Added `system.prop` for quality improvement.
> - Added GPU rendering optimizations for Redmi Note 8 on AOSP Android 10.
> - Added hardware composer and EGL usage for enhanced graphics handling.
> - Added advanced SurfaceFlinger tweaks to reduce frame latency and jitter.
> - Added background blur support in SurfaceFlinger for enhanced visual effects.
> - Added touch input resampling support to enhance touch accuracy and smoothness.
> - Added power and thermal configuration overrides to sustain peak GPU performance.
> - Added purgeable assets support to free memory more aggressively, improving multitasking.
> - Changed GPU rendering to force GPU rendering and disable Vulkan usage for better compatibility.
> - Changed GPU tuning properties to increase max frequency and scaling for improved performance.
> - Changed GPU frequency settings for better thermal management.
> - Changed animation and transition scale to 0.5 and reduced default animation durations for smoother, more fluid, and snappier UI transitions.
> - Changed scheduler and RenderThread priorities to improve UI responsiveness.
> - Changed Skia renderer settings to improve rendering efficiency on Adreno GPUs.
> - Changed frame buffer acquisition limits to reduce frame drops during heavy GPU load.
> - Changed RenderThread and HWUI support to ensure smooth UI rendering under load.
> - Changed profiling and debugging flags to assist in performance tuning.
> - Changed to improve compatibility with custom kernels supporting Vulkan and GPU tuning.
> - Fixed minor issues with GPU max/min frequency property application on certain ROMs.
---

> [2.0.0]
>
> - Added `verify.sh` to automate the integrity check.
> - Added `uninstall.sh` to remove the module contents.
> - Added notification to `module.prop`.
> - Changed the build.
> - Changed the Magisk structure.
> - Changed `customize.sh`.
> - Changed `module.prop`.
---

> [1.0.0]
>
> - Initial release.
---