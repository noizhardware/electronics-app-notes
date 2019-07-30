
## SPDT
###da rivedere - ritestare!!!!

#### `OK` @ +/-15V
#### @ +/-12V sembra ci sia un po di distorted bleedthru in alcuni casi

* le due shunt-res da `10k` devono essere omesse in alcuni casi, perchè possono trasportare distorted bleedthru alla GND.
  + si puo fare che le lascio facoltative da montare
  
* ad esempio, col send-return volume pedal (MTX_pedal7_v_0_0)

| //         | plain         | pedal               |
|------------|---------------|---------------------|
| 15v +10k   | `OK`            | `OK`                  |
| 15v NO 10k | not 100% mute | `OK`                  |
| 12v +10k   | `OK`            | distorted bleedthru |
| 12v NO 10k | not 100% mute | `OK`                  |


## SPST
  * `SPST.jpg` mostra un po di configurazioni in cui funziona bene, testate
  * `meagher-SPST.jpg` mostra un'ulteriore configurazione, embeddata in un mixer
  * `SPST-bufferpost.jpg` è una versione con un solo vactrol, con pochissimo passthru **USE WITH CAUTION**
---

#### TODO
  - re-test `SPDT` alla luce delle nuove scoperte in spst
  - try H11F optocouplers (datasheet with appnote here in folder)(0.42€ each)
  