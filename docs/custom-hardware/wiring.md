# Wiring notes

This is the human-readable wiring guide. Keep it synchronized with
[pin-map.md](pin-map.md) and the schematic.

## Power

- MCU board supply: **TODO**
- Display supply and logic level: **TODO**
- NRF24 PA/LNA supply arrangement for three modules: **TODO**
- CC1101 supply: **TODO**
- GPS supply: **TODO**
- PN532 supply and logic level: **TODO**
- Common ground topology: **TODO**
- Decoupling capacitors and regulator ratings: **TODO**

Do not power radio modules from an unverified rail. Measure the rail while the
highest-load transmitter is active.

## Bus topology

The intended shared SPI devices are the display, three NRF24 modules, CC1101,
and PN532. Confirm whether the display or any module requires a separate SPI
host, bus speed, mode, or transaction wrapper.

- SPI host(s): **TODO**
- SPI mode per device: **TODO**
- Maximum tested bus speed: **TODO**
- Per-device chip-select behavior: **TODO**

The NEO-6M is expected to use a UART, but its actual wiring and logic levels
must be recorded before connection.

## Physical assembly

- Board mounting: **TODO**
- Antenna clearance: **TODO**
- Cable lengths and shielding: **TODO**
- Touchscreen mounting/orientation: **TODO**
- Access to USB and boot controls: **TODO**
