# Update Spring 2024- all mechboards ferris kits are now able to use standard Sweep firmware. If your sweep PCB has a QR code on it, you can disregard the below.

The MBUK Ferris Sweep PCBs do not have a pinout that matches the standard sweep in QMK master.

Additionally, the controller labelling on the PCB is confusing.

This is how the controllers should be oriented (choc version at the top- chips up, mx/choc version at the bottom- chips down).

![image](https://github.com/mechboardsguides/mbuk-ferris-readme/assets/19674258/86000e5b-b801-4511-9232-9e7fd0ad9052)


This is frustrating. It will be remedied in future releases of the PCB.

The pre-built PCBs should come flashed with a VIA keymap- you should be able to open https://usevia.app/ and see your keyboard connected, its keymap, and then be able to remap keys there.

For now, the firmware source can be found here: 

https://github.com/keyboard-magpie/qmk_firmware/tree/mbuk-ferris/keyboards/ferris/sweep_choc_mbuk for the Choc Only PCB
https://github.com/keyboard-magpie/qmk_firmware/tree/mbuk-ferris/keyboards/ferris/sweep_mx_mbuk for the Choc/MX PCB

To compile your own firmware for these PCBs, you should follow https://docs.qmk.fm/#/newbs_getting_started?id=set-up-qmk and when it comes to cloning your repository use `qmk setup keyboard-magpie/qmk_firmware` then you will need to check out the `mbuk-ferris` branch (you can type `qmk cd` then `git checkout mbuk-ferris` after setup has completed.

Someone has kindly provided a ZMK source here for one of the PCBs- i have not tested nor clarified which PCB this is for: https://github.com/flunderpero/ferris-zmk/tree/main/config/boards/shields/perosweep1

Sorry. This isn't an optimal experience.

If you run into issues, reach out on discord (https://discord.gg/mbuk)
