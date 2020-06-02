# Headphones Driver
###### App Note nhan002

## Main schematic:
<img src="img/hp-v10.png" alt="2020f01" width="80%"/>
On the left the original version, on the right the final version, can drive a single channel or two channels in parallel.

100n cap to block unwanted DC, for once :D

For stereo headphones, use 2 separated copies. Use opa4134, quad version of the 2134

The `non-bus` resistor is to be used when you have a single source coming in.
If the source is a bus, each element of the bus should have their own 100k summing resistor.

## Other ideas:
<img src="img/ysr-v00.png" alt="ysr-v00" width="80%"/>
Adapted version from Yousynth. At the core of kiku_00

Still to be properly tested, will probably be ditched in favor of the simpler opa4134 version

---
<center>
     <a href="../README.md">
          <img src="../img/nhfavico_black.png" alt="noizHARDWARE logo" width="20"/></a></center>

<!--

,,headphones
,,headphone
,,amp
,,amplifier
,,pfl
,,opa 2134
,,tl 082
,,tl082
,,082
,,tl 072
,,tl072
,,072
,,bus
,,burr-brown
,,eurorack

-->