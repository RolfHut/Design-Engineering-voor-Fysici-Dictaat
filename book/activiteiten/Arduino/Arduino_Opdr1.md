

# Opdracht 1

## Het aansluiten van een LED

Een LED is een diode die licht uitzendt als er stroom door de LED gaat. De LED laat stroom maar door in één richting. De lange poot van de LED moet altijd op de + kant aangesloten worden, de korte poot op de – kant, zie {numref}`foto {number} <fig_LED>`.

<p align="right">
  <img src="../../../figures/arduino/Opdr1/LED_circuit.jpg" width="40%" title="De Arduino" name="fig_circuit_LED">
</p>


De stroom door een LED mag meestal maar 20 mA zijn waarbij de spanning over de LED 2,0 V is. 
De Arduino levert een 5,0 V spanning. De LED moet dus in serie geschakeld worden met een weerstand. 
De weerstand moet dus minimaal 150 Ω zijn (R = U / I = 3,0 / 0,020 = 150 Ω).

<p align="right">
  <img src="../../../figures/arduino/Opdr1/resistor_values.jpg" width="40%" title="De Arduino" name="fig_circuit_LED">
</p>

a) Er is geen weerstand aanwezig van 150 Ω maar wel een van 220 Ω. Zoek de weerstand op met behulp van de kleurcode: de eerste ring moet rood zijn, de tweede ring ook en de derde ring bruin (22·10). Een andere mogelijkheid is rood, rood, zwart, zwart.

b) Sluit nu de 5V uitgang van de Arduino aan op de **+** kolom en de **GND** (ground) uitgang van de Arduino aan op de – kolom. 

c) Sluit de LED en de weerstand in serie aan, zie  {numref}`tekening {number} <fig_LED_1>`.

```{figure} Figures/LED_1.PNG
---
width: 70%
name: fig_LED_1
align: center
---
De te maken schakeling
```

d) Verbind de Arduino via de usb met de computer. Als je het goed hebt gedaan brandt de LED!

Doordat de rode led bij lagere spanning licht uit zendt dan bijvoorbeeld een groene led, kun je een kleinere weerstand bij groene en blauwe led’s gebruiken. Zo branden ze uiteindelijk toch nog even fel!

|Kleur|Drempelspanning (V)|
|---|---|
|Blauw|2,3|
|Groen|2,0|
|Rood|1,5|

````

```{figure} Figures/Resistor_color_code.png
---
width: 70%
name: fig_colorcodes
---
Het kleurenschema voor bepaling van de weerstand, figuur van [wikimedia](https://commons.wikimedia.org/wiki/File:Resistor_color_code.png) (common creatives)
```

Nu kun je je led wel laten branden, maar daar heb je nog niet veel aan… Een volgende stap is de LED aansturen met behulp van een stukje code. 

````{exercise} Een knipperende LED
Om de LED aan te sturen met behulp van code moet je een uitvoerpoort (bijvoorbeeld pin 13) van de Arduino verbinden met je LED. De 5V output heb je nu niet nodig, pin 13 levert nu de spanning. In de tekening zie je dat deze wel verbonden is, bij grotere projecten vergeet je snel de 5V, vandaar!

a) Bouw de opstelling die je ziet in {numref}`tekening {number} <fig_LED_2>` en sluit de Arduino aan op de computer. We willen de Arduino aansturen, daarvoor gebruiken we het Arduino programma.

```{figure} Figures/LED_2.PNG
---
width: 50%
name: fig_LED_2
align: center
---
De te maken schakeling waarbij de LED aangestuurd wordt met Pin 13.
```


b) Open het programma en open het script blink via: `bestand/voorbeelden/basis/blink`.

```{figure} Figures/Blink.gif
---
width: 80%
name: fig_gif
align: center
---
Open uit de examples de code blink
```


c) Controleer het script met het vinkje. Mocht het programma niet werken, dan geeft het onderaan een foutmelding weer (het kan zijn dat je de COM-poort moet toewijzen, dit doe je via hulpmiddelen/poort).

```{figure} Figures/COM.gif
---
width: 80%
name: fig_COM
align: center
---
Aanwijzen van de USB poort waar de Arduino aan hangt.
```

d) Upload het script naar je Arduino met het tekentje {fa}`right-long`. (snelcode: ctrl + u)

e) Beschrijf kort wat je ziet. Probeer wat je ziet te verklaren met behulp van de code.

f) Verander het script zodat de LED sneller knippert.

g) Sluit drie verschillende LED lampjes aan, verander het script zodat ze om de beurt aan staan.

```{figure} Figures/Verkeerslicht.PNG
---
width: 50%
name: fig_Verkeerslicht
align: center
---
Uitbreiding van de schakeling met een gele en groene LED om het verkeerslicht te maken.
```

h) Verander het script en maak een verkeerslicht waarbij oranje maar even aan staat.
````