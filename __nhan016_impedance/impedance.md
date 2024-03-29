﻿Why is high input impedance a good thing?
Is high input impedance always a good thing?

It is a good thing for a voltage input, as if the input impedance is high compared to the source impedance then the voltage level will not drop too much due to the divider effect.

For example, say we have a 10V signal with 1kΩ impedance.

We connect this to a 1MΩ input, the input voltage will be 10V⋅1MΩ1MΩ+1kΩ=9.99V.

If we reduce the input impedance to 10kΩ, we get 10V⋅10kΩ10kΩ+1kΩ=9.09V

Reduce it to 1k and we get 10V⋅1kΩ1kΩ+1kΩ=5V

Hopefully you get the picture - generally an input impedance of at least 10 times the source impedance is a good idea to prevent significant loading.

High input impedance is not always a good thing though, for example if you want to transfer as much power as possible then the source and load impedance should be equal. So in the above example the 1k input impedance would be the best choice.
For a current input a low input impedance (ideally zero) is desired, for example in a transimpedance (current to voltage) amplifier.


Usually you connect a small resistor in series with the output of an opamp to ensure stability. This generally sets and/or dominates the **output impedance**


,,impedance
,,electronics
,,work
