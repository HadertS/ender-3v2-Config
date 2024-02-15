# Ender 3v2 Configuration files
Configuration files for my heavily modified Ender 3v2 3D printer - Currently running MainsailOS and Klipper. This is an ongoing project I've been tweaking for a while now, I'm primarily documenting this for my own reference but other people may find some of the information presented here useful for configuring their own machine (particularly the printer.cfg configurations).

## Modifications
This started life as a stock Ender kit but has since been heavily modded with the following:

- [Squash Ball Feet](https://www.thingiverse.com/thing:4809869) - to dampen vibrations, improving print quality.
- Stock fans replaced with Noctua Silent Fans, powered via step down Buck converters - reduces vibration output significantly but requires stepping down the stock 24v to the 12v thats the Noctua use.
- Ender 3 Briss fang Gen2 - Replaced stock hotend shroud.
- CR Touch - Installed for automated bed levelling, replacing a previously installed BL Touch due to build quality issues.
- Solid Silicone Bed Mounts - Replacing Yellow Spring Bed Mounts for increased replicability of auto bed levelling, which themselves replaced the stock spring bed mounts.
- Raspery Pi Web Host running MainsailOS and Klipper firmware - replacing a previous Octoprint/Octopi setup to enable advanced functionality not present in the Octopi firmware whilst also allowing remote management.
- Sunlu S2 Filament Dryer - replacing a similar Sunlu S1 due to improved performance, allowing for more reliable extursion by eliminating moisture.
- [Electronics relocated to an exterior enclosure](https://www.thingiverse.com/thing:4742032).
- All wiring re-terminated with crimped ferrules - for increased fire safety over stock tinned wires.
- All Metal Microswiss Hotend - a drop in replacement for the stock hotend, specifically replaced to counter the hotend to bowden tube gap in the stock hotend causing clogs.
- Micro Swiss Direct Drive - for improved retraction responsiveness over a non-stock all metal bowden extruder, which itself replaced the original plastic bowden extruder which has a known design flaw.
- Creality Dual Z Axis Upgrade - Installed to counteract z axis sag that was being exacerbated by the increased gantry.
- 3 Point Bed - Installed as I was struggling to get a 4 point bed level.
- Frame Brace - My frame was getting a lot of wiggle in the Y direction, I installed CR-10 style bracing rods to counteract some of this without increasing the tightness of the current bolts as I am concerned about warping the extrusions.
- Replaced Bed Base Aluminium extrusion - The extrusion in the middle of the H shaped base had become very warped due to the way it was cut out no longer being actively supported by the old electronics cases. I suspect that this part was always warped, but it had been significantly worsened due to overtightening of the frame bolts. 
- Magnetic PEI plate - much better for adhesion, meaning I can use a higher Z offset which leads to less stringing and print failure.


## Removed Modifications
- Carborundum Glass Bed - I was having to much trouble with adhesion, might go back to it eventually for certain materials.


## Future Plans
- Replace the hotend shroud with something smaller, lighter and with as small a Z offset as possible, preferably with a dual blower. I've fallen out of love with the Briss fang design due to the weight of the gantry increasing after installing the direct drive. This will also involve re-wiring one of the noctua fans and replacing it dual blowers.
- Replaced Bed Base Aluminium extrusion with a solid one with no cut outs to increase strength. These are no longer necessary due to the exterior electronics, but I don't currently have access to a drill press with suitable taps to put in new bolts so a stock replacement will have to do for now.
- Tidy up wiring harness and shield it - both to make it look nicer and for increased durability. Currently my wiring harness is open to the elements as I tinker with it, but once this is done it would be good to sort this out. This will probably also involve replacing some of the shorter cables as currently everything is kind of tight.


## Calibration
I use the Teaching Tech [Calibration Guide](https://teachingtechyt.github.io/calibration.html) although some adjustment must be made for Klipper specific GCode.
