## Betterbus
  * vedi schematic betterbus.jpg
  * usando dei summing resistor di vari valori si hanno vari risultati
  * nella cartella 7snd7betterbus ci sono le registrazioni coi vari valori di resistor
  * gli esperimenti sono fatti usando un longwire tra la summing resistor e il summing opamp, per vedere quale rende meglio, i parametri misurati sono;
    - distorted bleedthru (con resistenze troppo piccole si creano upper harmonics)
    - resilience to EMI-touch, grabbando i longwire con la mano
  
  **CONCLUSIONS :**
  - se uso una resistenza da 100k o piu grande, ho zero distortion, ma molto sensibile a EMI
  - se uso una resistenza troppo piccola è insensibile alle EMI, ma distorce il segnale
  - `47k` si è rivelato un ottimo candidato, zero distorsione, poca sensibilità alle EMI (non zero, purtroppo)
  
  