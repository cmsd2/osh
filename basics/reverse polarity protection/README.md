Reverse Polarity Protection using a p-channel MOSFET
====================================================

This demonstrates that using a carefully chosen p-channel mosfet,
we can protect sensitive components from a flipped power connector.

Explanation here:
http://electronics.stackexchange.com/questions/104535/reverse-voltage-protection-with-a-p-channel-mosfet

I chose the TSM2311 because it has:

 * very low drain-source resistance when working with TTL voltages
 * a gate-source operating voltage range of +/- 8v which can handle TTL voltages
 * a negative, but small gate threshold voltage 
 * able to pass more than enough current

for larger voltage ranges from gate to source there are ways of clamping V_gs using a zener diode plus a resistor, but that isn't necessary for most digital logic projects.

Included is a photo of the breadboard set up to test several surface mount SOT-23 packages soldered to miniature 6 pin breakout boards.

BOM
---
 * 1 x TSM2311
 * 2 x LED
 * 1 x 220 Ohm resistor
 * 1 x SparkFun SOT23 to DIP adapter https://www.sparkfun.com/products/717

