> `Changelog:`
> - All significant changes to this project will be documented in this file.
---

> [7.0.0]
>
> - Added `VortexSU` and spoofed build fallback detection to `detect_root_all`.
> - Added `busybox fstrim` fallback in `uninstall.sh` section 3.
> - Added `sm fstrim` before partition loop in `uninstall.sh` section 3.
> - Changed `detect_root_all` to loop-based structure with detection order APatch → KernelSU → Magisk.
> - Changed APatch `.method` file to 5 lines — added `APATCH_APP_VER`.
> - Changed `service.sh` to match updated `detect_root_all` detection order and 5-line APatch `.method` format.
> - Fixed `busybox chcon` in `uninstall.sh` — SELinux context was incorrectly applied to the backup file instead of the restored system file.
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