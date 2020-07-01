2020g01

* OUTPUT:  100R in series just before the output jack (see output.jpg) - shortcut protection
* INPUT: 1M pull-down + 1k series, see INPUT.jpg
  - see nishInput.jpg, I used an ac-blocking cap + 1M shunt (1k series omitted by mistake)
    - 2020g01 -- retested 100n ac-coup + 1M shunt + 1k series >> OK!
  - the 1k series resistor is current-limiting, a form of input protection
  - the 1M shunt is a pull-down resitor, keeps the input near GND when nothing's connected, preventing the output to skyrocket up at Vcc


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