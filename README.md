# avr-config

A repository for my most commonly used AVR fusebit configurations and their plain english descriptions.

#### Default high fuse byte, max start up time 8-16Mhz low power (not full swing) crystal oscillator with CKDIV8 and CKOUT disabled

avrdude -c usbtiny -p atmega328p -U hfuse:w:0b11011001:m -U lfuse:w:0b11111111:m
