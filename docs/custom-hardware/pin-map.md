# Pin map

All assignments are placeholders. Do not copy the values below into firmware;
they are intentionally blank until the physical wiring is documented.

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
- Confirm flash/PSRAM-reserved pins for the exact ESP32-S3 module.
- Confirm whether any onboard RGB LED uses a candidate pin.
- Confirm that every peripheral's logic voltage is compatible.
- Avoid sharing chip-select, reset, or interrupt lines unintentionally.
