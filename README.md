# Ender-5/SKR Pro v1.1/TMC5160 Config Files

This repository contains Marlin custom config files for Creality Ender-5 printers with a BIGTREETECH SKR Pro v1.1 motherboard and TMC5169 drivers.

**Updated on 2019-10-04.**



## Installation guide for Printers with BL Touch 3.1

1. Get the latest Marlin bugfix-2.0.x from the official site here: http://marlinfw.org/meta/download/.
2. Copy files from folder **\Config_BLTouch31\Config_Files** in this repository to the folder **\Marlin** in your firmware root folder.
4. Copy files from folder **\Config_BLTouch31\Compiler_Settings** in this repository to the your firmware root folder.
6. Compile the software and flash the board.
5. **Optional:** Do a "Restore failsafe" from the printer's menu to make sure that the printer is running with the default values and avoid malfunction.

   

## Installation guide for Printers without BL Touch

1. Get the latest Marlin bugfix-2.0.x from the official site here: http://marlinfw.org/meta/download/.

2. Copy files from folder **\Config_BLTouch31\Config_Files** in this repository to the folder **\Marlin** in your firmware root folder.

3. Copy files from folder **\Config_BLTouch31\Compiler_Settings** in this repository to the your firmware root folder.

5. Compile the software and flash the board.

6. **Optional:** Do a "Restore failsafe" from the printer's menu to make sure that the printer is running with the default values and avoid malfunction.

   

## Links

SKR Pro V1.1 Github page: https://github.com/bigtreetech/BIGTREETECH-SKR-PRO-V1.1

Marlin bugfix-2.0.x: http://marlinfw.org/meta/download/

Marlin Github repository: https://github.com/MarlinFirmware/Marlin

BIGTREETECH SKR Pro User Group on FB: https://www.facebook.com/groups/2264108593625228/



## Technical information

| Item                 | Detail/description                                           |
| -------------------- | ------------------------------------------------------------ |
| Printer              | Creality Ender-5                                             |
| Board                | BIGTREETECH SKR Pro v1.1                                     |
| Display              | Stock Ender-5 display (LCD 12864)                            |
| ABL                  | BL Touch 3.1                                                 |
| Original file source | Ender-5 example config files bundled with Marlin bugfix-2.0.x tree, commit 511cd6d6c5, 2019-10-04 |

