# avr-config

A repository for my most commonly used AVR fuse bit configurations and their plain english descriptions.  The description for each configuration will only describe variations from the default settings.


# ATMega328p - Default high fuse byte.  In low fuse byte, max start up time 16Mhz crystal oscillator with CKDIV8 disabled

avrdude -c usbtiny -p atmega328p -U hfuse:w:0b11011001:m -U lfuse:w:0b11111111:m

# ATTiny2313a - Default high fuse byte.  In low fuse byte, CKDIV8 disabled, max start up time 8Mhz or higher external crystal oscillator
avrdude -c usbtiny -p attiny2313a -U hfuse:w:0b11011111:m -U lfuse:w:0b11111111