## What is it?

It is a **Temporary filesystem image that the LLinux kernel loads into memory to help mount the real root filesystem**

## Relationship with airootfs and rootfs

[airootfs](airrootfs.md)

and there is also [rootfs](rootfs.md)

AND theres also [ramfs](ramfs.md)

## Basically

initramfs boots live environment, loads modules, finds ISO, mounts live ecosystem.

**BUT** airootfs is THE files and programs available after boot

