# Hardware inventory

This is a working inventory, not a final schematic. Add exact part markings,
links, voltage information, and evidence as they become available.

| Subsystem | Part | Interface | Status |
|---|---|---|---|
| MCU | ESP32-S3-DevKitC-1-N16R8 | USB, GPIO | Exact module suffix/voltage: **TODO** |
| Display | Hosyond 4.0-inch 320x480 TN capacitive LCD | SPI | ST7796S confirmed; touch controller: **TODO** |
| 2.4 GHz radio 1 | NRF24L01+PA+LNA | SPI | Exact module revision: **TODO** |
| 2.4 GHz radio 2 | NRF24L01+PA+LNA | SPI | Exact module revision: **TODO** |
| 2.4 GHz radio 3 | NRF24L01+PA+LNA | SPI | Exact module revision: **TODO** |
| Sub-GHz radio | CC1101 with SMA antenna | SPI | 433 MHz; GDO wiring: **TODO** |
| GPS | GY-NEO6MV2 NEO-6M | UART | Logic levels and PPS use: **TODO** |
| NFC/RFID | PN532 V3 | SPI | Interface jumpers and IRQ/reset: **TODO** |

## Evidence to add

- [ ] Photograph of each module, front and back
- [ ] Display product link or controller/touch-controller marking
- [ ] ESP32 module shield marking, including any suffix after N16R8
- [ ] Schematic or hand-drawn wiring diagram
- [ ] Power-rail measurements under radio transmit load
- [ ] Confirmed GPIO numbers from continuity tests
