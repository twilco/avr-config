# avr-config

A repository for my most commonly used AVR fusebit configurations and their plain english descriptions.

# Default high fuse byte, max start up time 16Mhz crystal oscillator with no CKDIV8 and CKOUT disabled (so CLKO pin behaves normally)

avrdude -c usbtiny -p atmega328p -U hfuse:w:0b11011001:m -U lfuse:w:0b11111111:m