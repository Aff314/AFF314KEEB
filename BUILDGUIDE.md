# Bulid guide 🚧 WIP 🚧

If you want to build the board feel free to do that, but you should probably wait until I've actually tested if every thing works. Then there should also be a buildguide available. 

## Building the board

🚧 Wip 🚧

Is going to be posted once the parts arrive.
But you basically just have to solder everything on.

## Flashing the firmware
First you have to download the [uf2 file](Firmware/AFF314KEEB-nice_nano_v2-zmk.uf2) or you could build the firmware on your own if for example you wanted to change the keymap or anything else. 
If you want to build the firmware yourself [here](Firmware/ZMK_config) are the ZMK config files which you can modify and compile. If you don't know hot that works you can watch a [tutorial](https://www.youtube.com/watch?v=O_urj-rF3bQ).

Once you've got your uf2 file you have to put your MCU in bootloder mode by connecting it to your pc and double pressing the reset-button.
Once it shows up as a drive (probably named NICE NANO) you have to copy the file to the MCU. It should now disconnect and then the firmware is succesfully flashed.



