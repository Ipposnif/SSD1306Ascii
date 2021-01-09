The SSD1306Ascii is a very good library, well structured and occupies little space.
I learnt a lot about characters rendering from it, so big thanks to the author.
This fork is to fit the library to my ongoing personal project, but the changes could be useful to other people that need to show multiple screens of properties.

1. The reverse mask, for double size characters, has been replaced with a normal mask char with a line at the bottom. Used for screen titles.
2. \[ char produces a 1 pixel separator
3. ] char produces a 4 pixels separator
4. ^ char feeds the line with empty separators
5. some replaced chars, for the battery icon, don't want a separator
6. double size chars don't have automatically a double size separator
7. the SH1106 (1.3 inches) screen seems to like 9V pump

##################################################################

Note: Version 1.2.x has several new examples and many changes/new features.

SSD1306Ascii is an unbuffered character only library for small OLED
displays like the Adafruit 1.3" and 0.96" Monochrome displays.

Many low cost OLED displays with SSD1306 controllers are available on ebay.

SSD1306Ascii runs on Arduino AVR boards, Arduino Due and many other
Arduino style boards that have the SPI or Wire library.

Please read the html documentation in the SSD1306Ascii/doc folder.

Several options can be set by editing SSD1306Ascii/src/SSD1306Ascii.h.

The SSD1306Ascii library only requires a few bytes of RAM.

Here is Uno memory use for the SPI "Hello world!" example with
scrolling disabled:

Sketch uses 2928 bytes (9%) of program storage space. Maximum is 32256 bytes.

Global variables use 54 bytes (2%) of dynamic memory, leaving 1994 bytes for local variables. Maximum is 2048 bytes.







