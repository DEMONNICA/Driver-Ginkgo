> `Changelog:`
> - All significant changes to this project will be documented here.
---

> [6.6.6]
>
> - License Changes.
> - Changed the structure of `README.md` for a better impression.
> - Updated `customize.sh` and `verify.sh` for better future performance.
> - Improved `detect_root_all` to match latest root manager variants.
> - Improved `set_donate_link` timezone detection with multiple fallbacks.
> - Fixed `local var=$(...)` declarations for better shell compatibility.
> - Fixed `post_install_actions` missing `NAME_MODULE` definition.
> - Fixed `MODDIR` missing closing quote in `uninstall.sh`.
> - Added `FolkLite` (`mi.yuki.folk`) detection to `detect_root_all`.
> - Added `set_donate_link` to `customize.sh`.
> - Added volume key driver selection for Android 10 (`Q-378` / `Q-415`).
> - Added automatic driver selection for Android 11 (`R`).
> - Added backup of original system files before driver is applied.
> - Added automatic restore of system files on uninstall via `uninstall.sh`.
> - Added GPU driver info to `module.prop` description via `service.sh`.
> - Removed `SKIPUNZIP=1` and `DEBUG=false` from `customize.sh`.
> - Removed legacy `service.sh` props and `pkill surfaceflinger` logic.
> - Updated `verify.sh` to match standard structure across all modules.
> - Added numbered comments throughout all scripts for better readability.
---

> [6.5.0]
>
> - Enhanced `detect_all_root` to make detection more extensive.
> - Changed module.prop `description` to be more professional.
---

> [6.0.0]
>
> - Changed module banner and removed `system.prop`, now it is created automatically.
> - Updating and improving all previous version code to make it more robust in the future.
> - And some other minor improvements and now it is more stable and safe for the future.
---