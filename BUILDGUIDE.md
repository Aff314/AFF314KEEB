# Bulid guide 🚧 WIP 🚧

If you want to build the board feel free to do that, but you should probably wait until I've actually tested if every thing works. Then there should also be a buildguide available. 

## Building the board

🚧 Wip 🚧

Is going to be posted once the parts arrive.
But you basically just have to solder everything on.


### Soldering the diodes
The diodes are really small and can be a bit tricky to solder but it's actually not that difficult.
The most important thing is that you solder them on in the right direction. You can find a line on the PCB and on the diode. They have to match. I recommend you to use flux for the diodes since it makes it alot easier.

As far as soldering goes you first have to put a bit of solder on one pad and place the correct diode leg on there, while heating it up with your soldering iron. Then you have to just solder on the other leg and if you need tou you can now improve the solder joint of the first leg.

### Soldering the hotswap sockets
Same as the diodes you have to solder on one side first and then the other.

If you build it without hotswap sockets you have to insert all switches and solder the oins directly.


### Soldering the MCU
At first you have to solder the pins to the MCU. I use MillMax pins which you can find in the BOM since they're more rigid, but you you can alternatively use through hole diode legs.
If you have a breadboard laying around use that and if you don't just try to make it as straight as possible. 

First cut the ic-sockets to 12 pin lenght if you've ordered the longer. Then push them into the breadboard, lay the MCU on it and push in the pins. Then you have to solder all the pins.

Now take out the sockets and place them on the PCB with the MCU attached and solder them from the bottom.


### Soldering the reset switch
Insert the reset switch and solder every thing on.


### Soldering the power switch solder 
You need to place the switch in it's position and first solder on the big pads and then the small ones. 


### Soldering the battery
If your battery has a connector you have to cut it off. The wires have to ba short enough so the battery fits properly under MCU.

Then you have to place the battery under the MCU. Turn off the power switch and solder the red wire to the + pad and the black wire to the - pad.


## Flashing the firmware
First you have to download the [uf2 file](Firmware/AFF314KEEB-nice_nano_v2-zmk.uf2) or you could build the firmware on your own if for example you wanted to change the keymap or anything else. 
If you want to build the firmware yourself [here](Firmware/ZMK_config) are the ZMK config files which you can modify and compile. If you don't know hot that works you can watch a [tutorial](https://www.youtube.com/watch?v=O_urj-rF3bQ).

Once you've got your uf2 file you have to put your MCU in bootloder mode by connecting it to your pc and double pressing the reset-button.
Once it shows up as a drive (probably named NICENANO) you have to copy the file to the MCU. It should now disconnect and then the firmware is succesfully flashed.





