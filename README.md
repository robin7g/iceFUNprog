This code is adapted from the main repo but made to work on MacOS. This code was tested on M1 Mac running Ventura 13.2.1 The main code branch segmentation faults on MacOS due to serial device not being found and then file close() function being called on a null file descripter. 

# iceFUNprog
Programmer for Devantech iCE40 modules, iceFUN and iceWerx

To build and install the programmer:

    $ make install


To program the module:

    $ iceFUNprog blinky.bin

Note: in case the programmer doesn't seem to do anything, make sure you are not accidentally
running software which tries to use your device as a modem 
(e.g. [ModemManager](https://www.freedesktop.org/wiki/Software/ModemManager/)) as this 
interferes with this programmer.
