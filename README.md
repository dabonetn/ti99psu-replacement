# ti99psu-replacement
Full drop in TI99/4a Power supply replacement. No soldering.


This board is a drop in replacement for the internal TI99/4a power board.
It uses a regulated +12V DC external power supply, 48 watt or greater.

Use a good quality supply, as this is the actual +12v for the computer.

This uses a DFR0831 5v buck converter, that's rated for +5v@4a, but I recommned no more than 3.5a draw.

You should also use a 2.5mm thermal pad underneath the DFR8031 to help cool it.

-5v is provided with a v7805-2000 switching regulator... It's overkill and will replaced with a 1a version later.
-5v is basically there for the 4116 ram.

The SUP53P06-20-E3 mosfet is there for reverse voltage input, but you can leave it out by connecting pins d & s ( the two close to the edge of the board)

This is a remix of the TI99-4A-dc-power-board by jonn-reenthused

https://github.com/jonn-reenthused/TI99-4A-dc-power-board

I wanted more than a 2a 5v supply, so I spun this up.

