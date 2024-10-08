# AGBSUBS1-01
This KiCAD PCB project aims to recreate the original AGBSUBS1-01 sub board meant for the original AGB 64M (E201843), 128M (E201850) and 256M (E201868) dev cartridges by Nintendo. Do note however, that it is not meant to be a 1:1 copy of the original PCB.

The board supports the following save types:
- 4kbit EEPROM
-  64kbit EEPROM
-  256kbit SRAM (via FRAM chip)
-  512kbit Flash
-  1Mbit Flash

## Ordering PCBs
A ready-to-manufacture set of Gerber files can found [here](https://github.com/Infinest/AGB-64M_SUB_BOARD/blob/master/Gerbers/AGB-64M_SUB_BOARD.zip).

### Important:
Make sure to order your PCBs with a thickness of 0.6mm or they may not fit into the cartridge.
For ease of soldering any fine-pitched components (like J1) ENIG as surface finish is recommended.

## BOM:

| Reference        | Part Number           | Description  |
| ------------- |:-------------:| -----:|
| R1, R2 | RC0201FR-0710KL (or equivalent) | 10K Ω resistor 0201 (0603 metric)|
| C1, C2, C3 | GRM033R60J104KE19D (or equivalent) | 0.1µF capacitor 0201 (0603 metric)|
| U1 | FM18W08-SG | 256kbit FRAM |
| U2 | MX29L010TC-15A1 or LE26FV10N1TS / SST39VF512 or SST39LF512 | 1Mbit Flash / 512kbit Flash  |
| U3 | 9854 / 9853 | 64kbit EEPROM / 4kbit EEPROM |
| J1 | AXK640347YG | Mezzanine connector |

### Note:
Per PCB only populate **ONE** of **U1**, **U2** or **U3**
- **R2** & **C2** should be added if U1 is being populated
- **R2** & **C3** should be added if U2 is being populated
- **R1** & **C1** should be added if U3 is being populated

## Examples
### 256kbit FRAM
![256kbit FRAM](https://github.com/user-attachments/assets/4cbfdd6e-4b26-457d-aa48-7760831ff34c)

### 64kbit EEPROM
![64kbit EEPROM](https://github.com/user-attachments/assets/2f8d01d3-4738-4193-8362-844d08df43ea)

### 1Mbit Flash
![1Mbit Flash](https://github.com/user-attachments/assets/e8c5cdcb-ef92-4572-ab72-89716537650f)

## Additional Images:
![image](https://github.com/user-attachments/assets/cd2af5ca-4d19-4341-b3be-2f40a7177c52)
![image](https://github.com/user-attachments/assets/9eddde3b-7e0f-47f6-b761-730c7dc2c732)
![image](https://github.com/user-attachments/assets/64a42905-85e4-4eb6-8df6-f808e537269a)
