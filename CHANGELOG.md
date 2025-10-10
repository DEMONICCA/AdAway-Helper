> `Changelog:`
> - All significant changes to this project will be documented here.
---

> [1.0.0] `FIX`
>
> - Optimized hosts file mounting in `customize.sh` with `mount -o bind` and fallback to copy, ensuring reliable ad-blocking across root environments.
> - Added SELinux context restoration in `customize.sh` using `busybox chcon` to match `/system/etc/hosts` for seamless integration.
> - Updated `service.sh` to replace `[BETA]` with `[FIX]` in `module.prop`, reflecting improved module stability.
> - Enhanced `service.sh` with fallback `cp -f` for hosts file if `mount -o bind` fails, improving compatibility on diverse devices.
> - Removed redundant `skip_mount` file creation in `customize.sh` for cleaner installation process.
> - Streamlined author update in `service.sh` by assuming existing author line, simplifying `module.prop` modifications.
> - Minor tweaks for consistent execution and error handling across scripts.
---

> [0.5.0] `BETA`
>
> - Initial release.
---