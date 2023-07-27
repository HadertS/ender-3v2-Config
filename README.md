# Ender 3v2 Configuration files
Configuration files for my heavily modified Ender 3v2 3D printer - Currently running MainsailOS and Klipper. This is an ongoing project I've been tweaking for a while now

## Modifications
This started life as a stock Ender kit but has since been heavily modded with the following:

- [Squash Ball Feet](https://www.thingiverse.com/thing:4809869) - to dampen vibrations, improving print quality.
- Stock fans replaced with Noctua Silent Fans, powered via step down Buck converters - reduces vibration output significantly but requires stepping down the stock 24v to the 12v thats the Noctua use.
- CR Touch - Installed for automated bed levelling, replacing a previously installed BL Touch due to build quality issues.
- Solid Silicone Bed Mounts - Replacing Yellow Spring Bed Mounts for increased replicability of auto bed levelling, which themselves replaced the stock spring bed mounts.
- Carborundum Glass Bed - Allows for good adhesion and a mirror smooth finish on the base of prints.
- Raspery Pi Web Host running MainsailOS and Klipper firmware - replacing a previous Octoprint/Octopi setup to enable advanced functionality not present in the Octopi firmware whilst also allowing remote management.
- Sunlu S2 Filament Dryer - replacing a similar Sunlu S1 due to improved performance, allowing for more reliable extursion by eliminating moisture.
- [Electronics relocated to an exterior enclosure](https://www.thingiverse.com/thing:4742032).
- All wiring re-terminated with crimped ferrules - for increased fire safety over stock tinned wires.
- All Metal Microswiss Hotend - a drop in replacement for the stock hotend, specifically replaced to counter the hotend to bowden tube gap in the stock hotend causing clogs.
- Micro Swiss Direct Drive - for improved retraction responsiveness over a non-stock all metal bowden extruder, which itself replaced the original plastic bowden extruder which has a known design flaw.
- Creality Dual Z Axis Upgrade - Installed to counteract z axis sag that was being exacerbated by the increased gantry.
