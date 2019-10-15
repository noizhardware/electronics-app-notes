### nhan001    <img src="../img/nhfull_tiny.png" alt="noizHARDWARE logo" width="30"/>

# Example App Note

[Go to App Note nhan001](http://htmlpreview.github.io/?https://github.com/noizhardware/electronics-app-notes/blob/master/nhan001/nhan001.html "App Note HTML page")

* in caso di (gain > 1), mettere sempre il gain il più "alla fine" possibile, quando possibile
  - mantenere il segnale con (gain == 1) per il più possibile, per evitare distorsioni e bleed.
  - ad esempio vedi il softswitch `SSPST_v_2_0`, giova esattamente di sta cosa qui!
  - è buono anche per un altro motivo; hi-voltages don't go to GND! se ho un gain alto all'inizio, poi se ho un volume pot, quando è a zero, manderà il segnale ad alto voltaggio nella GND, rischiando di creare disto-bleed!!!
  - **è probabilmente il motivo per cui succedeva il noise con `weston`**