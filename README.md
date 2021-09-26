# nhd-2.4-240320CF-raspberry

This repository contains a device tree overlay for a 2.4inch Newhaven Display:
https://www.newhavendisplay.com/nhd24240320cfbsxvf-p-9666.html

The display is driven using SPI. This was tested on a Raspberry Pi 4 Model B, pinout as follows:

| Display Pin | Function | Raspberry Pi Pin | Function |
|-------------|----------|------------------|----------|
| 1           | GND      | 6                |          |
| 2-5         | NC       |                  |          |
| 6           | VDD      | 1                | 3.3V     |
| 7           | IOVDD    | 17               | 3.3V     |
| 8           | MOSI     | 19               |          |
| 9           | MISO     | 21               |          |
| 10          | SCLK     | 23               |          |
| 11          | DC       | 18               | GPIO24   |
| 12          | CS       | 24               |          |
| 13          | RESET    | 16               | GPIO23   |
| 14          | IM0      | Pull Down        |          |
| 15          | IM1      | Pull Up          |          |
| 16-19       | LEDK1-4  | Backlight        |          |
| 20          | LEDA     | Backlight        |          |

The compiled DTBO was tested on kernel Linux raspberrypi 5.10.60-v7l+ #1449 SMP Wed Aug 25 15:00:44 BST 2021 armv7l GNU/Linux

