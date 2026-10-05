# Custom hardware notes

This directory records the hardware adaptation for **ESP32-DIV-TOGD**.
It intentionally follows the upstream repository layout: firmware remains under
`ESP32-DIV/`, while board-specific notes live here.

No pin assignment is considered final until it is confirmed from the module
documentation, physical wiring, and a successful hardware test. Replace each
`TODO` with evidence as the build progresses.

## Current hardware inventory

- Controller: Espressif ESP32-S3-DevKitC-1, marked N16R8 (exact suffix to verify)
- Display: Hosyond 4.0-inch 320x480 TN capacitive SPI LCD, ST7796S controller
- 2.4 GHz radios: three NRF24L01+PA+LNA modules
- Sub-GHz radio: one CC1101 module with SMA antenna, 433 MHz
- GPS: one GY-NEO6MV2 NEO-6M module with ceramic antenna
- NFC/RFID: one PN532 V3 module configured for SPI

## Documents

- [Hardware inventory](hardware-inventory.md)
- [Display details and pinouts](display.md)
- [GPS module details](gps.md)
- [PN532 module details](pn532.md)
- [Pin map](pin-map.md)
- [Wiring notes](wiring.md)
- [Build notes](build.md)
- [Bring-up test plan](test-plan.md)
- [Local photo workflow](local-media-workflow.md)

The firmware files and upstream directory names are intentionally left in their
original locations so upstream documentation remains easy to follow.
