# EuroBusboard

A Eurorack bus board with 8 module connectors for distributing ±12V, +5V, gate, and CV signals. Multiple connector variants are available in the project.

## Variants

The KiCad project contains several connector configurations:

| Variant | Files | Notes |
|---|---|---|
| 16-pin IDC | `EuroBusboard.kicad_pcb` | The "standard" Doepfer 16-pin Eurorack IDC pinout |
| 10-pin IDC, 8 outputs | `eurobusboard_idc_8.kicad_pcb` | Without CV/Gate buses |
| 10-pin IDC + JST, 8 outputs | `eurobusboard_idc_jst_8.kicad_pcb` | Mixed connector types |
| JST, 8 outputs | `eurobusboard_jst_8.kicad_pcb` | JST-only |

## Schematic

- Latest: **Rev 0.1** — [PDF](Schematic%20PDFs/EuroBusboard-Schematic-rev0.1.pdf)

## Hardware

- KiCad project: [kicad/](kicad/)
- See also the 16-pin variant in a separate repo: [EuroBusboard-8-IDC-16PIN](https://github.com/DIYSynthMNL/EuroBusboard-8-IDC-16PIN) *(private)*

## Pinout (Doepfer 16-pin standard)

Looking at the connector with the keyway up:

```
GATE   -12V  -12V  ...
CV     +12V  +12V  ...
+5V    GND   GND   ...
```

`-12V` is always pointed down when looking at the board (Eurorack convention).

## Build status

What's available for builders, and what's still on the TODO list:

- [x] Schematic PDF (Rev 0.1) — [EuroBusboard-Schematic-rev0.1.pdf](Schematic%20PDFs/EuroBusboard-Schematic-rev0.1.pdf)
- [x] KiCad source files — [kicad/](kicad/)
- [ ] Gerber files for PCB fabrication — *not yet exported — generate from kicad/ before sending to a fab*
- [ ] Bill of materials (BOM) — *bus boards are simple — see schematic for the parts list*
- [ ] Photos of an assembled board — *not yet*
- [x] License — [LICENSE](LICENSE)
