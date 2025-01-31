# Echo akoestisch algoritme
Vandaag ga je zelf een algoritme ontwerpen waarmee je de locatie van een object op basis van echo's gaat bepalen.
Dit notebook helpt je daar doorheen.

## Leerdoel
Het leerdoel voor vandaag is: 

- Inzien dat het maken van een algoritme een ontwerpproces is en het proces optimaal inrichten op de randvoorwaarden van de opdracht

Aan het einde van de dag laat je zien dat je dit leerdoel onder de knie hebt door relevant zaken aan te leveren. Zie onderaan dit notebook.

### Groep aanmelden 
Deze opdracht doe je in groepen van 3 studenten. Je kan je groepsnummer en je medestudenten vinden op Brightspace onder Groups: ontwerpopdracht 4: maak een algoritme. Vervolgens ga je naar het juiste notebook in vocareum (link op brightspace) en geef je hier met de knop 'Send Invite' je groepsgenoten aan zodat jullie gezamenlijk in dezelfde notebook kunnen werken. Uiteindelijk lever je dit notebook als groep in via vocareum door op submit te klikken.

Als je groep om 11:00 niet compleet is, trek dan aan de bel je TA erbij te roepen. Wij komen dan kijken wie er mist en schuiven met studenten in incomplete groepen om jullie in volledige groepen te krijgen.

### Samenwerken
Overleg bij alles wat je in het notebook invult met je team: wat je inlevert is van jullie alle drie. Je zal dus goed moeten samenwerken. Jullie hebben allemaal als het goed is het hele notebook doorgelezen. Maak nu samen een planning waarin je aangeeft

- Hoe laat je bij de mijlpalen verwacht te zijn. Als je een mijlpaal niet haalt omdat je vast zit is het een goed idee om je TA om hulp te vragen
- Op welke tijden je als team niet met de opdracht bezig gaat zijn (je pauzes, plan deze in! continue werken is niet effectief)

Vul onderstaande tabel in bij opdracht 1 in de template. 
*Laat de planning aan je TA zien om deze te controleren. De planning moet uiterlijk om 11.00 gezien zijn*.

### Voorbereiding, werkruimte inrichten, benodigd materiaal.

Run cel onder opdracht 2 in de template om alle benodigde libraries te laden. Mogelijk voeg je er zelf nog een aantal toe later vandaag.

Je hebt een leeg oppervlak van (minstens) 70 cm bij 70 cm nodig. Op de tafels hebben we een assenstelsel aangebracht. Daarnaast heb je nodig:

- Stuk gevouwen A3 papier, hoe steviger het papier hoe beter. Staat al op je tafel.
- Je Arduino, met daarop aangesloten de akoestische sensor, die in je zelfgemaakte houder zit. Zie hieronder voor de schakeling waarmee je de Arduino aansluit op de sensor.
- Een telefoon of andere camera om foto's van je opstelling te maken. Voeg, waar nodig, een korte beschrijving toe om toe te lichten wat we zien op de foto

Sluit je Arduino aan volgens deze schakeling, zorg ervoor dat je USB kabel niet in je laptop zit terwijl je de schakeling aansluit!

<img src="\schakeling.png\" width="\2000\">

### Opdracht 1: Kalibreren sensor 

Upload de code ```distanceCalibration.ino``` die op Brightspace staat naar je Arduino. Open vervolgens de ```Serial Monitor``` op je laptop. Je ziet nu de ruwe meetwaarden van je sensor binnenkomen. In het college  is uitgelegd wat deze waardes betekenen.

Doe een serie metingen om je sensor te kalibreren. Bepaal zelf geschikte afstanden waarop je zender, ontvanger en reflector neerzet. Gebruik het meetlint van één van de assen op je tafel om de afstand te bepalen. Verwerk jullie metingen bij opdracht 3 in de template. Bepaal zelf welk verband het beste je metingen beschrijft en fit de bijpassende functie.

***Let erop dat je totale afgelegde afstand van het geluid gebruikt, dus 'heen en terug'***

Maak ook een foto van je kalibratieopstelling en voeg deze in bij opdracht 3 in de template. 

### Zet kalibratie resultaat in Arduino
Open vervolgens de Arduino code ```distanceMeasurement.ino``` die op Brightspace staat. Pas deze code aan zodat je eigen kalibratie constanten erin staan. Upload vervolgens deze code naar je Arduino. Jullie hebben nu zelf jullie sensor gekalibreerd en bent klaar voor het volgende deel van de opdracht.
   
### Opdracht 2: Testen meetopstelling
 We hebben op elke tafel een assenstelsen aangebracht met papieren linialen. We gebruiken de notatie (x,y) in centimeters, bijvoorbeeld (0,40) is het punt 40 cm op de y-as, en (35,35) is in het midden van je oppervlak.
 
 Jullie gaan 7 metingen doen om het imaging algoritme te testen. 
 Zet het papier met de vouw op (20,20) en met een hoek van 90 graden.
 Zie onderstaande figuur.
 <img src=\"testMeting.png\" width=\"400\">
 
 Doe metingen met je bron en ontvanger op de volgende posities. Noteer de totaal afgelegde afstand van het geluid zoals je Arduino die meet. Gebruik hiervoor de cel bij opdracht 4 in de Template.
 - bron (0,40), ontvanger (0,30)
 - bron (0,30), ontvanger (0,20)
 - bron (0,10), ontvanger (0,20)
 - bron (40,0), ontvanger (30,0)
 - bron (30,0), ontvanger (20,0)
 - bron (10,0), ontvanger (20,0)
 - bron (10,0), ontvanger (0,10)

Dit moet nu een uitkomst opleveren dichtbij de verwachte waarden: x0=20 cm y0=20 cm alpha=0 graden, beta=0 graden met kleine std. dev.

Laat dit zien aan je TA. **De deadline hiervoor is 12.00 PM. Als het voor die tijd niet gelukt is komen we kijken wat er mis gaat en hoe we jullie kunnen helpen.**
 
## Ontwerp individueel algoritme
Hieronder doorloop je de stappen van de ontwerp-cyclus.

Nu bedenkt elke student, individueel, een eerste algortime. Voor veel groepen komt dit ongeveer overeen met de lunchpauze. Beschrijf je algoritmen visueel (blokkenschema) op een A3 zodat je mede studenten (en docenten) snappen hoe je algoritme werkt. 

In sommige gevallen (uitzonderingen) zal je wat python code willen schrijven voor je algoritme.

Ten slotte voer je je algoritme uit om te kijken of het daadwerkelijk werkt. 

Daarna ga je als 1e iteratie de beste ideeen van de verschillende algoritmes combineren tot één nieuw algoritme. "

# Iteratie 0: Eerste pogingen
### Synthese
Beschrijf bij opdracht 5 in de template jullie algoritmes. Voeg als nodig een figuur toe.

### Simulatie 
Overleg als groep welke algoritme je kansrijk acht om goed te gaan werken. Kies minstens twee, mogelijk alle drie, de algoritme om te testen. Hou er rekening mee dat metingen doen en verwerken tijd kost, dus werk snel. Kies als groep zelf een combinatie van x0, y0, alpha en beta. Zet het reflectie-paper op deze zelf gekozen positie en voer één voor één minimaal twee van de drie algoritmes uit. Dat levert een hele reeks aan meetgegevens op die je bij opdracht 6 in de template invult.

Alleen de metingen die een bruikbare waarde opgeven kun je in de data array in de volgende stap toevoegen; 
de rest van de metingen kan niet gebruikt worden door het imagingDEF programma en moet je dus met een ```#``` commentarieren. 

### Evaluatie
Run de cellen onder opdracht 7 in de template om de evaluatie uit te kunnen voeren. 

# Iteratie 1+
### Synthese
Maak een nieuwe blokkenschema op A3 van wat je nu als algoritme gaat proberen. Als het kleine wijzigingen zijn ten opzichte van een vorige iteratie, kras dan gewoon in de oude blokkenschema als dat duidelijk blijft. Maak een foto en zet die bij opdracht 8 van de template. Zorg dat het iteratienummer goed op de foto te zien is.

### Simulatie en evaluatie
Je gaat nu weer metingen doen om je algoritme te controleren. Kies een nieuwe target plek en hoek waar je het papiertje neerzet. We raden je aan om minstens twee meetseries te doen met verschillende locaties. Deze meetseries kunnen verwerkt worden bij opdracht 9 in de template.

### Decision
Is je algoritme goed genoeg, of valt er nog wat te verbeteren? Kan je het aantal benodigde metingen nog omlaag brengen? Als je algoritme nog verbeteringen nodig heeft, kopieer cellen vanaf opdracht 8 en 9. Plaats deze onder opdracht 9 in de template en maak daarin de volgende iteratie. 

Is je algoritme klaar dan ga je hieronder door.

## Algoritme aan TA laten zien
Hierboven heb je als het goed is een aantal keren ge-itereerd.
**Als je tevreden bent met je algoritme roep je je TA erbij en laat deze meekijken met de laatste versie van je algoritme. Als je TA tevreden is met jullie algoritme krijg je van je TA een locaties voor het papier.**
Doe metingen op deze locatie en voer je algortime voor de laatste keer uit. Gebruik hier bij Opdracht 10 in de template.

# Leerdoel: ontwerpcyclus
Om te laten zien dat je begrepen hebt hoe je vandaag met de ontwerpcyclus om moet gaan, zet je bij opdracht 11 in de template: onder elkaar alle blokkenschema's van alle versies van je algoritme. Zet ze in de goede volgorde (op tijd). Licht hierbij de gemaakte evaluaties en beslissingen kort toe. Dit, samen met het resultaat dat het gelukt is hierboven, laat zien dat je het leerdoel voor vandaag onder de knie hebt.

## Inleveren
Als je helemaal klaar bent kan je je uiteindelijke versie inleveren.

Controleer eerst nog goed of alles klopt. **Klik boven op Kernel -> Restart and Run all en check of er geen errors zijn.** Zorg dat alle benodigde bestanden zijn geüpload in vocareum en dat de afbeeldingen zichtbaar zijn in het notebook.

Als je helemaal klaar bent kan het notebook worden ingeleverd door bovenaan op submit te klikken. Je kan meerdere keren iets inleveren, alleen de laatste versie wordt dan bewaard.
   