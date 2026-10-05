# Controller board details

The controller is an **ESP32-S3-DevKitC-1 V1.1** development board. The
rear silkscreen is the clearest source for the header labels in the photos.
The rear photo is shown with the USB connectors at the left; because this is
the reverse side of the board, do not compare its top and bottom edges to a
front-side drawing without accounting for that orientation.

> **Controller rear reference** — Rear silkscreen and header labels. The
> printed labels are evidence of the board marking, not yet the project's
> final peripheral assignments.
>
> ![ESP32-S3-DevKitC-1 rear](images/controller/controller-back.jpg)

> **Controller front reference** — ESP32-S3 module, USB connectors, buttons,
> and status hardware.
>
> ![ESP32-S3-DevKitC-1 front](images/controller/controller-front.jpg)

## Observed rear header labels

| Header edge in the rear photo | Labels, left to right |
|---|---|
| Upper edge | GND, GND, GPIO19, GPIO20, GPIO21, GPIO47, GPIO48, GPIO45, GPIO0, GPIO35, GPIO36, GPIO37, GPIO38, GPIO39, GPIO40, GPIO41, GPIO42, GPIO2, GPIO1, RX, TX, GND |
| Lower edge | GND, 5V, GPIO14, GPIO13, GPIO12, GPIO11, GPIO10, GPIO9, GPIO46, GPIO3, GPIO8, GPIO18, GPIO17, GPIO16, GPIO15, GPIO7, GPIO6, GPIO5, GPIO4, RST, 3V3, 3V3 |

These labels should be cross-checked against the official board documentation
and continuity measurements before they are used in firmware.
