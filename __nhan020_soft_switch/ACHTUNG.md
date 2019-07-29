
## `OK` @ +/-15V
## @ +/-12V sembra ci sia un po di distorted bleedthru in alcuni casi

* le due shunt-res da `10k` devono essere omesse in alcuni casi, perchè possono trasportare distorted bleedthru alla GND.
  + si puo fare che le lascio facoltative da montare
  
* ad esempio, col send-return volume pedal (MTX_pedal7_v_0_0)

| //         | plain         | pedal               |
|------------|---------------|---------------------|
| 15v +10k   | `OK`            | `OK`                  |
| 15v NO 10k | not 100% mute | `OK`                  |
| 12v +10k   | `OK`            | distorted bleedthru |
| 12v NO 10k | not 100% mute | `OK`                  |


---
####**TODO**
  - ritestare il SPST con la shunt 10k PRIMA del vactrol!!!
    - e prova anche con 47k
  - same table for SPST version
  - add notes from Meagher_7line
  