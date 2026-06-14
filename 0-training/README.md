# Training Ender‑3 V3 SE

## Specifications

| Parameter | Value |
|-----------|-------|
| Printing technology | Fused deposition modeling |
| Build volume | 220 × 220 × 250 mm |
| Typical printing speed | 180 mm/s |
| Max. printing speed | 250 mm/s (CR-PLA test) |
| Acceleration | 2500 mm/s² |
| Printing accuracy | ±0.1 mm |
| Layer height | 0.1–0.35 mm |
| Extruder type | "Sprite" direct extruder |
| Leveling mode | Auto leveling |
| Build surface | PC spring steel |
| Nozzle temperature | ≤260 °C |
| Heatbed temperature | ≤100 °C |
| Mainboard | 32-bit silent mainboard |
| Display | 3.2" color knob screen |
| Power loss recovery | Yes |
| Default nozzle diameter | 0.4 mm |
| Extruder count | 1 |
| Rated voltage | 100–120 V~ / 200–240 V~, 50/60 Hz |
| Rated power | 350 W |
| File transfer | SD card |
| Supported filaments | PLA, PETG, TPU (95A) |
| Slicing file formats | STL, OBJ, 3MF, AMF |
| Slicing software | Creality Print, Cura 5.0+, Simplify3D |

## Power Consumption Calculation

Energy consumed is calculated as:

$$
E = P \times t
$$

where `E` is energy in kWh, `P` is power in kW, and `t` is time in hours.

Cost is calculated as:

$$
\text{Cost} = E \times \text{Rate}
$$

Rates used for calculation:

- Daytime: 8.24 RUB/kWh
- Nighttime: 3.54 RUB/kWh

At rated power (350 W = 0.35 kW), energy per hour:

$$
E_{1h} = 0.35 \times 1 = 0.35 \text{ kWh}
$$

Hourly cost at full rated load:

| Tariff | Calculation | Cost per hour |
|--------|-------------|---------------|
| Daytime | 0.35 × 8.24 | **2.88 RUB/h** |
| Nighttime | 0.35 × 3.54 | **1.24 RUB/h** |

Actual consumption is usually below 350 W (heating peaks, then lower during steady printing). Use these values as an upper-bound estimate.

## Printer Shutdown

### Daily Use

After a print completes, let the printer cool down. Switch off the rear power switch only when the nozzle is below ~100 °C and the bed below ~50 °C (per the display). No software shutdown is required.

Do not cut power while the nozzle is still hot (200+ °C) with fans off — this risks heat creep and filament charring in the hotend.

### Long-Term Storage

- Retract and remove filament from the hotend

