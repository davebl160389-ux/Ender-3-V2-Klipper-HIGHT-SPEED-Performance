# Ender 3 V2 - High Speed Performance Config

This Klipper configuration is optimized for a modified Ender 3 V2. The goal is maximum performance and reliability at significantly increased print speeds.

## Hardware Requirements
To use this config, the following setup (or similar) is required:
- Sprite Pro Extruder (or similar Direct Drive)
- ADXL345 Input Shaper for resonance calibration
- Dual 5015 part cooling fans for sufficient cooling at high speeds

## Important Notes
- **Speed & Accel:** The values in the `printer.cfg` (e.g., 7000 mm/s² acceleration) require perfectly adjusted mechanical stability and tight belts.
- **No Copy-Paste Guarantee:** The PID values, Z-offset, and Input Shaper values in my config are specific to my printer.
- **Mandatory Calibration:** After copying the files, you must perform the following steps:
  1. `PID_CALIBRATE` for hotend and bed.
  2. `PROBE_CALIBRATE` for your Z-offset.
  3. `SHAPER_CALIBRATE` with your ADXL345.

## Installation
Copy all files from this repository into your Klipper config folder on your Raspberry Pi / Host. Ensure that your `printer.cfg` correctly includes the other files using the `[include ...]` directive.

---

# Ender 3 V2 - High Speed Performance Config

Diese Klipper-Konfiguration ist für einen modifizierten Ender 3 V2 optimiert. Das Ziel ist maximale Performance und Zuverlässigkeit bei deutlich erhöhten Druckgeschwindigkeiten.

## Hardware-Voraussetzungen
Für die Nutzung dieser Config ist folgendes Setup (oder vergleichbar) erforderlich:
- Sprite Pro Extruder (oder ähnlicher Direct Drive)
- ADXL345 Input Shaper zur Resonanzkalibrierung
- Dual 5015 Bauteillüfter für ausreichend Kühlung bei Speed

## Wichtige Hinweise
- **Speed & Accel:** Die Werte in der `printer.cfg` (z.B. 7000 mm/s² Beschleunigung) setzen eine perfekt eingestellte mechanische Stabilität und straffe Riemen voraus.
- **Keine Copy-Paste-Garantie:** Die PID-Werte, das Z-Offset und die Input-Shaper-Werte aus meiner Config sind spezifisch für meinen Drucker. 
- **Pflicht-Kalibrierung:** Führe nach dem Kopieren zwingend folgende Schritte aus:
  1. `PID_CALIBRATE` für Hotend und Bett.
  2. `PROBE_CALIBRATE` für dein Z-Offset.
  3. `SHAPER_CALIBRATE` mit deinem ADXL345.

## Installation
Kopiere alle Dateien aus diesem Repository in deinen Klipper-Config-Ordner auf dem Raspberry Pi / Host. Achte darauf, dass deine `printer.cfg` die anderen Dateien via `[include ...]` korrekt einbindet.
