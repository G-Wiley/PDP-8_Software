README.md
<b>BLINK</b><br>
<p>BLINK is a simple utility that reads a word from the switch register and rotates that pattern in the Accumulator lights on the front panel. Be sure to rotate the front panel switch to display the AC register.</p>
<p>BLINK was developed to be a simple flashy light demo when I exhibited my 8/m at VCF SoCAL 2026. The original demo that I had planned was somewhat of a failure, to BLINK was created to give the appearance that the machine was doing something.</p><br>
<p>This an improved version of the original blink. This version reads the switch register after each complete rotation of 12 shifts so the user can change the pattern "live" by changing the switch register value.</p><br>
<p>Any value can be entered in the SR except that bit 0 (SR00) must be zero. The program is terminated by flipping switch 0 to one. This will return control to the OS/8 command prompt.</p>


