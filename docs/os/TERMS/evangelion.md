GRUB boot menu custom(evangelion)

Includes 720, 1080 and 1440 with 4K wallpaper

Lists:

- Ayanami
- Soryu
- Pen-Pen
- SEELE
- EVA-01
- Wunder
- EVA-02
- Ramiel

## What it requires

- Linux
- GRUB 2
- Bash
- awk

Installer should detects /boot/grub or /boot/grub2 and the available GRUB tools

It is tested on Arch Linux with GRUB 2.14(IMPORTANT)

## Flow

The user can choose the resolution(720, 1080 and 1440)

Installation uses a graphical theme for choosing an OS, then switches to a full-screen console when an entry stars.

GRUB displays the selected entry name


## Dissecting install.sh

This scripts takes in 3 parameters

- uninstall|--uninstall
- install | --install
- -h|--help|help

Then at the end it will exe "$SCRIPT_DIR/bin/eva" with its action(Install/uninstall)  $EVA_ACTION" and $@

eva is another bash script


