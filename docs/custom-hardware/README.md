# Custom hardware notes

This directory contains the hardware adaptation notes for **ESP32-DIV-TOGD**.
Firmware remains under `ESP32-DIV/`; board-specific documentation is collected
here.

Pin assignments remain provisional until confirmed by module documentation,
physical wiring, and hardware testing.

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
- [Controller board details](controller.md)
- [nRF24 radio details](nrf24.md)
- [CC1101 radio details](cc1101.md)
- [GPS module details](gps.md)
- [PN532 module details](pn532.md)
- [Pin map](pin-map.md)
- [Wiring notes](wiring.md)
- [Build notes](build.md)
- [Bring-up test plan](test-plan.md)
- [Hardware verification report](verification-report.md)
- [Local photo workflow](local-media-workflow.md)
