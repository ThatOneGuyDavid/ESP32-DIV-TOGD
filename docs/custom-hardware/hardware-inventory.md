# Hardware inventory

This inventory records identified parts, interfaces, and verification status.

| Subsystem | Part | Interface | Status |
|---|---|---|---|
| MCU | ESP32-S3-DevKitC-1 V1.1, ESP32-S3-WROOM-2 | USB, GPIO | Rear silkscreen photographed; exact N16R8 suffix: **TODO** |
| Display | Hosyond 4.0-inch 320x480 TN capacitive LCD | SPI | Connector labels confirmed; controller/touch IDs: **TODO** |
| 2.4 GHz radio 1 | ACEIRMC NRF24L01+PA+LNA | SPI | Same module as radios 2 and 3; header order: **TODO** |
| 2.4 GHz radio 2 | ACEIRMC NRF24L01+PA+LNA | SPI | Same module as radios 1 and 3; header order: **TODO** |
| 2.4 GHz radio 3 | ACEIRMC NRF24L01+PA+LNA | SPI | Same module as radios 1 and 2; header order: **TODO** |
| Sub-GHz radio | DWEII CC1101 with SMA antenna | SPI | 433 MHz purchase; header order/GDO wiring: **TODO** |
| GPS | GY-NEO6MV2 NEO-6M | UART | Logic levels and PPS use: **TODO** |
| NFC/RFID | PN532 V3 | SPI | Interface jumpers and IRQ/reset: **TODO** |

## Evidence to add

- [ ] Photograph of each module, front and back
- [ ] Display product link or controller/touch-controller marking
- [ ] ESP32 module shield marking, including any suffix after N16R8
- [ ] Schematic or hand-drawn wiring diagram
- [ ] Power-rail measurements under radio transmit load
- [ ] Confirmed GPIO numbers from continuity tests
