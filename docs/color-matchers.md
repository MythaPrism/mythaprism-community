# Color matchers

A color matcher decides which filament goes where and how many layers each part of the picture gets. Different matchers plan the layers in different ways, so the same photo can come out with a different look. Try a few and keep the one you like.

<img src="../assets/color_matchers.jpg" width="100%">

<sub>One NASA photo of Earth matched by different color matchers (real screen captures). NASA does not endorse MythaPrism.</sub>

## The families

- **Black and white.** The free plan's matcher, in a smooth style or a halftone style, with black and white filament.
- **Each color used once.** Every filament appears once in the stack, from the bottom up. Simple to print and easy on filament changes.
- **Colors may repeat.** A filament can come back higher in the stack, which gives richer color at the cost of more changes.
- **Zoned.** Different parts of the picture get their own stacks. Made for printers with several spools loaded at once, such as an AMS.
- **Full spectrum printing (beta).** Mixes cyan, magenta, yellow, black and white into the colors of the picture, the way a magazine prints a photo with a few inks.
- **LithoPrism.** Plans a lithophane for light coming through the print.

Which matchers you get depends on your plan, and the [prices page](https://mythaprism.com/#pricing) lists every one. The color match menu shows them grouped by family.

## Calibration

On Plus and Pro you can print a calibration plate, take a photo of it, and let MythaPrism read the real colors your printer and your spools make. The preview then shows those colors, and the layer plan uses them. The photo of the plate is read on your device.

## Two rules every matcher keeps

- **Black hides what is under it.** One thin layer of black covers everything below it, so black is planned as a top color or as a base under other colors, never as a see-through layer.
- **Your spools, not a palette.** A matcher only uses the filaments you turned on in the library, and it never picks a specialty filament such as silk or marble for you.
