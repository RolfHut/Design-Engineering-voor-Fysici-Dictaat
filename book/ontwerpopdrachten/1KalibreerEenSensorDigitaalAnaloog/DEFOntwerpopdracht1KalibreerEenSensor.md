# DEF Ontwerpopdracht Kalibreer een Sensor
Vandaag ga je samen kijken of de sensor die je van ons krijgt geschikt is voor een bepaalde toepassing. Welke toepassing dat is en wat de criteria zijn ga je zelf bepalen.

## Introductie

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

**Laat aan je TA zien dat alle drie de sensoren werken. Je TA tekent dit af.** 

## Ontwerpstap Analyse
Als eerste gaan we verzinnen wat je met deze sensoren zou kunnen doen. **LET OP: JE GAAT DEZE OPSTELLING NIET BOUWEN: JE VERZINT HIER WAT ER MOGELIJK KAN MET DEZE SENSOR** Bijvoorbeeld: met een geluidsensor kan je de geluidsoverlast van een overkomend vliegtuig meten. Schets individueel op een papier (liefst A3) per sensor drie verschillende toepassingen van de sensor die je op jouw Arduino hebt aangesloten (dus als groep 9 toepassingen per sensor in totaal). Leg je schetsen naast elkaar, maak één foto en upload die bij *Opdracht 1* van het invul template.

## Ontwerpstap Criteria
Bepaal voor de bedachte toepassingen de criteria waarbij de sensor geschikt is. Definieer je criteria als een harde grens. Gebruik natuurkundige eenheden. Denk aan **SM**a**R**t uit het college. Het kunnen per toepassing meerdere criteria zijn. Kies vervolgens één van de drie sensoren uit om de rest van de dag mee verder te gaan. Vul je criteria en keuze in bij *Opdracht 2* van het template. 

##  Sanity Check
**Laat je criteria aan je TA zien. Laat ook aan je TA zien dat de gekozen sensor werkt: dat de meetwaarde wijzigt als je de sensor beinvloedt (warmer maakt, erin knijpt, etc). Je TA tekent dit af!**. Dit laat ons zien dat het jullie allemaal gelukt is in ieder geval de sensor werkend aan te sluiten. Als je niet voor 12.00 iets laat zien komen we bij jullie groep langs om te vragen wat er mis is en om jullie te helpen.

## Ontwerpstap simulatie en evaluatie: kalibratie opstelling maken!
Je gaat een kalibratieopstelling ontwerpen en bouwen om je sensor mee te evalueren. Het ontwerpen van je opstelling is een aparte ontwerp ronde binnen deze evaluatie stap! 

### sub-ontwerpstap: Synthese
Welk experiment wil je gaan doen om jouw sensor te evalueren? Schets hieronder de meetopstelling die je voor ogen hebt. Hou rekening met beschikbare materialen. Zorg ook dat het elektrisch circuit dat onderdeel van jouw opstelling is duidelijk is. Mogelijk teken je dit apart. Jouw schets hoeft niet mooi te zijn, maar moet wel duidelijk zijn. Geef waar nodig aan met labels wat je bedoelt. Maak een foto van je schets en zet die bij *Opdracht 3* in het invul template. 

### sub-ontwerpstap: Evaluatie

In deze stap bepaal je of jouw opstelling in staat gaat zijn om de evaluatie uit te voeren. Beantwoord de volgende vragen:

1. Welke variabelen ga je veranderen? 
2. Over welk bereik ga je deze variabelen veranderen?
3. Wat ga je allemaal meten?
4. Hoeveel metingen ga je doen?
5. Ga je met deze keuzes kunnen evalueren of jouw sensor geschikt is voor de gekozen toepassingen?

Als je bij vraag 5 nee antwoord, ga dan terug naar sub-ontwerpstap: Synthese hierboven en pas jouw ontwerp aan. Als het antwoord ja is, vul je antwoorden dan in bij *Opdracht 4* van het template en **laat dit dan aan je TA zien voordat je verder gaat.**

### sub-ontwerpstap: simulatie: bouwen en meten

- Bouw de kalibratieopstelling.
- doe je kalibratie metingen (noteer op papier!)

### Eerste meting MIJLPAAL 2
**Zodra je jouw eerste meting gedaan hebt laat je deze aan je TA zien. Je TA tekent dit af** Je TA geeft mogelijk nog feedback op de opstelling en het meetplan om deze waar nodig te verbeteren. 

- Ga daarna door met het meetplan uitvoeren.
- Maak een foto van de opstelling. Zet deze foto bij *Opdracht 5* van het invul template

### sub-ontwerpstap: simulatie

bij *Opdracht 6* van het invul template staan Python cellen waar je zelf code kan schrijven. 

- Zet je data in een handig formaat
- maak een grafiek zoals je geleerd hebt bij het practicum.
- Voeg een fit-lijn aan je grafiek toe. Denk goed na over de vorm van deze lijn.

### sub-ontwerpstap: iteratie nodig?

Op dit punt moet je beslissen: hebben we genoeg gegevens om een conclusie te trekken: is deze sensor geschikt voor de door ons gekozen toepassingen? Overleg dit met jouw groep. Als jouw antwoord is: we hebben nog niet genoeg gegevens, beschrijf dan bij *Opdracht 7* wat jullie nog gaan doen: meer van dezelfde metingen? Andere metingen? 

Als je gaat itereren, voeg dan zelf extra cellen toe aan het invul template waar je de extra code en grafieken in laat zien van de extra metingen. Dat is prima en hoort bij ontwerpen.

Als je niet gaat itereren, meld dat dan bij *Opdracht 7*

### sub-ontwerpstap: Conclusie
Op basis van jouw metingen zou je een conclusie moeten kunnen trekken over de bruikbaarheid van jouw sensor voor de gekozen toepassing. Schrijf bij *Opdracht 8* jouw conlusie. Wees kort en bondig, maar leg wel duidelijk uit waar je jouw conclusie op baseert, alleen "ja" of "nee" volstaat niet. Gebruik max 50 woorden. **Laat je conclusie aan je TA zien. Als je TA alles ok vindt, ben je bijna klaar voor vandaag en kan je gaan evalueren, inleveren en opruimen.** 

## Aantonen leerdoelen
Je hebt vandaag gewerkt aan het onder de knie krijgen van de volgende leerdoelen:

1.	simpele circuits (RC-circuit, spanningsdelers met sensoren) ontwerpen en fabriceren.
2.	ontwerpeisen voor een opdracht SMART opstellen en vervolgens de ontwerpcyclus inrichten, rekening houdend met de randvoorwaarde van de opdracht.
3.	voor een gegeven sensor & analoog-digitaal convertor en gegeven (of zelf gekozen) toepassing een kalibratie meting ontwerpen, inclusief het circuit om de sensor aan te sluiten op de analoog-digitaal convertor, de opstelling bouwen, en meetresultaten verwerken en concluderen of de combinatie van sensor en analoog-digitaal conversie geschikt is voor de toepassing.

Als het goed is laat je werk in het template zien dat je deze leerdoelen nu beheert. Het is aan jullie om zelf aan te geven welke cellen van het template bij welk leerdoel horen. Lees het template door, kijk goed naar de cellen met LEERDOEL in de titel. Kopieer deze cellen en zet ze bij het juiste leerdoel in het template bij *Opdracht 9*.

## Inleveren op Vocareum
Je bent nu klaar met het invul template en kan deze op vocareum inleveren. 

- Open Vocareum via de link op Brightspace. 
- Nodig je groepsgenoten uit
- Upload je notebook en alle foto's naar vocareum via de 'upload' knop.
- Open je notebook in Vocareum
- **Klik boven op Kernel -> Restart and Run all**
- Check of er geen errors zijn en alle afbeeldingen zichtbaar zijn.
- Als je helemaal klaar bent kan het notebook worden ingeleverd door bovenaan op **submit** te klikken. Je kan meerdere keren iets inleveren en alleen de laatste versie wordt bewaard. Na de deadline is het niet meer mogelijk om in te leveren.

**Wanneer je klaar bent, roep je de TA. Laat je notebook binnen Vocareum aan de TA zien. Je TA tekent dit af**

## Evalueren groepswerk
Voordat je het uiteindelijke resultaat inlevert geef je binnen je groep feedback op hoe het samenwerken vandaag ging. Kijk eerst allemaal deze youtube video: https://www.youtube.com/watch?v=16uW1kPoiww. Lees daarna het PDF document 'instructie feedback geven' dat op Brightspace staat. Geef ten slotte elkaar feedback. Noteer de feedback die je krijgt in het 'logboek ontvangen feedback' dat ook op Brightspace staat. Bewaar dit logboek goed: je moet het elke week aanvullen met de feedback die je die week krijgt.

Lever individueel je logboek in op Brightspace, voor 17.30.

## Opruimen
Als de TA de conclusie goedgekeurd heeft en jouw opdracht ingeleverd is kan je gaan opruimen. Als alles opgeruimd is laat je dit aan de TA zien. **Pas als de TA zegt dat het goed opgeruimd is mag je naar huis**. Groepen die vertrekken zonder dat de TA gecontroleerd heeft of alles netjes opgeruimd is worden niet nagekeken.


### Optioneel: Implementatie van Kalibratie
Nu de sensor gekalibreerd is, zou je de code op jouw Arduino moeten kunnen aanpassen zodat je op de seriale monitor niet meer ruwe digitale meetwaardes ziet, maar daadwerkelijk gemeten fysische waardes, bijvoorbeeld de temperatuur in graden Celsius als je voor de thermistor gekozen hebt. 

### Optioneel: Implementatie van toepassing
Mogelijk ben je met de gegeven materialen zelfs in staat om de toepassing die je voor ogen had te bouwen.