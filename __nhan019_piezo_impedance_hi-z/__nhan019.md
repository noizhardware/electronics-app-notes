TL;DR 2025j20-1708
- seagull w/ 1M pulldown, recommended 2x row gain is ok w/ piezo, eguit, line/eurorack
- use OPA1677/8/9 for general use
- use TL08x specific for guitar, maybe sounds better
- DC coupled

- ESP 249 still to try, compare w/ seagull

---

folder `OLDrecs`
i files che iniziano con A e B fanno parte di due set diversi di test
- A; piezo su chitarra classica
- B; chitarra elettrica, collegata direttamente, senza piezo

i nomi "oldstone" e "seagull" si riferiscono a due schemi di amplificatore, trovi gli schemi in .jpg qui nella cartella

cmq alla fine il migliore è il _seagull con TL082_ in entrambe le applicazioni ; confirmed 2024k14-1310

new tests, w/ TL082 seagull;
seagull; ok with electric guitar(opamp gain = 1(simple shortcut feedback)) 2025j16-1752
seagull; ~ok w/ piezo; non cambia quasi nulla che attaccarlo derettamente al Zoom H4n.  2025j16-1805
input pulldown; 10M, 1M OK, 100k troppo poco, taglia un po i bassi col piezo 2025j17

w/ OPA1678 seagull;
also OK, w/ 1M pull-down
- w/ piezo on classical guitar OK (no difference w/ direct plugin in H4n) 2025j17-2131
- w/ electric guitar OK (~ no difference w/ direct plugin in H4n) 2025j17-2131
- w/ eurorack ~ok (a bit leaky at 0vol, but maybe it's the breadboard)
conclusions;
- OPA1678 good all-rounder
- TL082 slightly better for guitar


- ESP alternatives;
- project 202 (recs in `/media/nff/RED/Work/git/electronics-app-notes/__nhan019_piezo_impedance_hi-z/toTry/recs`)
	- AC-coupled
	- Fig.1 ; gain 2x, use C3=1uF for extended bass freq range, `R2` and `R6` should go to `Vee`, not `GND`
	- 2025j20 ok w/ piezo, ~same as seagull-1M-2x
	- ok w/eguit, a bit noisy
	- ok w/ eurorack, less bleedthru than seagull
- project 161 ; uber-overkill, included only for reference
- project 252 ; guitar 6band equaliser / out of scope here
- project 214 ; amp to build inside cable to eliminate cable capacitance, out of scope here
- project 249 ; guitar booster, interesting, to try


---

2024k18-1433 schematic "C" (simple buffer)

- electric guitar
- mid pickup
- all tone down
- volume MAX
- E string strummed at fret 12
- E minor chord strummed at neck pickup
- zoom H4n

- schematic `C` w/ Guitar
	- TL072
		- CG_072_100k
		- CG_072_1M
		- CG_072_2M
		- CG_072_5M
		- CG_072_10M
		- CG_072_15M
		- CG_072_20M
	- TL082
		- CG_082_100k
		- CG_082_1M
		- CG_082_2M
		- CG_082_5M
		- CG_082_10M
		- CG_082_15M
		- CG_082_20M
	- OPA2134
		- CG_OPA_100k
		- CG_OPA_1M
		- CG_OPA_2M
		- CG_OPA_5M
		- CG_OPA_10M
		- CG_OPA_15M
		- CG_OPA_20M
	- NE5532
		- CG_NE_100k
		- CG_NE_1M
		- CG_NE_2M
		- CG_NE_5M
		- CG_NE_10M
		- CG_NE_15M
		- CG_NE_20M

NE5532 ubernoisy!
OPA2134 w/ 2M (1M is also ok) pulldown wins 2024k18-2123 / confirmed 2025j15

