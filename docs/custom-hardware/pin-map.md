# Pin map

All assignments are placeholders and remain blank until the physical wiring is
documented.

## ESP32-S3-DevKitC-1

| GPIO | Function | Connector/pin | Direction | Voltage | Evidence | Status |
|---:|---|---|---|---|---|---|
| TODO | Display SPI SCK | TODO | output | TODO | TODO | unassigned |
| TODO | Display SPI MOSI | TODO | output | TODO | TODO | unassigned |
| TODO | Display SPI MISO | TODO | input | TODO | TODO | unassigned |
| TODO | Display CS | TODO | output | TODO | TODO | unassigned |
| TODO | Display D/C | TODO | output | TODO | TODO | unassigned |
| TODO | Display RESET | TODO | output | TODO | TODO | unassigned |
| TODO | Display backlight | TODO | output/PWM | TODO | TODO | unassigned |
| TODO | Touch interrupt | TODO | input | TODO | TODO | unassigned |
| TODO | Touch bus/pins | TODO | TODO | TODO | TODO | unassigned |
| TODO | Shared SPI SCK | TODO | output | TODO | TODO | unassigned |
| TODO | Shared SPI MOSI | TODO | output | TODO | TODO | unassigned |
| TODO | Shared SPI MISO | TODO | input | TODO | TODO | unassigned |
| TODO | NRF24 CSN 1 | TODO | output | 3.3 V | TODO | unassigned |
| TODO | NRF24 CE 1 | TODO | output | 3.3 V | TODO | unassigned |
| TODO | NRF24 CSN 2 | TODO | output | 3.3 V | TODO | unassigned |
| TODO | NRF24 CE 2 | TODO | output | 3.3 V | TODO | unassigned |
| TODO | NRF24 CSN 3 | TODO | output | 3.3 V | TODO | unassigned |
| TODO | NRF24 CE 3 | TODO | output | 3.3 V | TODO | unassigned |
| TODO | CC1101 CSN | TODO | output | 3.3 V | TODO | unassigned |
| TODO | CC1101 GDO0 | TODO | input/interrupt | TODO | TODO | unassigned |
| TODO | CC1101 GDO2 | TODO | input/interrupt | TODO | TODO | optional |
| TODO | PN532 CS | TODO | output | TODO | TODO | unassigned |
| TODO | PN532 IRQ | TODO | input/interrupt | TODO | TODO | optional |
| TODO | GPS TX/RX | TODO | UART | TODO | TODO | unassigned |
| TODO | GPS PPS | TODO | input | TODO | TODO | optional |
| TODO | LED/buzzer/buttons | TODO | TODO | TODO | TODO | unassigned |

## Constraints to check before selecting GPIOs

- Preserve USB and boot/strapping functions.
- On WROOM-2/octal-flash variants, GPIO35, GPIO36, and GPIO37 are reserved for
  internal flash/PSRAM communication.
- On DevKitC-1 v1.1, GPIO38 drives the onboard RGB LED unless deliberately
  repurposed.
- Confirm that every peripheral's logic voltage is compatible.
- Avoid sharing chip-select, reset, or interrupt lines unintentionally.
