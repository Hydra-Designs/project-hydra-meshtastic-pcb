# Project Hydra (Meshtastic PCB)

[![Build Artifacts](https://github.com/PlumRugOfDoom/project-hydra-meshtastic-pcb/actions/workflows/build-release-artifacts.yml/badge.svg)](https://github.com/PlumRugOfDoom/project-hydra-meshtastic-pcb/actions/workflows/build-release-artifacts.yml)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)


A minimalist PCB design built around the Ebyte E22-900M30S 30dbm (1 watt) LoRA radio and the ESP32-WROOM-32U cpu compatible with the [Meshtastic-device](https://github.com/meshtastic/Meshtastic-device) firmware. 

![image](https://user-images.githubusercontent.com/93053584/147958065-cc98ba30-0f0b-4a98-ab02-f6d852b78876.png)

## Features
- Supports up to 30dbm (1 watt) transmit power *(Please check local ISM band regulations for power limitations)*
- OLED support via I2C
- GPS support via UART
- PSRAM support
- User button via pin header
- Switchable 3.3V power rail (GPS power saving)
- ADC input for battery voltage sensing
- Single 5V input (no reverse polarity and overvoltage protection!)
- 3.3V output (or input if onboard buck converter is not assembled)
- Two GPIO reserved for future use (for example power control)
- Programmable via USB-Serial adapter (RTS/DTR are required for the on-board auto reset!)
- Compatible with "meshtastic-diy-v1" target in Meshtastic-device firmware


## Project status
- V2.1 has been published and introduces breaking changes.
- Production file generation has not been verified yet for all variants.
- Core PCB KiCad footprint and schematic symbol will be available afer the official V2 release.

## Ordering from JLCPCB
- Basic ordering instructions can be found at the [ordering page](ordering.md).

## Assembly instructions
- Use the fancy iBom for reference!
- Start with the 3.3v step down regulator and test the 3.3v rail first.
- Assemble all the parts for the auto reset circuit and the ESP32 module. Don't forget to connect the 2.4G antenna!
- Try to program the core pcb next.
- Lastly, populate the RF modem. You can use a strip of cardboard as a spacer to leave a small gap between the two PCBs, in case the ESP32 stops working you can use solder wick to easily remove and reuse the RF modem.
- Never ever turn on the core pcb withount an antenna! This may infuriate the RF gods and you inevitably end up performing a sacrifial ritual to please the RF gods with magic smoke.
- PSRAM is optional

## Contributing

Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a branch, add commits, and [open a pull request](https://github.com/PlumRugOfDoom/project-hydra-meshtastic-pcb/compare/).

## Support

Please [open an issue](https://github.com/PlumRugOfDoom/project-hydra-meshtastic-pcb/issues/new) for support.

## License
[GPL v3](https://choosealicense.com/licenses/gpl-3.0/)

[Meshtastic](https://meshtastic.org/)® is a registered trademark of Geeksville Industries LLC. Meshtastic software components are released under various licenses, see github for details. No warranty is provided - use at your own risk.
