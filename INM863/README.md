<b>INM863</b><br>
<p>INM863 is a simple utility that reads the 12-bit input port from J2 of the M863 12 Channel Buffered Digital I/O (DR8E), and displays the word in the AC lights. After reading the input port, the program enters a wait loop to hold the value in the AC lights before reading the input register again. This utility is convenient for debugging the M863, or to understand how it works, or to debug issues with cables that attach to J2 in the M863. Be sure to rotate the front panel switch to display the AC register to observe the value read from the input port. Switch 0 must be set to zero when the program is started. The program is terminated by flipping switch 0 to one. This will return control to the OS/8 command prompt.</p>
<p>The M863 input register is cleared when INM863 is started. The M863 can be configured to either latch a value in the input register or to pass the value from J2 directly to the input register. This can be configured bit-by-bit via jumpers on the M863 board. Refer to the DEC documentation and schematic for a more detailed description.</p>
<P>INM863.PA is the PAL source file<br>
INM863.LS is the listing file<br>
To build this utility and output a listing, type the following at the OS/8 command line:<br>
PAL INM863,INM863_INM863/H</P>
