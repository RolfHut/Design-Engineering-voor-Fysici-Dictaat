# DEF Ontwerpopdracht Kalibreer een Sensor
Vandaag ga je kijken of de sensor die je van ons krijgt geschikt is voor een bepaalde toepassing. Welke toepassing dat is en wat de criteria zijn ga je zelf bepalen.

### Leerdoelen

De leerdoelen voor vandaag zijn (deze lijst komt uit de studiehandleiding):

1.	simpele circuits (RC-circuit, spanningsdelers met sensoren) ontwerpen en fabriceren.
2.	ontwerpeisen voor een opdracht SMART opstellen en vervolgens de ontwerpcyclus inrichten, rekening houdend met de randvoorwaarde van de opdracht.
3.	voor een gegeven sensor & analoog-digitaal convertor en gegeven (of zelf gekozen) toepassing een kalibratie meting ontwerpen, inclusief het circuit om de sensor aan te sluiten op de analoog-digitaal convertor, de opstelling bouwen, en meetresultaten verwerken en concluderen of de combinatie van sensor en analoog-digitaal conversie geschikt is voor de toepassing.

### Groep aanmelden 
Deze opdracht doe je in groepen van 3 studenten. Je kan je groepsnummer en je medestudenten vinden op Brightspace onder Groups: ontwerpopdracht 1: Kalibreer een sensor. Allereerst moet je aan de juiste tafel zitten: check of je met de juiste teamgenoten aan tafel zit! ga je naar het juiste notebook in vocareum (link op Brightspace) en geef je hier met de knop 'Send Invite' je groepsgenoten aan zodat jullie gezamelijk in dezelfde notebook kunnen werken. 

**Laat het aan je TA weten zodra je succesvol het notebook heb geopend en jouw groepsgenoten heb uitgenodigd.**

Als jouw groep om 10.55 niet compleet is, trek dan aan de bel bij de TA (vinger opsteken). Wij komen dan kijken wie er mist en schuiven met studenten in incomplete groepen om jullie in volledige groepen te krijgen.


### Samenwerken
Overleg bij alles wat je in het notebook invult met jouw team: wat je inlevert is van jullie alle drie. Je zal dus goed moeten samenwerken. Jullie hebben allemaal als het goed is het hele notebook doorgelezen. Maak nu samen een planning waarin je aangeeft

- Hoe laat je bij de mijlpalen verwacht te zijn. Als je een mijlpaal niet haalt omdat je vast zit, dan is het een goed idee om een TA om hulp te vragen.
- Op welke tijden je als team niet werkt: jullie pauzes, plan deze in! Continue werken is niet effectief.

Vul onderstaande tabel in (en eventueel aan als je meer regels nodig hebt). **Laat je planning aan je TA zien.** De planning moet uiterlijk om **11.15** klaar zijn.

## Voorbereiding: Sanity Checks
Elke groep heeft vier type sensoren gekregen: 

- een lichtgevoelige weerstand (LDR)
- een temperatuur gevoelige weerstand (thermistor)
- een sensor voor sterkte van magneetveld (hall sensor, type 49e)
- een indruk sensor (Force sensor) 

Kies als groep drie van de vier sensoren. Elke student sluit één van de sensoren aan op hun Arduino. Lees via het AnalogReadSerial programma de meetwaarde uit. Bij de LDR, thermistor en druk sensor maak je een spanningsdeler met een referentie weerstand, zoals voorgedaan in het college. Voor de hall sensor zoek je zelf op internet op hoe je hem aan moet sluiten. (Hint: gebruik de zoekterm "pinout"). Kijk bij elke sensor of het je lukt om de meetwaarde te laten variëren. 

Het aansluiten van deze sensoren gaat precies zoals je maandag gedaan hebt in het college introductie Arduino. Kijk het materiaal daarvan terug wanneer het niet lukt om je sensor goed aan te sluiten.


## Stap 1:  Analyse
Als eerste gaan we verzinnen wat je met deze sensoren zou kunnen doen. **LET OP: JE GAAT DEZE OPSTELLING NIET BOUWEN: JE VERZINT HIER WAT ER MOGELIJK KAN MET DEZE SENSOR** Bijvoorbeeld: met een geluidsensor kan je de geluidsoverlast van een overkomend vliegtuig meten. Schets individueel op een papier (liefst A3) per sensor drie verschillende toepassingen van de sensor die je op jouw Arduino hebt aangesloten (dus als groep 9 toepassingen per sensor in totaal). 