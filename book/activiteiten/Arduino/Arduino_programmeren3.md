# Programmeren deel 3

De Arduino kan niet alle waarden uitlezen. 
De ANALOG IN heeft een 10 bits chip. 
Dit betekent dat er 2<sup>10</sup> = 1024 waarden doorgegeven kunnen worden. 
<p>
  <img align="right" src="../../../figures/arduino/programmeren3/Picture7.jpg" width="40%" title="bit_steps">
</p>

Het is alsof je de 5,0 V in 1024 - 1 kleine blokjes verdeelt. 
De waarde die je uitleest bij opdracht 5 is dus ook niet de spanning zelf, maar het getal dat bij een spanning hoort. 
Het getal 223 hoort dus bij: 223 / 1023 * 5,0 = 1,09 V. 
De PWM(~) is een 8 bits systeem en kan dus 2<sup>8</sup> = 256 waarden geven.

Oei… zie je het probleem? 
We kunnen inlezen met 1023 verschillende waardes, maar uitschrijven kan maar met 255 waardes…. 

Gelukkig is er een code die zorgt voor een automatische schaling (**map**). 
De functie **map** wil 5 getallen hebben. 
- Het eerste getal is wat de analoge poort door geeft. 
- Het tweede getal is het laagste getal dat uitgelezen kan worden
- Het derde getal de grootste waarde dat uitgelezen kan worden. Dit hoeft niet per se 0 en 1023 te zijn… 
  De gevoeligheid van je sensor kan ook zitten tussen 500 en 900, zie wederom grafiek 2 uit programmeren deel 3. 
- Het vierde getal geeft de lower bound van de target range. 
- En het vijfde getal geeft de upperbound van de target range. 

```
void loop(){
    sensorValue = analogRead(sensorPin);
    brightness = map(sensorValue,500,900,255,0);
    Serial.println(sensorValue);
    delay(10);
    analogWrite(ledPin,brightness);
}
```

In het voorbeeld moet een inputwaarde van 500 een output waarde worden van 255. 
Een input waarde van 900 moet een output waarde van 0 worden.

Een functie die ook handig is, is de functie ++, ``` count++;``` (Python: ``` count += 1```)
Elke keer als de loop de volgende cyclus ingaat, wordt de waarde met 1 verhoogd. 
Zo kan je eenvoudig bijhouden hoeveel loops er al zijn geweest. 
Ook is het mogelijk om op die manier elke keer een andere pin aan te sturen of later een frequentie te veranderen.