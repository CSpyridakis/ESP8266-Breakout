# ESP8266-Breakout ![MIT license](https://img.shields.io/github/license/CSpyridakis/ESP8266-Breakout?style=plastic) ![Size](https://img.shields.io/github/repo-size/CSpyridakis/ESP8266-Breakout?style=plastic)

A breadboard-friendly ESP12E/F breakout with all I/O pins available, flash/reset buttons onboard, and place to directly use it with FTDI modules like [FT232RL FTDI Serial Adapter Module](https://www.banggood.com/FT232RL-FTDI-USB-To-TTL-Serial-Converter-Adapter-Module-p-917226.html?rmmds=buy&cur_warehouse=CN).

![ESP-Breakout-Breadboard](doc/ESP8266-Breakout-Breadboard.jpg)

### Schematic
![Schematic](doc/schematic.png)

|Top View             |  Bottom View              |
|:-------------------:|:-------------------------:|
| ![Top](doc/top.png) | ![Bottom](doc/bottom.png) |

### Sample
![PCB](doc/ESP8266-Breakout.jpg)

## Assembly 
| No  |   Component   |    Quantity      |
|:---:|:-------------:|:----------------:|
| 1.  |      ESP8266 - 12e/f         | 1 | 
| 2.  |    10KΩ 0805 smd resistors   | 5 | 
| 3.  |      SMD-SWITCH-6.2MM        | 2 |
| 4.  | Pin Header 1x11 Male 2.54 mm | 2 |

### Notes
* If you want to power up ESP8266-Breakout directly from a FTDI board, you need to solder the jumper that exists on the bottom side of the ESP8266-Breakout. **IMPORTANT:** Do not forget to change the jumper to 3.3V instead of 5V, on the FTDI module.
* If you want to use ESP8266-Breakout with a breadboard.
  - Connect Vcc to 3.3V
  - Connect Gn to Ground
  - You do not need to connect EN pin (ESP8266-Breakout itself has the required connection)
  - You do not need to add any extra pull-up or pull-down resistors on GPIO15, GPIO2 or GPIO0 for Boot Mode Selection

## PCB CAD tool
This project was developed using free version of  [EAGLE 9.5.2](https://www.autodesk.com/products/eagle/overview)

Gerber files are available [here](pcb/gerber/)
