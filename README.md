# Ender-5/SKR Pro v1.1/TMC5160 Config Files

This repository contains Marlin custom config files for Creality Ender-5 printers with a BIGTREETECH SKR Pro v1.1 motherboard and TMC5169 drivers.   Settings used are also compatible with **Ender-3** and **Ender-3 Pro**, just be sure to use the correct config examples for your printer. For more information about which settings to change please browse to the config folder in this repository and read the readme.md files.

Features:

- Stock Ender-5/Ender-3/Ender-3 Pro LCD 12864 support.

- BL Touch 3.x support (connected to dedicated on board port).

- I2C EEPROM support.

- TMC5160 with SPI communication for X, Y, Z and E0.

- Automatically controlled extruder fan with auto-start at 50º C (connected to FAN2, pin PE6).

- Works with Octoprint.

  

**Updated on 2019-12-17**



## Installation guide for Printers with BL Touch 3.1

1. Get the latest Marlin bugfix-2.0.x from the official site here: http://marlinfw.org/meta/download/.

2. Copy files from folder **\Config_BLTouch31\Config_Files** in this repository to the folder **\Marlin** in your firmware root folder.

3. Copy files from folder **\Config_BLTouch31\Compiler_Settings** in this repository to the your firmware root folder.

4. Copy files from folder **\Config_BLTouch31\Pins_Files** in this repository to the folder **\Marlin\src\pins\stm32** in your firmware root folder.

5. Compile the software and flash the board.

6. **Optional (add I2C EEPROM support):** Edit **\Marlin\src\pins\stm32\pins_BTT_SKR_PRO_V1_1.h** in your firmware root folder and append the text from file that matches your EEPROM size: **\I2C_EEPROM\I2C_4K_EEPROM.h** or **\I2C_EEPROM\I2C_32K_EEPROM.h**.

7. **Optional (applies to users with I2C EEPROM installed):** Do a "Restore failsafe" from the printer's menu to make sure that the printer is running with the default values and avoid malfunction.

   

## Installation guide for Printers without BL Touch

1. Get the latest Marlin bugfix-2.0.x from the official site here: http://marlinfw.org/meta/download/.
2. Copy files from folder **\Config_Standard\Config_Files** in this repository to the folder **\Marlin** in your firmware root folder.
3. Copy files from folder **\Config_Standard\Compiler_Settings** in this repository to the your firmware root folder.
4. Copy files from folder **\Config_Standard\Pins_Files** in this repository to the folder **\Marlin\src\pins\stm32** in your firmware root folder.
5. Compile the software and flash the board.
6. **Optional (add I2C EEPROM support):** Edit **\Marlin\src\pins\stm32\pins_BTT_SKR_PRO_V1_1.h** in your firmware root folder and append the text from file that matches your EEPROM size: **\I2C_EEPROM\I2C_4K_EEPROM.h** or **\I2C_EEPROM\I2C_32K_EEPROM.h**.
7. **Optional (applies to users with I2C EEPROM installed):** Do a "Restore failsafe" from the printer's menu to make sure that the printer is running with the default values and avoid malfunction. 



## Connecting BL Touch to dedicated on-board header

Below is a picture showing where to connect BL Touch to use the dedicated on-board header. This not required but it leaves both Z end stops ports available if you want to repurpose it. In this case you also need to **follow** **step 3** from the **Installation guide for Printers with BL Touch 3.1**. 

Please note that the on-board header has only 4 pins and that the brown (or blue on some BL Touch kits from Creality) wire (Servo GND) from BL Touch cable **is not connected**.  Also make sure sure that BL Touch it is configured in **open drain mode**. 



![](https://i.imgur.com/qnmc4Bd.jpg)





## Connecting an I2C EEPROM

Below is a picture showing where to connect an I2C EEPROM if you wish to save your printer settings in permanent storage.

<img src="https://i.imgur.com/UJ8KCGU.jpg" style="zoom:50%;" />

## Links

SKR Pro V1.1 Github page: https://github.com/bigtreetech/BIGTREETECH-SKR-PRO-V1.1

Marlin bugfix-2.0.x: http://marlinfw.org/meta/download/

Marlin Github repository: https://github.com/MarlinFirmware/Marlin

BIGTREETECH SKR Pro User Group on FB: https://www.facebook.com/groups/2264108593625228/

Octoprint download page: https://octoprint.org/download/



## Technical information

| Item                 | Detail/description                                           |
| -------------------- | ------------------------------------------------------------ |
| Printer              | Creality Ender-5 (settings also compatible with Ender-3 and Ender-3 Pro using the correct config file examples from Marlin 2.0.x) |
| Board                | BIGTREETECH SKR Pro v1.1                                     |
| Display              | Stock Ender-5 display (LCD 12864)                            |
| ABL                  | BL Touch 3.1                                                 |
| Original file source | Ender-5 example config files bundled with Marlin bugfix-2.0.x tree, commit 2434f0e8ef, 2019-12-17 |

