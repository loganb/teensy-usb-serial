Introduction
==============

This is a repo of the USB Serial code for the Teensy microcontroller code from http://www.pjrc.com/teensy/usb_serial.html. It was forked at version 1.7 and contains (or will soon contain) some small improvements to make it easier to use from within an event loop. 


How to use in a Teensy project
---------------------

Check out this repo into a sub-folder of your Teensy project (e.g. usb_serial/...)
Edit the SRC line of your Makefile to include usb_serial.c, e.g.:

    SRC = $(TARGET).c \
          usb_serial/usb_serial.c

When including usb_serial.h in your source files, qualify it with the path to the sub-folder, e.g.:

    #include "usb_serial/usb_serial.h"

