[![licensebuttons by-nc-sa](https://licensebuttons.net/l/by-nc-sa/3.0/88x31.png)](https://creativecommons.org/licenses/by-nc-sa/4.0)

## FunKey S Hardware
This repository contains all the hardware design and production files required to build the [FunKey-S retro-gaming console](https://www.funkey-project.com/) electronic PCBA using the [KiCAD ECAD tools](https://kicad.org/).

If you don't want to install these tools but still want to get an idea of what it looks like, you can check the [schematics](https://github.com/FunKey-Project/FunKey-S-Hardware/blob/master/PDF/FunKey%20Schematics.pdf) and the [layout](https://github.com/FunKey-Project/FunKey-S-Hardware/blob/master/PDF/FunKey%20PCB.pdf) in PDF format, the interactive [BOM](https://github.com/FunKey-Project/FunKey-S-Hardware/tree/master/BOM) is directly in HTML format, you can download it and display it in a browser.

The FunKey S is a small foldable retro-gaming console.

Its electronic parts consist in:
 - 1x main PCB (0.8 mm thickness) with components on both sides, the maximum component height above PCB on both sides is 1.5 mm. Current revision for this board is Revision E
 - 1x 1.54” IPS LCD TFT screen with SPI interface and using a custom flex cable
 - 1x 420 mAh 402540 LiPo battery

![FunKey S Block Diagram](https://github.com/FunKey-Project/FunKey-S-Hardware/raw/master/Pictures/FunKey%20S%20Block%20Diagram.png)

The FunKey S PCBA Rev. E contains the following main components:
 - 1x Allwinner V3s SoC with integrated 64MB DDR2 DRAM (LQFP128 package)
 - 1x X-Powers AXP209 companion PMIC chip to provide almost all required power supply rails (QFN48 package)
 - 1x Sylergy SY8088 Buck DC/DC SMPS chip to provide the DRAM power supply rail (SOT23-5 package)
 - 1x NXP PCAL6416 I2C GPIO expander to control all buttons and keypads (except Power Key) (QFN24 package)
 - 1x Diodes Inc. PAM8301 mono audio amplifier (TSOT26 package)
 - 1x 24 MHz main crystal
 - 1x 32.768 kHz RTC crystal
 - 1x Standex-Meder MK24 Reed switch for magnet proximity detection
 - 1x LED for charge indication
 - 1x 8 Ω 0.3 W built-in speaker
 - 1x Micro USB edge-mounted connector
 - 1x Micro SD (TF Card) Push/Push low-profile connector
 - 1x Hirose DF37 0.4 mm pitch miniature LCD connector
 - 1x JST 1 mm pitch battery connector
 - 1x 1.27 mm pitch debug UART header (not mounted)

![FunKey Top](https://github.com/FunKey-Project/FunKey-S-Hardware/raw/master/Pictures/FunKey%20S%20Top.png)

![FunKey Bottom](https://github.com/FunKey-Project/FunKey-S-Hardware/raw/master/Pictures/FunKey%20S%20Bottom.png)
