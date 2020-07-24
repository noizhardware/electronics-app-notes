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

**ACHTUNG** (2020g24) using a `tl082` instead of a `tl074` _seems_ to be solving the distortion problem with this version.
In the end this is the most flexible version, as you're not stuck with a fixed `1x` for the **Gmin**.

Use this **ONLY** if you need to have `Gmin` smaller than 1.

Small resistor values for `Ri` and `Rm` might result in distortion. **ALWAYS TEST**

TODO: set lower limits for `Ri` and `Rm` to work without distortion.

  If you need it to just be inverting, the best way to do it is using the non-inverting version and then inverting the signal.

<img src="img/varigain.png" alt="" width="80%"/>

**Rm** = Gmin * Ri

**Ri** = (Rf + Rm) / Gmax



---
<center>
     <a href="../README.md">
          <img src="../img/nhfavico_black.png" alt="noizHARDWARE logo" width="20"/></center></a>

<!--

,,gain
,,varigain

-->
