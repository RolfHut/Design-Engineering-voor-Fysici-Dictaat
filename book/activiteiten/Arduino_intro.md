# Arduino intro

Leuk dat je aan de slag gaat met Arduino! Wellicht heb je nog geen idee wat een Arduino is en wat je er mee kunt. Een Arduino is een soort microcomputer. De Arduino sluit je aan op een computer waarbij je een programma (in Arduino noemen ze dat een sketch) stuurt naar de Arduino. De Arduino voert vervolgens je geschreven script uit en zorgt voor de uitvoer. Zo kun je een koelkast op een bepaalde temperatuur houden, een zelfrijdende robot aansturen, lichtsensoren maken, een lcd scherm op je shirt aansturen en ga zo maar door. Ook is het mogelijk om geen software te gebruiken en alleen met de elektronica te spelen. De Arduino is dan de spanningsbron.

In deze module gaan we aan het werk met de Arduino en leren we de basismogelijkheden van een Arduino. Bij het werken met een Arduino heb je twee belangrijke onderdelen: De Arduino en een breadboard. De Arduino is de computer, met invoer en uitvoer mogelijkheden. Op het breadboard sluit je de elektronica aan die aangestuurd wordt door de Arduino.

## Arduino
De Arduino Uno, zie {numref}`foto {number} <fig_arduino>` is een van de populairste microcontrollers voor hobbyisten, studenten en professionals. Het is een kleine, programmeerbare elektronica-board die je kunt gebruiken om allerlei creatieve projecten te maken, zoals robots, slimme apparaten en sensoren. Een belangrijk kenmerk van de Arduino Uno is de reeks pinnen die beschikbaar zijn voor interactie met andere elektronische componenten.

```{figure} Figures/Arduino.jpg
---
width: 50%
name: fig_arduino
---
De Arduino.
```

De Arduino Uno heeft verschillende soorten pinnen, elk met een specifieke functie, samengevat in onderstaande tabel. Een groot deel van die pinnen behandelen we tijdens de verschillende onderdelen van de cursus.

|Categorie	|Pinnen	|Functie|
|---|---|---|
|Digitale pinnen|	0–13|	Digitale I/O, aan/uit, seriële communicatie|
|PWM pinnen|	~3, ~5, ~6, ~9, ~10, ~11|	Analoge simulatie (bijv. LED dimmen)|
|Analoge pinnen|	A0–A5|	Lezen van analoge sensoren|
|Voedingspinnen|	5V, 3.3V, GND, Vin|	Voeding en gronding van externe componenten|
|I²C-pinnen|	A4 (SDA), A5 (SCL)|	Communicatie met I²C-apparaten|
|SPI-pinnen|	MOSI, MISO, SCK|	SPI-communicatie|
|Reset pin|	RESET|	Herstart van de Arduino Uno|
|tx & rx| 1 & 2 | seriële communicatie|


## Breadboard
Het breadboard heeft aan beide zijdes twee kolommen die verbonden worden met de voeding (+ en -). De + kant sluit je aan op de 5V uitgang of op een uitvoerpoort van de Arduino. De – kant sluit je aan op de GND (ground) van de Arduino. Alhoewel je de constante output niet altijd gebruikt, is het wel verstandig om deze altijd aan te sluiten.

```{figure} Figures/Breadboard.jpg
---
width: 100%
name: fig_breadboard
align: center
figclass: margin
---
Het breadboard om schakelingen op te bouwen.
```

Het breadboard heeft rijen en kolommen, zie hiernaast en hieronder voor een opgewerkte breadboard. De punten in een rij zijn met elkaar verbonden. Maar laten we hier niet te lang bij stil staan… we gaan aan de slag! 

```{figure} Figures/Breadboardopen.PNG
---
width: 40%
name: fig_breadboardopen
align: center
---
Een open gewerkt breadboard om te tonen hoe de rijen en kolommen verbonden zijn.
```

```{note}
Vaak moet je even aangeven in welke USB-Poort je Arduino zit. Dit doe je door in het programma te gaan naar: Hulpmiddelen/Poort. Daar kun je de juiste USB poort aanklikken, zie {numref}`Figuur {number} <fig_COM>`.
```

## Benodigdheden
Benodigdheden voor deze module:
* Arduino
* Breadboard
* Jumperkabels
* Weerstanden (220 Ω; 330 Ω; 1,0 kΩ; 10 kΩ)
* Potmeter (1 kΩ; 10 kΩ)
* Diode
* 2x LDR
* LED (rood, geel, groen)
* RGB LED
* Servo motor
* DC Motor
* 5x Drukknop
* 2N2222 transistor
* LCD
* Actieve piëzo element (buzzer)

## Opdrachten

````{exercise} Het aansluiten van een LED

Een LED is een diode die licht uitzendt als er stroom door de LED gaat. De LED laat stroom maar door in één richting. De lange poot van de LED moet altijd op de + kant aangesloten worden, de korte poot op de – kant, zie {numref}`foto {number} <fig_LED>`.

```{figure} Figures/LED.jpg
---
width: 10%
name: fig_LED
---
De lange poot van de LED moet aangesloten aan de + kant van de spanningsbron.
```

De stroom door een LED mag meestal maar 20 mA zijn. De spanning over de LED is dan ongeveer 2,0V, deze waardes verschillen een beetje per soort LED, zie onderstaande tabel. De Arduino levert een 5,0 V spanning. De LED moet dus in serie geschakeld worden met een weerstand. De weerstand moet dus minimaal 150 Ω zijn ($R = \frac{U}{I} = \frac{3,0}{0,020} = 150$ Ω). 

```{figure} Figures/LED_opstelling.png
---
width: 30%
name: fig_LED_opstelling
align: center
---
De schakeling van de LED.
```

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