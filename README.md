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

# CustomKeyboard V1

A 65% hand-wired mechanical keyboard with Mac-optimized layout.

## Specifications

| Feature       | Value                  |
|---------------|------------------------|
| Layout        | 65% (68 keys)          |
| MCU           | Arduino Pro Micro      |
| Connectivity  | USB-C                  |
| Firmware      | QMK                    |
| Assembly      | Hand-wired             |


## Features

- Mac layout with Command/Option keys
- Hand-wired matrix construction
- QMK support for keymap configuration
- Cross-platform compatibility (macOS, Windows, Linux)
- 3D printed case and plate

## Cost Estimate (Prices may vary)

| Component | Price (USD) |
|-----------|-------------|
| Arduino Pro Micro USB-C | $11 |
| Diodes 1N4148 (68 pcs) | $3.5 |
| Wire (~3m, solid core) | $2 |
| MX switches (68 pcs) | $20.5 |
| Keycaps (68 pcs) | $14 |
| Case (3D printed) | $8 |
| Switch plate (3D printed) | $4 |
| Stabilizers (4–5 pcs) | $2 |
| USB-C cable | $2 |
| Hardware (screws, standoffs, O-ring) | $1.5 |

**Total:** ~$70

## Repository Structure
```
CustomKeyboard V1/
├── hardware/
│   ├── plate.dxf
│   ├── CaseAndPlate3DModel.f3d
├── firmware/
│   └── qmk/
├── img/
│   ├── CustomKeyboard3DModel.png
│   ├── CustomKeyboardRender.png
│   ├── CustomKeyboardDesign.png
│   └── WiringDiagram.png
├── JOURNAL.md
├── README.md
└── bom.csv
```

## Hand-Wiring Process

1. 3D print or laser cut switch plate
2. Install switches into plate
3. Wire matrix (rows and columns)
4. Solder diodes to switches
5. Connect matrix to microcontroller
6. Flash firmware and test
7. Install in case
