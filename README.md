# MCP23S17 Breakout Board

[![Creative Commons License](https://i.creativecommons.org/l/by-sa/4.0/80x15.png)](http://creativecommons.org/licenses/by-sa/4.0/)

![Board front](https://github.com/squarefrog/mcp23s17-breakout-board/raw/master/images/top.png "Board top")
![Board back](https://github.com/squarefrog/mcp23s17-breakout-board/raw/master/images/bottom.png "Board bottom")

A 30x40mm breakout board for the [MCP23S17](http://www.microchip.com/wwwproducts/en/MCP23S17) SOIC package.

As used in my [MIDI Encoder Box](https://github.com/squarefrog/teensy-midi-encoder-box) project.

## Assembly

1. Start by soldering the MCP23S17 chip onto the board. Ensure you note the position of pin 1 by looking for the dot on the board and the chip.

2. **NOTE:** before proceeding any further, consider what you'd like the hardware address of the chip to be. There are 3 solder jumpers at the top of the board. You may use these to assign an address to the chip. Connect the middle pin of `A0`, `A1`, `A2`, to either ground (labelled `0`), or VDD (labelled `1`). Simply use some solder to join the two pads together.

3. Next, solder on the 2 1x8 header pins. Solder one edge pin first, then check that the header is straight. Once you're happy the header is straight solder the rest of the pins.

4. Now do the same for the 2 1x2 interrupt and power pins.

5. Finally, solder the 2 1x4 SPI header pins in place. Optionally, you may want to use 1x6 headers and get an extra few ground connections.

## IMPORTANT

Ensure you don't forget to solder the jumper pads. Even if you don't plan to use hardware addressing, you should bridge between the middle pin and ground pin.

