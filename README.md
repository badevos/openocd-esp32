build configuration
===================

On Ubuntu 19.10 the system was configured as follows:

```
sudo apt-get install libusbprog-dev libusb-dev libusb-1.0-0 libusb-0.1-4 libusb-1.0-0-dev libhidapi-dev libhidapi-hidraw0 libhidapi-libusb0 libftdi-dev libftdi1-dev libftdipp1-dev
```

Then it was configured with 'all' the options ...

```
./configure --enable-dependency-tracking --enable-ftdi --enable-stlink --enable-ti-icdi --enable-ulink --enable-usb-blaster-2 --enable-ft232r --enable-vsllink --enable-xds110 --enable-osbdm --enable-opendous --enable-aice --enable-usbprog --enable-rlink --enable-armjtagew --enable-cmsis-dap --enable-kitprog --enable-usb-blaster --enable-presto --enable-openjtag --enable-jlink --enable-jtag_vpi --enable-amtjtagaccel --enable-ep93xx --enable-at91rm9200 --enable-bcm2835gpio --enable-imx_gpio --enable-gw16012 --enable-buspirate --enable-sysfsgpio --enable-remote-bitbang

libjaylink configuration summary:
 - Package version ................ 0.2.0-git-f73ad5e
 - Library version ................ 0:0:0
 - Installation prefix ............ /usr/local
 - Building on .................... x86_64-pc-linux-gnu
 - Building for ................... x86_64-pc-linux-gnu

Enabled transports:
 - USB ............................ yes
 - TCP ............................ yes


OpenOCD configuration summary

MPSSE mode of FTDI based devices        yes
ST-Link Programmer                      yes
TI ICDI JTAG Programmer                 yes
Keil ULINK JTAG Programmer              yes
Altera USB-Blaster II Compatible        yes
Bitbang mode of FT232R based devices    yes
Versaloon-Link JTAG Programmer          yes
TI XDS110 Debug Probe                   yes
OSBDM (JTAG only) Programmer            yes
eStick/opendous JTAG Programmer         yes
Andes JTAG Programmer                   yes
USBProg JTAG Programmer                 yes
Raisonance RLink JTAG Programmer        yes
Olimex ARM-JTAG-EW Programmer           yes
CMSIS-DAP Compliant Debugger            yes
Cypress KitProg Programmer              yes
Altera USB-Blaster Compatible           yes
ASIX Presto Adapter                     yes
OpenJTAG Adapter                        yes
SEGGER J-Link Programmer                yes
```

And then to build/install:

```
make

sudo make install
```
