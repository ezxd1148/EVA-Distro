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

Set -eu flag

-e: Exits the script on error
-u: Treat unset variables as an error

It takes in 3 parametes, uninstall install and help.

then execute script from SCRIPT_DIR/bin/eva then inputs in the EVA_ACTION from user initial input "./install.sh (install/uninstall)"

## Dissecting eva

Set -Eeuo pipefail flag

-E: Exit on error
-e: Exit on error
-u: Treat unset variables as an error
-o: Fail on error
-p: Fail on error

Then takes in current SCRIPT_DIR && pwd meaning fetching the current directory

It will check if user run the script outside the directory, then source the script.

basically it checks if the user is in directory and if installation file are present

Then it sets in a bunch of functions
