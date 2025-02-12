# Elektronica 

Wanneer je alleen een knop hebt ben je snel uitgekeken… 

We willen ook robots aansturen, racemachines niet tegen muren laten botsen en ga zo maar door. 
Daar hebben we sensoren voor nodig.
<p>
  <img  align="right" src="../../../figures/arduino/elektronica/Picture8.jpg" width="40%" title="blink">
</p> 
We gaan beginnen met een lichtsensor.

Voor een lichtsensor hebben we een LDR nodig, zie de foto. 
LDR staat voor Light Dependent Resistor (licht afhankelijke weerstand). 
De weerstandswaarde verandert met veranderende lichtintensiteit, zie de grafiek.
<p>
  <img  align="right" src="../../../figures/arduino/elektronica/Picture9.jpg" width="40%" title="blink">
</p>
We sluiten de LDR in serie aan met een Ohmse weerstand (een weerstand met een constante weerstandswaarde). 
Zo hebben we een spanningsdeler gemaakt. 
<p>
  <img align="right" src="../../../figures/arduino/elektronica/Picture10.gif" width="40%" title="blink">
</p>

Een deel van de spanning staat over de LDR en een deel van de spanning staat over de weerstand. 
Het enige wat we moeten doen is de spanning over de LDR uitlezen en we weten hoe licht het is!

Het is belangrijk om iets meer te weten over hoe een spanningsdeler werkt, omdat bij het gebruik van een sensor er sprake is van een spanningsdeler. 
De LDR en de Ohmse weerstand staan in serie zodat er geldt: R<sub>totaal</sub> = R<sub>LDR</sub> + R<sub>Ω</sub>. 
De bronspanning is 5,0 Volt en omdat de weerstanden in serie geschakeld zijn, geldt dat de stroomsterkte overal gelijk is. 
De stroomsterkte bereken je met: I = U<sub>bron</sub> : R<sub>totaal</sub>. 
Als je deze informatie combineert, zie je dat de verhouding tussen de spanningen gelijk is aan de verhouding tussen de weerstanden: I =U<sub>LDR</sub> : R<sub>LDR</sub> = U<sub>Ω</sub> : R<sub>Ω</sub>.

Als het lichter is wordt de weerstandswaarde van de LDR kleiner waardoor er minder spanning over de LDR staat, maar meer over de Ohmse weerstand. 
De spanning over de LDR (U<sub>LDR</sub> = 5,0 x R<sub>LDR</sub> / (R<sub>LDR</sub> + R<sub>Ω</sub>)) kan je meten met behulp van de ANALOG IN van de Arduino. 
De spanning is dan een maat voor de gemeten lichtintensiteit.
Je kan nu ook kiezen welke Ohmse weerstand je wilt hebben. 
Dat ligt er aan voor welk gebied je sensor gevoelig moet zijn. Zie de tweede grafiek.
<p align="right">
  <img src="../../../figures/arduino/elektronica/Picture11.jpg" width="100%" title="blink">
</p>
