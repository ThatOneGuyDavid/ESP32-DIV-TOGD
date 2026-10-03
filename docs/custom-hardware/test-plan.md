# Bring-up test plan

Run tests in this order and record date, firmware commit, wiring revision, and
result. Do not enable or test radio-disruption features outside equipment,
networks, and frequencies where you have explicit authorization and local rules
permit the activity.

1. **Power-only:** confirm regulated rails and current draw.
2. **Serial boot:** confirm stable reset and readable startup logs.
3. **Display:** initialize the ST7796S panel; verify orientation, colors, and
   touch-controller identification.
4. **Touch:** verify all corners and calibration persistence.
5. **Storage:** mount and read/write the SD card, if present.
6. **Input:** verify every button or I/O-expander input.
7. **LED/buzzer:** verify outputs without disturbing shared buses.
8. **SPI isolation:** test the display, each NRF24, CC1101, and PN532 separately.
9. **GPS:** verify UART reception and a valid fix outdoors.
10. **NFC:** verify PN532 detection and a test tag you own.
11. **Integrated idle:** run the UI with all peripherals connected.
12. **Authorized feature tests:** test only permitted functions, one subsystem at a
    time, and record failures.

## Test record

| Date | Firmware commit | Wiring revision | Test | Result | Notes |
|---|---|---|---|---|---|
| TODO | TODO | TODO | TODO | TODO | TODO |
