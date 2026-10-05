# Hardware verification report

## Scope and method

This report compares the project photographs with manufacturer documentation,
component datasheets, and the product listings supplied for the purchased radio
modules. A statement is marked **confirmed** only when the evidence directly
supports it. A statement is marked **provisional** when the component family is
known but the particular breakout-board wiring or configuration is not proven.

## Results

### ESP32-S3 controller — confirmed with one configuration caveat

- The rear photograph is marked `ESP32-S3-DevKitC-1 V1.1`.
- The photographed header labels match the Espressif v1.1 header layout when the
  rear-side view is read with its physical orientation taken into account.
- Espressif documents the v1.1 RGB LED on GPIO38.
- Espressif documents GPIO35, GPIO36, and GPIO37 as unavailable for external
  use on boards using octal flash/PSRAM, including WROOM-2 variants.

The board identity and printed labels are confirmed. The exact flash/PSRAM
suffix and the project's final peripheral assignments are not confirmed.

Evidence: [ESP32-S3-DevKitC-1 v1.1 user guide](https://docs.espressif.com/projects/esp-dev-kits/en/latest/esp32s3/esp32-s3-devkitc-1/user_guide_v1.1.html)

### nRF24L01+PA+LNA modules — interface confirmed, breakout order unconfirmed

The Nordic specification confirms the nRF24 control and SPI signals: CE, CSN,
SCK, MOSI, MISO, IRQ, VDD, and VSS. The product listing identifies the three
modules as the same ACEIRMC NRF24L01+PA+LNA model and specifies a 3.0–3.6 V
operating range.

The photographs do not show a readable header legend. The signal names and
electrical limits are therefore confirmed at the radio-interface level, but the
physical left-to-right order on this particular breakout is not confirmed.

Evidence: [nRF24L01+ product specification](https://devzone.nordicsemi.com/cfs-file/__key/communityserver-discussions-components-files/4/content.pdf), [product listing](https://www.amazon.com/dp/B092ZNYLYZ)

### CC1101 module — radio interface confirmed, breakout order unconfirmed

TI confirms the CC1101 four-wire SPI interface (`SI`, `SO`, `SCLK`, and `CSn`)
and the configurable `GDO0`, `GDO1`, and `GDO2` signals. The product listing
identifies the purchased board as a DWEII CC1101 module with SMA antenna.

The photograph does not show readable header labels. The current header table
is a functional reference, not a physical pin-order claim. Continuity testing
or a board-specific schematic is required before wiring.

Evidence: [TI CC1101 datasheet](https://www.ti.com/lit/ds/symlink/cc1101.pdf), [product listing](https://www.amazon.com/dp/B0CSYX1454)

### GPS module — visible labels confirmed, electrical details unconfirmed

The photograph clearly shows a GY-NEO6MV2 / NEO-6M-style board and the header
labels `VCC`, `RX`, `TX`, and `GND`. The photo does not prove the board's supply
tolerance, logic-level behavior, or whether a PPS signal is available.

### PN532 module — visible labels confirmed, interface selection unconfirmed

The photographs clearly show the SPI-side labels `SCK`, `MISO`, `MOSI`, `SS`,
`VCC`, `GND`, `IRQ`, and `RSTO`, plus an interface-selection jumper area. The
photos do not prove the jumper position required for SPI or the electrical
levels of this particular breakout.

### Display — connector labels confirmed, controller identity not photo-proven

The photographs support the documented P2 and long-header labels. The photos
alone do not identify the controller IC or touch controller; ST7796S remains a
product/configuration assumption until confirmed from the display documentation
or by controller-ID probing.

## Work still required

The following items cannot be verified from the current evidence:

1. Physical header order on the nRF24 and CC1101 breakout boards.
2. Final ESP32 GPIO assignments and continuity from each connector.
3. Supply voltage and peak-current behavior with all three PA/LNA radios active.
4. PN532 jumper setting and actual SPI mode.
5. GPS logic levels and PPS availability.
6. Display touch-controller identity and verified ST7796S controller ID.

Until those checks are complete, the pin map and wiring tables should be treated
as design notes rather than a ready-to-build wiring diagram.
