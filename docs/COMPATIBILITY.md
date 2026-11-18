# Printer & filament compatibility

MythaPrism exports a **.3mf project** (with per-layer filament changes or per-part colors) plus an STL + swap list for
any other workflow. It has been developed and test-printed primarily on Bambu Lab machines with an AMS.

## Printers with a built-in profile
| Printer | Notes |
|---|---|
| Bambu Lab **H2C**, **H2D**, **X2D** | dual-nozzle: colors are split across both nozzles automatically, 0.2 / 0.4 / 0.6 mm nozzles |
| Bambu Lab **X1 / X1 Carbon**, **P1S / P1P**, **A1 / A1 mini** | AMS or manual swaps, 0.4 mm (0.2 / 0.6 where supported) |
| Prusa **XL** (5 toolheads), **CORE One** | via OrcaSlicer-family profiles |
| Snapmaker **U1**, Snapmaker Orca | single-extruder machines: use a One color per layer matcher or manual swaps |
| FlashForge Creator 5 | tool changer |
| **Generic** 180 / 220 / 256 / 300 / 350 mm beds | any slicer that opens 3MF. Set your own printer and process |

Relief/zoned prints place many colors side by side within a layer and **need a multi-material system** (AMS or
similar). Printers without one should use a One color per layer matcher, which never puts two colors in the same layer.

## Filaments
The built-in library starts with Bambu Lab PLA Basic and Matte colors. Any filament can be
added by name and hex color, a **calibration plate** export (Tool: filament library · App: Colors sheet) prints a
plate of your own filaments so the tool can read how they really print. Notes from the community welcome. Open a
"Share a print result" issue with the filament brand, color and what you saw.

## Slicers
Bambu Studio is the reference, OrcaSlicer opens the same projects. Other slicers get the STL + swap list.

