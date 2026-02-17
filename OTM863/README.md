<b>OTM863</b><br>
<p>OTM863 is a simple utility that writes a rotating logic one to the 12-bit output register on J1 of the M863 12 Channel Buffered Digital I/O (DR8E). This utility is convenient for debugging the output register functions of the M863, or to understand how it works, or to debug issues with cables that attach to J1 in the M863. The output register latches when a selected bit is set and will reset when a selected bit is cleared. This utility first clears all output register bits and incrementally sets each bit of the output register starting with bit 0, then bit 1, and so on. After bit 11 is set the program clears all output register bits and starts over. This is intended to be a scope-loop type of utility. Switch 0 must be set to zero when the program is started. The program is terminated by flipping switch 0 to one. This will return control to the OS/8 command prompt.</p>
<P>Note that the outputs to J1 on the M863 board are active low, so setting the output register causes a low level to appear on J1. The outputs are driven by a SN7416 high-voltage open-collector drivers that are pulled to +5V through a 470 ohm resistor.</P>
<P>OTM863.PA is the PAL source file<br>
OTM863.LS is the listing file<br>
To build this utility and output a listing, type the following at the OS/8 command line:<br>
PAL OTM863,OTM863_OTM863/H</P>
