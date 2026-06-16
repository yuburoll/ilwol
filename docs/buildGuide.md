# Build Guide
this is build guide for ilwol.

the build guide contains build of prototype version. newest version have following differences:

- the corner screws of outside top are moved 1u inside, so do the PCB design.

- lower pinky modifier keys are not changeable. as black marked in prototype PCB

This documents are translated by generative AI, so there can be some misleading texts.

### Additional Resources
[**Soldering Tips**](solderingTip.md)

# PCB Preparation
Prepare two PCBs for the ilwol. Since these are reversible PCBs, be careful to place components on different sides for each board.

The side where components will be placed is treated as the back, and the side without components is treated as the front. **All components go on back side only, so please be careful when soldering.**

![ilwolbuildPCB0](../images/ilwolbuildPCB0.jpg)
![ilwolbuildPCB1](../images/ilwolbuildPCB1.jpg)

# Soldering the Diodes
Solder the diodes. The builds show SMD diodes being used, but THT diodes can also be used.

When using SMD diodes, first apply a solder blob to one side of the pad with a soldering iron, as shown in the following build.

![ilwolbuildDiode0](../images/ilwolbuildDiode0.jpg)

Reheat the solder blob with the iron to melt it, align the diode in the correct orientation and place it in position, then remove the iron.

![ilwolbuildDiode1](../images/ilwolbuildDiode1.jpg)

Once it is seated properly, solder the opposite leg.

![ilwolbuildDiode2](../images/ilwolbuildDiode2.jpg)

# Soldering the Hot-swap Sockets
Solder the hot-swap sockets. The process is largely the same as soldering the diodes and LEDs.

As before, apply a solder blob to one side of the pad, reheat the blob to melt it, place the component and hold it in position, remove the iron, then solder the opposite leg.

![ilwolbuildHotswap0](../images/ilwolbuildHotswap0.jpg)
![ilwolbuildHotswap1](../images/ilwolbuildHotswap1.jpg)

# Soldering the TRRS Jack
Refer to the following builds to identify where the TRRS jack will be placed.

![ilwolbuildJack0](../images/ilwolbuildJack0.jpg)
![ilwolbuildJack1](../images/ilwolbuildJack1.jpg)

Solder the TRRS jack. When soldering the Tip and Sleeve pins, also bridge them to the adjacent pads as shown in the build.

![ilwolbuildJack2](../images/ilwolbuildJack2.jpg)

# Soldering the Dev Board
First, check the header pins on the provided Pro Micro dev board. The outermost row of header pins past 5V is not needed, so trim them off.

![ilwolbuildDevboard0](../images/ilwolbuildDevboard0.jpg)
![ilwolbuildDevboard1](../images/ilwolbuildDevboard1.jpg)

Insert the header pins starting from 5V, align them, and solder the dev board. When soldering, make sure the components face upward as shown in the build.

![ilwolbuildDevboard2](../images/ilwolbuildDevboard2.jpg)
![ilwolbuildDevboard3](../images/ilwolbuildDevboard3.jpg)

Place the dev board with the soldered header pins on top of the already-soldered hot-swap sockets. Press down firmly to ensure a tight fit.

![ilwolbuildDevboard4](../images/ilwolbuildDevboard4.jpg)
![ilwolbuildDevboard5](../images/ilwolbuildDevboard5.jpg)

Just like when soldering the TRRS jack pins, bridge the header pins to the adjacent pads as if soldering jumpers. Since a large amount of solder is used, there is a risk of bridging with flux, so be sure to clean the area with alcohol after soldering.

![ilwolbuildDevboard6](../images/ilwolbuildDevboard6.jpg)

# Soldering the Jumpers
On the front side seen when soldering the dev board, bridge the jumpers located just below. Apply enough solder so that a blob forms on top.

![ilwolbuildJumper0](../images/ilwolbuildJumper0.jpg)
![ilwolbuildJumper1](../images/ilwolbuildJumper1.jpg)

# Check before Assembly
a finished right side of PCB looks like following images. mirror it on the left side.

the build didn't jumped the front jumper, but you may jump there if you building wired version.

![ilwolbuildPCBFinish0](../images/ilwolbuildPCBFinish0.jpg)
![ilwolbuildPCBFinish1](../images/ilwolbuildPCBFinish1.jpg)

# Assembly
First, assemble the case, plate, and switches together. (Note: If you assemble the plate, switches, and PCB first, the assembly will not fit into the case.)
The plate and case are fastened together with screws at four points.

![ilwolbuildAssembly0](../images/ilwolbuildAssembly0.jpg)
![ilwolbuildAssembly1](../images/ilwolbuildAssembly1.jpg)

Insert the protruding part of the TRRS jack into the hole in the case, then lower the PCB onto the switches to mate them together.

![ilwolbuildAssembly2](../images/ilwolbuildAssembly2.jpg)
![ilwolbuildAssembly3](../images/ilwolbuildAssembly3.jpg)

Place the backplate over the case and fasten it with screws at eight points per side to complete the build.

![ilwolbuildAssembly4](../images/ilwolbuildAssembly4.jpg)
