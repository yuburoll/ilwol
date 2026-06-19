# Build Guide
this is build guide for ilwol.

the build guide contains photo of prototype version. newest version have following differences:

- the corner screws of outside top are moved 1u inside, so do the PCB design.

- lower pinky modifier keys are not changeable. as black marked in prototype PCB

This documents are translated by generative AI, so there can be some misleading texts.

### Additional Resources
[**Soldering Tips**](solderingTip.md)

# PCB Preparation
Prepare two PCBs for the ilwol. Since these are reversible PCBs, be careful to place components on different sides for each board.

The side where components will be placed is treated as the back, and the side without components is treated as the front. **All components go on back side only, so please be careful when soldering.**

![ilwolPCBway2](../images/ilwolPCBway2.jpg)

# Soldering the Diodes
Solder the diodes. The photos show SMD diodes being used, but THT diodes can also be used.

In the photo, the hot-swap sockets are soldered first, but I recommend soldering the diodes first.

When using SMD diodes, first apply a solder blob to one side of the pad with a soldering iron, as shown in the following photos.

![ilwolBuildDiodes1](../images/ilwolBuildDiodes1.jpg)
![ilwolBuildDiode2](../images/ilwolBuildDiodes2.jpg)

Reheat the solder blob with the iron to melt it, align the diode in the correct orientation and place it in position, then remove the iron.

![ilwolBuildDiode3](../images/ilwolBuildDiodes3.jpg)

Once it is seated properly, solder the opposite leg.

![ilwolBuildDiode4](../images/ilwolBuildDiodes4.jpg)

# Soldering the Hot-swap Sockets
Solder the hot-swap sockets. The process is largely the same as soldering the diodes and LEDs.

As before, apply a solder blob to one side of the pad, reheat the blob to melt it, place the component and hold it in position, remove the iron, then solder the opposite leg.

![ilwolBuildSocket2](../images/ilwolBuildSocket2.jpg)
![ilwolBuildSocket4](../images/ilwolBuildSocket3.jpg)

# Soldering the TRRS Jack and the Jumper
Refer to the following photos to identify where the TRRS jack will be placed. The jack will be placed on back side, so you may solder that on front side.

![ilwolBuildJack1](../images/ilwolBuildJack1.jpg)
![ilwolBuildJack2](../images/ilwolBuildJack2.jpg)

Solder the TRRS jack. When soldering the Tip and Sleeve pins, also bridge them to the adjacent pads as shown in the photo.

And, On the front side seen when soldering the jack, bridge the jumpers located aside. Apply enough solder so that a blob forms on top.

![ilwolBuildJack3](../images/ilwolBuildJack3.jpg)

# Soldering the Dev Board
First, check the header pins on the provided Pro Micro dev board. The outermost row of header pins past 5V is not needed, so trim them off.

![BuildBoard0](../images/BuildBoard0.jpg)
![BuildBoard1](../images/BuildBoard1.jpg)

Insert the header pins starting from 5V, align them, and solder the dev board. When soldering, make sure the components face upward as shown in the photo.

![BuildBoard2](../images/BuildBoard2.jpg)
![BuildBoard3](../images/BuildBoard3.jpg)

Place the dev board with the soldered header pins on top of the already-soldered hot-swap sockets. Press down firmly to ensure a tight fit.

![ilwolBuildBoard1](../images/ilwolBuildBoard1.jpg)
![ilwolBuildBoard2](../images/ilwolBuildBoard2.jpg)

Just like when soldering the TRRS jack pins, bridge the header pins to the adjacent pads as if soldering jumpers. Since a large amount of solder is used, there is a risk of bridging with flux, so be sure to clean the area with alcohol after soldering.

![ilwolBuildBoard4](../images/ilwolBuildBoard3.jpg)

# Check PCB and flash firmware before Assembly
The finished PCBs looks like a following image.

![ilwolBuildAssembly](../images/ilwolBuildAssembly.jpg)

If you're a keyboard enthusiast, I'd recommend installing stabilizers at keycap positions 2u or larger, as shown in the following photo.

![ilwolBuildStabilizer](../images/ilwolBuildStabilizer.jpg)

Also, please flash the firmware before assembling the case.

For the RP2040 promicro, hold down the Boot button on the development board while connecting the USB, then drop the .uf2 file onto the removable disk that appears.

For the ATmega32U4 promicro, load the firmware .hex in your flashing tool (e.g., QMK Toolbox). Then, with the USB connected, briefly short RST and GND with a conductor, or solder a 4x4x1.5mm tactile switch to those pads and press it. The Caterina bootloader will activate and the tool will flash the firmware.

# Assembly
First, assemble plate and switches together with proper direction, and assemble PCB on it.

![ilwolBuildKeyswitches1](../images/ilwolBuildKeyswitches1.jpg)
![ilwolBuildKeyswitches2](../images/ilwolBuildKeyswitches2.jpg)

Place the plate assembly over the case and fasten it with screws at eight points per side to complete the build. also, you may add four bumpons on the bottom of the case.

![ilwolBuildFinish1](../images/ilwolBuildFinish1.jpg)
![ilwolBuildFinish2](../images/ilwolBuildFinish2.jpg)
