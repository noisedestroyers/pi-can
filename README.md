# PI-CAN

Raspberry PI trials with Microchip CAN<->SPI

Enable SPI on PI & detail CAN clock speed and PI interrupt input pin:
/boot/config.txt:

#dtparam=audio=on
dtparam=spi=on
dtoverlay=mcp2515-can0-overlay,oscillator=8000000,interrupt=25
dtoverlay=spi-bcm2835-overlay


Resources:

PI 2 Pinout:
http://www.raspberrypi-spy.co.uk/wp-content/uploads/2014/07/Raspberry-Pi-GPIO-Layout-Model-B-Plus-rotated.png

PI SPI Info
https://www.raspberrypi.org/documentation/hardware/raspberrypi/spi/README.md

Device Trees, Overlays, parameters:
https://www.raspberrypi.org/documentation/configuration/device-tree.md

Wiring PI & GPIO Utility
http://wiringpi.com/reference/spi-library/
http://wiringpi.com/the-gpio-utility/

BusPirate SPI Sniffer & Pinout & SPI Guide
http://dangerousprototypes.com/docs/Bus_Pirate_binary_SPI_sniffer_utility#Downloads
http://dangerousprototypes.com/docs/images/1/1b/Bp-pin-cable-color.png
http://dangerousprototypes.com/bus-pirate-manual/bus-pirate-spi-guide/



py-spidev:
https://github.com/doceme/py-spidev

PI Forums CAN Thread:
https://www.raspberrypi.org/forums/viewtopic.php?f=44&t=7027&start=125

Similar chipset in prebuilt pi kit:
http://skpang.co.uk/blog/archives/1165
http://skpang.co.uk/catalog/images/raspberrypi/addon/pican_rev_B.pdf

SocketCAN utilities:
http://elinux.org/Can-utils

SocketCanD CAN -> RawTCP
https://github.com/dschanoeh/socketcand/blob/master/doc/protocol.md

Youtuber:
https://www.youtube.com/watch?v=sLitCqj6S1w

CLI CAN Debugging:
https://www.ridgerun.com/developer/wiki/index.php/How_to_configure_and_use_CAN_bus#Enable_socketcan_and_ip_tools

Higher Level Tools:
http://kayak.2codeornot2code.org/
http://sourceforge.net/projects/cantools/
https://github.com/julietkilo/CANBabel

CANARD & CANTACT HW & SW
https://github.com/ericevenchick/canard
https://github.com/linklayer

http://lnxpps.de/rpie/
http://elinux.org/RPi_CANBus
http://www.cowfishstudios.com/blog/canned-pi-part1
