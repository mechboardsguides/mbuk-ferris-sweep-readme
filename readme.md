The MBUK Ferris Sweep PCBs do not have a pinout that matches the standard sweep in QMK master.

This is frustrating. It will be remedied in future releases of the PCB.

For now, the firmware source can be found here: 

https://github.com/keyboard-magpie/qmk_firmware/tree/mbuk-ferris/keyboards/ferris/sweep_choc_mbuk for the Choc Only PCB
https://github.com/keyboard-magpie/qmk_firmware/tree/mbuk-ferris/keyboards/ferris/sweep_mx_mbuk for the Choc/MX PCB

To compile your own firmware for these PCBs, you should follow https://docs.qmk.fm/#/newbs_getting_started?id=set-up-qmk and when it comes to cloning your repository use `qmk setup keyboard-magpie/qmk_firmware` then you will need to check out the `mbuk-ferris` branch (you can type `qmk cd` then `git checkout mbuk-ferris` after setup has completed.

Sorry. This isn't an optimal experience.

If you run into issues, reach out on discord (https://discord.gg/mbuk)
