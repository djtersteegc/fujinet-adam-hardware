After building a few of mozzwald's original [FujiNet](https://fujinet.online/fujinet/) for [Coleco ADAM](https://fujinet.online/fujinet/#ColecoADAM) boards, I decided I wanted to create a new SMD version that was a bit quicker to assemble for folks building them in quantity, but still sticking with the ESP Devkit board and larger 0805 sized components for the DIY crowd. Both boards are single sided for easy assembly, with the only through hole parts being the RJ12 jack(s), LED's, and the devkit board itself. In the end I ended up with two different designs, one I'm calling the Devkit SMD and the other the Devkit Mini.

# Devkit SMD

Similar to the original design, this one offers two ADAMNet ports to daisy chain other devices, but instead of a microSD slot, now offers a full size SD card.

![devkit-smd](docs/devkit-smd.jpg)

You can build it in two different configurations, one using 8.5mm female headers for the devkit board, similar to the original.  This gives the options of reusing the ESP32 for something else in the future and easy access to the SMD components underneath it.  If you are confident in your soldering skills and want something more compact, you can also build it with the ESP board soldered directly to the main PCB on 3mm spaces.

![devkit-smd-tall-vs-short](docs/devkit-smd-tall-vs-short.jpg)

See the [Devkit SMD page](fujinet-adam-devkit-smd/README.md) for BOM and assembly instructions.

# Devkit Mini

This was an exercise in can I make a full Fujinet fit in the space of the devkit PCB. For that I had to go back to a microSD slot and it only supports one ADAMNet port.

![devkit-mini](docs/devkit-mini.jpg)

![devkit-mini-esp32](docs/devkit-mini-esp32.JPG)

See the [Devkit Mini page](fujinet-adam-devkit-mini/README.md) for BOM and assembly instructions.

# Getting a Bare Board or Assembled Unit

Any extras I have available will be in my [Tindie](https://www.tindie.com/stores/tersteeg/) store. I don't ship outside the US currently, but gerber files are available for both boards if you want to order your own from your favorite PCB fab like JLCPCB or PCBWay.

