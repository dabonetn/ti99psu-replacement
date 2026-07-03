# ti99psu-replacement
Full drop in TI99/4a Power supply replacement. No soldering.


This board is a drop in replacement for the internal TI99/4a power board that uses the pin headers to connect to the motherboard.
There is a header to install the pigtail that some early units used.

It uses a regulated +12V DC external power supply, 48 watt or greater. (4amp)

Use a good quality supply, as this is the actual +12v for the computer.

This uses a DFR0831 5v buck converter, that's rated for +5v@4a, but I recommned no more than 3.5a draw.

There's a error on the schematics, the 220ohm resistor isn't enough for modern leds, so I recommend a 560ohm for bright or 2.2k for dull.

You should also use a 2.5mm thermal pad underneath the DFR8031 to help cool it.

-5v is provided with a P78E05-1000 switching regulator...This is rated for 1amp compared to the originals .5 amp.
-5v is basically there for the 4116 ram.

The mosfet is there for reverse voltage input, but you can leave it out by connecting pins d & s ( the two close to the edge of the board)

This is a remix of the TI99-4A-dc-power-board by jonn-reenthused

https://github.com/jonn-reenthused/TI99-4A-dc-power-board

I wanted more than a 2a 5v supply, so I spun this up. 

BOM:


--G-Switch SS-22G88-G090 from lcsc.

https://www.lcsc.com/product-detail/C2848925.html

This switch needs to be trimmed to fit, it's a little too long, I just use some flush cutters to trim to size.

--YLPTEC K7805-1000R3 from lcsc.

https://www.lcsc.com/product-detail/C2992391.html


Only substitute with parts that support a negative output. Some buck converts don't have negative output support.

--DFR0831 (Digikey/Mouser/etc)

--TE Connectivity 1-1123723-4 from lcsc.

https://www.lcsc.com/product-detail/C596174.html

--Standard LED round. Your choice of color.
--Either a 560 or 2.2k resistor for the led.

--10uf@25v Caps X3

--25uf@16v Caps X2





This project was made using EasyEDA, because the original version I forked this from was.
I'll eventually move it to kicad.

