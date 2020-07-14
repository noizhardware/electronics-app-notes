# Varigain
###### App Note nhan025

## Main schematics:

### non-inverting
the non-inverting version is free from distortion and safe to use.
`Gmin` cannot be smaller than 1 in this configuration.
<img src="img/varigain-NI.png" alt="" width="80%"/>

**Gmin** = 1

**Gmax** = 1 + Rp/Rs

**Rs** = Rp / (Gmax - 1)

### inverting
This is the inverting version, might cause distortion in some cases.
Use this if you need to have `Gmin` smaller than 1.
Small resistor values for `Ri` and `Rm` might result in distortion. **ALWAYS TEST**
TODO: set lower limits for `Ri` and `Rm` to work without distortion.
  If you need it to just be inverting, the best way is to use the non-inverting circuit and then invert the signal.

<img src="img/varigain.png" alt="" width="80%"/>



---
<center>
     <a href="../README.md">
          <img src="../img/nhfavico_black.png" alt="noizHARDWARE logo" width="20"/></center></a>

<!--

,,gain
,,varigain

-->