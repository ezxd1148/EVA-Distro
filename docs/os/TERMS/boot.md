## bootloader flow (as far as I know)

1. bootloader loads linux kernel and archiso [initramfs](initramfs.md)
2. initramfs locates and mounts the ISO
3. it mounts the compressed [airootfs](airootfs.md) as a READ-ONLY base filesystem
4. It may place a writeable overlay on top of it
5. Combined overlay becomess the live system's '/'
6. Changes are written to the persistence layer only if persistence has been configured