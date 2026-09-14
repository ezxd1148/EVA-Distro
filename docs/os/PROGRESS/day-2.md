# Day 2: More work to do...

15 September 2026
> Started at 1am again...

# Steps taken

- Initialized new repo called EVA-Distro

- Checked out evangelion grub by Aleph1-9012

To be honest, I dont really know how to use it for my distro. I will be researching after I am done with archiso.

- Learned about [airrootfs](../TERMS/airrootfs.md)
  - Maybe I can put the evangelion grub here?
  - Not really, cachyos too, changed their grub after live installation

- Learned about [nftables](../TERMS/nftables.md)

- PLANNING: Look into pacman aur to add a repository usable in live env.
  - It said if repo uses key. what is key?

- Reached Kernel section 2.5 and thought it might be fun
  - [kernel](../TERMS/kernel.md)
  - edited linux-zen to be included in packages

ARCHISO TIPS:

To add a file to the install user's home directory, place it in archlive/airootfs/root/. To add a file to all other users home directories, place it in archlive/airootfs/etc/skel/.
