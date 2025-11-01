# CustomKeyboard V1

A 65% mechanical keyboard with Mac-optimized layout.

## Specifications

| Feature | Value |
|---------|-------|
| Layout | 65% (68 keys) |
| MCU | ATmega32U4 |
| Mounting | O-ring gasket |
| Connectivity | USB-C |
| Firmware | QMK/VIA |
| Dimensions | 312 × 110 × 30mm |
| PCB | 2-layer, 1.6mm |

## Features

- Mac layout with Command/Option keys
- Hotswap sockets for MX switches
- VIA support for keymap configuration
- Cross-platform compatibility (macOS, Windows, Linux)
- Aluminum or 3D printed case options

## Repository Structure
```
CustomKeyboard/
├── hardware/
│   ├── pcb/           # KiCAD files
│   ├── case/          # CAD models (STEP/STL)
│   └── bom.csv        # Bill of materials
├── firmware/
│   └── qmk/           # QMK configuration
└── docs/              # Build documentation
```

### PCB Manufacturing
1. Export Gerber files from KiCAD
2. Upload to JLCPCB or PCBWay
3. Specify: 1.6mm thickness, HASL finish

## Layout
```
┌───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───┬───────┬───┐
│Esc│ 1 │ 2 │ 3 │ 4 │ 5 │ 6 │ 7 │ 8 │ 9 │ 0 │ - │ = │ Bkspc │Del│
├───┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─────┼───┤
│ Tab │ Q │ W │ E │ R │ T │ Y │ U │ I │ O │ P │ [ │ ] │  \  │PgU│
├─────┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴┬──┴─────┼───┤
│ Caps │ A │ S │ D │ F │ G │ H │ J │ K │ L │ ; │ ' │  Enter │PgD│
├──────┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴─┬─┴────┬───┼───┤
│ Shift  │ Z │ X │ C │ V │ B │ N │ M │ , │ . │ / │Shift │ ↑ │End│
├────┬───┴┬──┴─┬─┴───┴───┴───┴───┴───┴──┬┴───┼───┴──┬───┼───┼───┤
│Ctrl│Opt │Cmd │        Space           │Cmd │Fn    │ ← │ ↓ │ → │
└────┴────┴────┴────────────────────────┴────┴──────└───┴───┴───┘
```

## Acknowledgments

Based on <a href="https://github.com/kkatano/bakeneko-60/tree/develop">Bakeneko60 by kkatano</a>.
