# USB1.1 Host Controller packaged for Xilinx IP

This is a fork of [core_usb_host](https://github.com/ultraembedded/core_usb_host), with some customizations and fixes.


## Differences between this and upstream repo

1. AXI4-Lite address and data no longer need to arrive in the same cycle
2. Support 60MHz utmi clock instead of 48MHz
3. Fix RX and TX IFS logic where IFS should be counted after EOP is sent by PHY
4. Add new CTRL2 register(address 0x24) to control phy reset
5. Use XPM FIFO to match timing requirements, thus only Xilinx Vivado is supported now


## License

Licensed under GPLv3.
