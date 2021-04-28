2021d28

* **OUTPUT**:  100R in series just before the output jack (see output.jpg) - shortcut protection
* **INPUT**: 100k pull-down + 1k series, see INPUT.jpg

  1M is not really useful, with a floating input, it doesn't pull down enough to suppress the noise floor.
  
  I was using 1M to keep the input impedance high, but from nhan018 we can see even with a guitar, a 100k pull-down is ok.
  - see nishInput.jpg, I used an ac-blocking cap + 1M shunt (1k series omitted by mistake) -- (also I could have used a 100k pull-down)
    - 2020g01 -- retested 100n ac-coup + 1M shunt + 1k series >> OK!
    - **TO TEST:** 100n ac-coup + 100k shunt + 1k series (with guitar + amp) **this is the only untested case (I rarely use ac-coupling caps on inputs, tho)**
  - the 1k series resistor is current-limiting, a form of input protection
  - the 100k-1M shunt is a pull-down resitor, keeps the input near GND when nothing's connected, preventing the output to skyrocket up at Vcc


* bhoooo.jpg mi sembra non abbia senso: perchè ho collegato un inverting opamp in quel punto del ciruito? che è poi da dove lo collego allo scope...bhoooo

,,input
,,output
,,protection
,,resistor
,,470r
,,1k
,,cap
,,ac
,,dc
,,coupling
,,clip
,,clipping
,,100R
,,1M