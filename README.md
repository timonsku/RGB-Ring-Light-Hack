# RGB-Ring-Light-Hack
Info and material to hack common RGB(W) ring lights with your own controller

The hack adds a Raspberry Pi Pico into the original case of the controller with some side cutter modifications and a backpack PCB that adds buttons and mosfets to control the cold and warm white LEDs.

This is based on a RGB ring light that you can buy from AliExpress, Ebay, Amazon etc.
The generic term is "10 Inch RGB Ring Light" or "10 Inch RGB Beauty Light"
The case hack that you can find in this repo is based on the model found from this vendor (affiliate link): https://s.click.aliexpress.com/e/_99rVuu

This is a high quality model of this ring light and I recommend getting that version. You might find cheaper models but they often use a different controller with a smaller case and generally a bit worse built quality, the PCB for the light seems to be generally the same though.

![Demo Video](Videos/demo.webp)

For reproducing you will need a Raspberry Pi Pico, order the PCB in `Case-Hack-PCB` and modify the case with a pair of flat side cutters according to the reference photos in `Case-Modification-Reference`. Beware of the cutouts for the buttons, you need to make them large enough so that the new buttons can fit, otherwise the case will not close well.

To open the case the first time, insert something flat/sharp between the edges of the two halfs and lever them apart, you may need to do that in multiple points before it comes apart. There is no snap fits, its just a pressure fit.

When soldering the PCB, take a look at `Case-Hack-PCB/solder-reference-headers.jpg` you need to trim the headers after soldering and add a header pointing in the opposite direction to the SWD pins for stabilization, those should be soldered first, otherwise its going to be difficult with the button pcb already in place.

I don't have the time to document this in a step by step manner. If anyone reproduces this and would like to do that, PR's are more than welcome.

Original Twitter thread with possibly some more details: https://twitter.com/timonsku/status/1357681117395103746