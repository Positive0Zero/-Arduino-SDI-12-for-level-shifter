# -Arduino-SDI-12-for-level-shifter
An adapted SDI12 library for use with 3.3V Arduino boards, tested with SAMD controllers, in particular Arduino MKR.

# Hardware
SDI12 operates at a 5V logic level. Therefore, we use a level shifter.
Some tests and experience show that a bidirectional level shifter does not work.
Therefore, we use a shifter here whose direction can be set via a DIR pin.

For example, the SN74LVC2T45DCUR

The input and output network is taken from the SDI12 specification. This includes several filters and protection circuits.

#
Sample Circuit Diagram
A1 = SDI Data low voltage
B1 = SDI Data high voltage
DIR = Direction of level shifting

<img width="1322" height="428" alt="grafik" src="https://github.com/Positive0Zero/-Arduino-SDI-12-for-level-shifter/blob/main/Schematic_Level_Shifter.JPG" />


