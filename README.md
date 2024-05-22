# Ender 3v2 Configuration files
Configuration files for my heavily modified Ender 3v2 3D printer - Currently running MainsailOS and Klipper. This is an ongoing project I've been tweaking for a while now, I'm primarily documenting this for my own reference but other people may find some of the information presented here useful for configuring their own machine (particularly the printer.cfg configurations).

## Modifications
This started life as a stock Ender kit but has since been heavily modded with the following:

- Stock fans replaced with Noctua Silent Fans, powered via step down Buck converters - reduces vibration output significantly but requires stepping down the stock 24v to the 12v that the Noctua use.
- CR Touch - Installed for automated bed levelling, replacing a previously installed BL Touch due to build quality issues.
- Solid Silicone Bed Mounts - Replacing Yellow Spring Bed Mounts for increased replicability of auto bed levelling, which themselves replaced the stock spring bed mounts.
- Raspery Pi Web Host running MainsailOS and Klipper firmware - replacing a previous Octoprint/Octopi setup to enable advanced functionality not present in the Octopi firmware whilst also allowing remote management.
- Sunlu S2 Filament Dryer - replacing a similar Sunlu S1 due to improved performance, allowing for more reliable extursion by eliminating moisture.
- [Electronics relocated to an exterior enclosure](https://www.thingiverse.com/thing:4742032).
- All wiring re-terminated with crimped ferrules - for increased fire safety over stock tinned wires.
- Creality Dual Z Axis Upgrade - Installed to counteract z axis sag that was being exacerbated by the increased gantry.
- 3 Point Bed - Installed as I was struggling to get a 4 point bed level. Recently, I have cut this down to allow for a larger stepper motor on the Y axis, which may cause issues down the line, but we will see. 
- Frame Brace - My frame was getting a lot of wiggle in the Y direction, I installed CR-10 style bracing rods to counteract some of this without increasing the tightness of the current bolts as I am concerned about warping the extrusions.
- Replaced Bed Base Aluminium extrusion - The extrusion in the middle of the H shaped base had become very warped due to the way it was cut out no longer being actively supported by the old electronics cases. I suspect that this part was always warped, but it had been significantly worsened due to overtightening of the frame bolts.
- Magnetic PEI plate - much better for adhesion, meaning I can use a higher Z offset which leads to less stringing and print failure.
- Replaced the stock Y stepper with non-pancake creality 42-40 for more torque as the original motor was missing steps due to overheating after changing a broken timing belt. This necessatated cutting down the 3 point bed base and one of the levelling nobs to fit the larger profile, which may be an issue in the long term, but so far is not causing any issues.
- Creality Sprite Pro - replaced the microswiss system as I was having issues with stripping the tiny choke screw and wanted something that was easier to maintain. So far this seems far superior for my purposes as has been much more reliable, although I have had to rewire the ribbon cable due to stress damage (this seems to be a design flaw/cut corners on creality's part) and the part cooling airflow is much worse.
- Mainboard changed to BTT E3 SKR MINI V3.0 to allow for pressure advance which has led to massive speed and quality gains.
- [KUSBA-PRO](https://github.com/xbst/KUSBA-PRO) - Used for resonance compensation, which has contributed to massive speed and quality gains.

## Removed Modifications
- Carborundum Glass Bed - I was having to much trouble with adhesion, might go back to it eventually for certain materials.
- All Metal Microswiss Hotend - a drop in replacement for the stock hotend, specifically replaced to counter the hotend to bowden tube gap in the stock hotend causing clogs.Removed as I had issues with the tiny choke screw getting stripped and heat damaged and wanted something with easier maintainence
- Micro Swiss Direct Drive - surplus to requirements witht the sprite.
- Ender 3 Briss fang Gen2 - Removed as I wanted something that allowed for easier maintainence.
- [Squash Ball Feet](https://www.thingiverse.com/thing:4809869) - removed to increase stability. 

## Future Plans
- Replaced Bed Base Aluminium extrusion with a solid one with no cut outs to increase strength. These are no longer necessary due to the exterior electronics, but I don't currently have access to a drill press with suitable taps to put in new bolts so a stock replacement will have to do for now.
- Upgrade the the Sprite Pro fan system to increase airflow.
- Change mainboard to one that allows for seperate Z control.

## Calibration
I now use the [Klipper calibration documentation](https://www.klipper3d.org/Installation.html) for everything. 
