# Opdracht 5

## Een lichtsensor

De schakeling lijkt erg op de schakeling van opdracht 4. 
Alleen nu gebruiken we een LDR en een ANALOG IN .

a) Bouw de schakeling.

<p align="center">
  <img src="../../../figures/arduino/Opdr5/LDR_bb.jpg " width="40%" title="LED_opdr2">
</p>

b) Open in de Arduino IDE het programma Analogreadserial.
De belangrijkste code vind je hieronder.
```
void loop(){
    int sensorValue = analogRead(A0);
    Serial.println(sensorValue);delay(1);
}
```

De Arduino krijgt de opdracht om de analoge poort uit te lezen ```analogRead(A0)```. 
Deze waarde wordt gehangen aan de variabele sensorValue. 
Vervolgens willen we deze waarde weten. 
De waarde wordt dan ook geprint voor ons ```Serial.println(sensorValue);```. 
De waarde kan niet continu gelezen worden daarom wordt er een ```delay``` ingebouwd.

c) Upload het programma naar de Arduino en lees de waarden uit met behulp van de SerialMonitor (rechts boven in de Arduino IDE).

d) Bedek met je hand de LDR. Verandert de gegeven waarde?

e) Combineer opdracht 3 en deze opdracht. 
Zorg ervoor dat de LED feller gaat branden als het donkerder wordt.

f) Breid de schakeling verder uit zodat je de hele schakeling ook met een knop aan en uit kan zetten.

g) Leg met behulp van grafiek 2 uit dat een grote waarde van $$R_Ω$$ ervoor zorgt dat de LDR in het hele bereik even gevoelig is.



