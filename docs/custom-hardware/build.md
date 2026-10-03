# Build notes

This is a placeholder for the custom-board build procedure. Keep the upstream
firmware build steps recognizable and document only deviations here.

## Toolchain

- Arduino IDE or CLI version: **TODO**
- ESP32 board package version: **TODO**
- Selected board definition: **TODO**
- Partition scheme: **TODO**
- Upload speed: **TODO**
- Required libraries: **TODO**

## Configuration changes

The expected customization points are:

- `ESP32-DIV/BoardConfig.h`
- `ESP32-DIV/shared.h`
- `ESP32-DIV/config.h`
- Any display-driver or touch-driver setup required by the ST7796S module

Do not place a guessed pin map directly into feature files. Record the final
values in the custom board section first, then update the smallest upstream
configuration point that consumes them.

## Build commands

```text
# TODO: add exact commands after the board profile is confirmed
```

## Flashing and recovery

- Boot-button sequence: **TODO**
- Serial port identification: **TODO**
- Erase-flash requirement: **TODO**
- First-boot serial baud: **TODO**
- Recovery procedure: **TODO**
