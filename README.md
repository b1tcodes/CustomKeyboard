# CustomKeyboard V1

A 65% hand-wired mechanical keyboard with Mac-optimized layout.

## Specifications

| Feature | Value |
|---------|-------|
| Layout | 65% (68 keys) |
| MCU | Arduino Pro Micro or Elite-C |
| Mounting | O-ring gasket |
| Connectivity | USB-C |
| Firmware | QMK/VIA |
| Dimensions | 312 × 110 × 30mm |
| Assembly | Hand-wired |

## Features

- Mac layout with Command/Option keys
- Hand-wired matrix construction
- VIA support for keymap configuration
- Cross-platform compatibility (macOS, Windows, Linux)
- 3D printed case

## Cost Estimate

| Component | Price (USD) |
|-----------|-------------|
| Arduino Pro Micro / Elite-C | $5-20 |
| Diodes 1N4148 (100 pack) | $3 |
| Wire (solid core 22-24 AWG) | $8 |
| MX switches (68) | $35-70 |
| Keycaps | $40-100 |
| Case (3D printed) | $20 |
| Stabilizers | $8 |
| Hardware (screws, O-ring) | $5 |

**Total:** $124-234

## Repository Structure
```
CustomKeyboard/
├── hardware/
│   ├── plate/         # Plate design files (DXF/SVG)
│   ├── case/          # CAD models (STEP/STL)
│   └── wiring-diagram.png
├── firmware/
│   └── qmk/           # QMK configuration
└── docs/              # Build documentation
```

## Hand-Wiring Process

1. 3D print or laser cut switch plate
2. Install switches into plate
3. Wire matrix (rows and columns)
4. Solder diodes to switches
5. Connect matrix to microcontroller
6. Flash firmware and test
7. Install in case

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
└────┴────┴────┴────────────────────────┴────┴──────┴───┴───┴───┘
```

## Acknowledgments

Based on <a href="https://github.com/kkatano/bakeneko-60/tree/develop">Bakeneko60 by kkatano</a>.
