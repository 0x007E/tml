[![Version: 1.0 Release](https://img.shields.io/badge/Version-1.0%20Release-green.svg)](https://github.com/0x007e/tml) ![Build](https://github.com/0x007e/tml/actions/workflows/release.yml/badge.svg) [![License CC By-NC-SA](https://img.shields.io/badge/Hardware-CC--BY--NC--SA--4.0-lightgrey)](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode)

# `TML` - Temperature Logger

The `TML` is a board with an [LM386](#additional-information) that is used to scale up a temperature (0°-100°) from [KT200](#additional-information). The temperature gets A/D converted over an [ATtiny1606](#additional-information) and is stored in an eeprom [AT24CM0X](#additional-information) with current time and date that is provided by a [MCP7940](#additional-information) r(eal)-t(ime)-c(lock). The board itself provides a reverse polarity protection and can be supplied between `9-12V`. The voltage is line regulated to `5V`.

| Experience | Level |
|:------------|:-----:|
| Soldering   | ![?%](https://progress-bar.xyz/55?progress_color=00ff00&suffix=%20Medium&width=120) |

# Downloads

| Type      | File               | Description              |
|:---------:|:------------------:|:-------------------------|
| Schematic | [pdf](https://github.com/0x007E/tml/releases/latest/download/schematic.pdf) / [cadlab](https://cadlab.io/project/30575/main/files) | Schematic files |
| Board | [pdf](https://github.com/0x007E/tml/releases/latest/download/pcb.pdf) / [cadlab](https://cadlab.io/project/30575/main/files) | Board file |
| Drill | [pdf](https://github.com/0x007E/tml/releases/latest/download/drill.pdf) | Drill file |
| BoM | [xlsx](https://github.com/0x007E/tml/releases/latest/download/bom.xlsx) / [html](https://github.com/0x007E/tml/releases/latest/download/ibom.html)          | Bill of Material as Excel/interactive HTML |
| PCB    | [zip](https://github.com/0x007E/tml/releases/latest/download/kicad.zip) / [tar](https://github.com/0x007E/tml/releases/latest/download/kicad.tar.gz)    | KiCAD/Gerber/BoM/Drill files       |

# Hardware

The pcb is created with `KiCAD`. All files are built with `github actions` so that they are ready for a production environment.

## PCB

The circuit board is populated on both sides (Top, Bottom). The best way for soldering the `SMD` components is within a vapor phase soldering system and for the `THT` components with a standard soldering system.

### Top Layer

![Top Layer](https://github.com/0x007E/tml/releases/latest/download/top.kicad.png)

### Bottom Layer

![Bottom Layer](https://github.com/0x007E/tml/releases/latest/download/bottom.kicad.png)

# Additional Information

| Type  | Link                                                | Description                                   |
|:------|:---------------------------------------------------:|:----------------------------------------------|
| LM358 | [pdf](https://www.ti.com/lit/ds/symlink/lm358b.pdf) | Industry-Standard Dual Operational Amplifiers |
| KT200 | [pdf](https://rocelec.widen.net/view/pdf/qxp2nqwwr1/INFNS04262-1.pdf?t.download=true&u=5oefqw) | Silicon Temperature Sensors |
| ATtiny1606 | [pdf](https://ww1.microchip.com/downloads/en/DeviceDoc/ATtiny804-06-07-1604-06-07-DataSheet-DS40002312A.pdf) | tinyAVR® 0-series |
| AT24CM01 | [pdf](https://ww1.microchip.com/downloads/en/DeviceDoc/AT24CM01-I2C-Compatible-Two-Wire-Serial-EEPROM-Data-Sheet-20006170A.pdf) | I²C-Compatible (Two-Wire) Serial EEPROM 1‑Mbit (131,072 x 8) |
| AT24CM02 | [pdf](https://ww1.microchip.com/downloads/en/DeviceDoc/I%C2%B2C-Compatible-(Two-Wire)-Serial-EEPROM-2-Mbit-(262,144x8)-20006197B.pdf) | I²C-Compatible (Two-Wire) Serial EEPROM 2‑Mbit (262,144 x 8) |
| MCP7940 | [pdf](https://ww1.microchip.com/downloads/en/DeviceDoc/MCP7940M-Low-Cost%20I2C-RTCC-with-SRAM-20002292C.pdf) | Low-Cost I2C Real-Time Clock/Calendar with SRAM |

---

R. GAECHTER
