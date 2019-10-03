# Ender-5/SKR Pro v1.1/TMC5160 Config Files

This repository contains Marlin custom config files for Creality Ender-5 printers with a BIGTREETECH SKR Pro v1.1 motherboard and TMC5169 drivers.

**Updated on 2019-10-23.**



## Installation guide for Printers with BL Touch 3.1

1. Get the latest Marlin bugfix-2.0.x from the official site here: http://marlinfw.org/meta/download/.
2. Copy files from folder **\Config_BLTouch31\Config_Files** in this repository to the folder **\Marlin** in your firmware root folder.
4. Copy files from folder **\Config_BLTouch31\Compiler_Settings** in this repository to the your firmware root folder.
5. **If you Marlin source files are older than 6 Sep, 2019** copy files from folder **\CR10_Display_Fix** in this repository to the folder **\Marlin\src\lcd\dogm** in your firmware root folder (fixes [BUG] #15113 on latest Marlin bugfix-2.0.x, please view links section for more details).
6. Compile the software and flash the board.
7. **Optional:** Do a "Restore failsafe" from the printer's menu or delete file EEPROM.DAT from the SD Card before powering on to make sure that the printer is running with the default values and avoid malfunction.
8. 

## Installation guide for Printers without BL Touch

1. Get the latest Marlin bugfix-2.0.x from the official site here: http://marlinfw.org/meta/download/.

2. Copy files from folder **\Config_BLTouch31\Config_Files** in this repository to the folder **\Marlin** in your firmware root folder.

3. Copy files from folder **\Config_BLTouch31\Compiler_Settings** in this repository to the your firmware root folder.

4. **If you Marlin source files are older than 2019-09-06** copy files from folder **\CR10_Display_Fix** in this repository to the folder **\Marlin\src\lcd\dogm** in your firmware root folder (fixes [BUG] #15113 on latest Marlin bugfix-2.0.x, please view links section for more details).

5. Compile the software and flash the board.

6. **Optional:** Do a "Restore failsafe" from the printer's menu or delete file EEPROM.DAT from the SD Card before powering on to make sure that the printer is running with the default values and avoid malfunction.

   

## Links

SKR Pro V1.1 Github page: https://github.com/bigtreetech/BIGTREETECH-SKR-PRO-V1.1

Marlin bugfix-2.0.x: http://marlinfw.org/meta/download/

Marlin Github repository: https://github.com/MarlinFirmware/Marlin

[BUG] #15113 breaks CR10_STOCKDISPLAY support on SKR Mini E3: https://github.com/MarlinFirmware/Marlin/issues/15141 - **Fixed on 2019-09-05, commit 2ef2d56566**

BIGTREETECH SKR Pro User Group on FB: https://www.facebook.com/groups/2264108593625228/



## Technical information

| Item                 | Detail/description                                           |
| -------------------- | ------------------------------------------------------------ |
| Printer              | Creality Ender-5                                             |
| Board                | BIGTREETECH SKR Pro v1.1                                     |
| Display              | Stock Ender-5 display (LCD 12864)                            |
| ABL                  | BL Touch 3.1                                                 |
| Original file source | Ender-5 example config files bundled with Marlin bugfix-2.0.x tree, commit 72a6a6028c, 2019-10-03 |

