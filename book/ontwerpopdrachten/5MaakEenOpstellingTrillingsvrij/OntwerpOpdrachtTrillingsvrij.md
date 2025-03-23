# 5. Maak een meetopstelling trillingsvrij
De leerdoelen voor vandaag zijn:

- Inzien dat de parameters in een differentiaalvergelijking ontwerpparameters zijn die een ontwerpruimte opspannen.
- Op basis van een differentiaal vergelijking een keuze maken voor parameters en die vervolgens kunnen vertalen in een fysiek ontwerp.

Om die leerdoelen onder de knie te krijgen gaan jullie een opstelling maken die in staat is om een gevoelige meetopstelling te isoleren van trillingen van de buitenwereld. Je gaat dat doen door parametrisch te ontwerpen: we reduceren het ontwerpprobleem tot een gering aantal fysische parameters die we kunnen controleren. Dit notebook helpt je daar stap voor stap doorheen. Je moet meerdere dingen inleveren:

##### voor de lunch (sanity checks, aan je TA laten zien):
- een berekende grafiek die je bij je ontwerp nodig hebt (zie onder)
- laat zien dat je de Arduino werkend aangesloten hebt.

##### voor einde van de dag (ontwerpopdracht)
- het [invul template ](OntwerpopdrachtMaakEenOpstellingTrillingsvrijInvulTemplate.ipynb) op vocareum
- Een video bestand (liefst gif!) met een video die laat zien dat je opstelling 'werkt', op Brightspace
- je samenwerken feedback logboek op Brightspace.

### Groep vormen 
Deze opdracht doe je in groepen van 3 studenten. Je kan je groepsnummer en je medestudenten vinden op Brightspace onder Groups: ontwerpopdracht 5: Maak een meetopstelling trillingsvrij. Net als in vorige weken hebben we [een invultemplate notebook](OntwerpopdrachtMaakEenOpstellingTrillingsvrijInvulTemplate.ipynb) dat je gedurende de dag bij houdt. Aan het einde van de dag ga je via de link op Brightspace naar Vocareum. Dat staat aan het einde van dit document uitgelegd. 

**Als je groep om 11.00 niet compleet is, trek dan aan de bel door je TA erbij te roepen.** Wij komen dan kijken wie er mist en schuiven met studenten in incomplete groepen om jullie in volledige groepen te krijgen.

### Laptops 
Net als vorige week werk je met twee laptops en één fysiek notebook. Op een van de notebooks open je de Arduino software en Processing. Op de andere laptop open je [het invultemplate notebook](OntwerpopdrachtMaakEenOpstellingTrillingsvrijInvulTemplate.ipynb). We willen, net als vorige week, geen andere applicaties of websites open zien staan (met uitzondering van de youtube video hieronder).

### Samenwerken
Overleg bij alles wat je in het notebook invult met je team: wat je inlevert is van jullie alle drie. Je zal dus goed moeten samenwerken. Jullie hebben allemaal als het goed is het hele notebook doorgelezen. Maak nu samen een planning waarin je aangeeft

- Hoe laat je bij de mijlpalen verwacht te zijn. Als je een mijlpaal niet haalt omdat je vast zit is het een goed idee om je TA om hulp te vragen
- Bij opsplitsen: wie welke actie gaat doen en hoe laat die klaar gaan zijn.
- Op welke tijden je als team pauzes neemt. Continu werken is niet effectief.

Vul bij *opdracht 1* in de template de tabel in (en eventueel aan als je meer regels nodig hebt). **Laat de planning aan je TA zien. **De planning moet uiterlijk om **11.00** gezien zijn.

Jullie keuzes in de ontwerpcyclus kunnen betekenen dat je in het template zelf cellen toevoegt of verwijdert aan het template. Dat is prima, zolang je ons maar laat zien welke ontwerpstappen je genomen hebt. Dus niet het notebook aan het einde van de rit invullen, maar gedurende het ontwerpen en maken continue invullen en aanpassen waar nodig. Succes!

## Opsplitsen: twee taken
Als voorbereiding ga je opsplitsen: één teamlid doet taak 1. Twee teamleden doen taak 2. Zodra je daarmee klaar bent heb je groepsoverleg waar je belangrijke beslissingen samen neemt. 

### Taak 1: sanity check Arduino & Processing software
Bekijk dit filmpje: [https://www.youtube.com/watch?v=VqTxH3CenRw](https://www.youtube.com/watch?v=VqTxH3CenRw) (link ook op Brightspace) waarin de docent uitlegt hoe je twee acceleratiemeters aansluit op je Arduino en een meting doet. **De docent zegt hierin dat je een video moet maken, dat hoeft niet meer. Deze youtube is uit de corona-tijd, je kan nu aan je TA laten zien dat het werkt! Aan het einde van de dag maak je wel een video van je totale opstelling** Aan het einde moet je aan je groepsgenoten vertellen en bij *opdracht 2a* in het invultemplate invullen: 

- hoe makkelijk of moeilijk de setup is om mee te werken.
- hoe lang je verwacht dat het duurt om één meting te doen.
- welke nauwkeurigheid je verwacht te kunnen halen.

### Taak 2: ontwerp-eis omrekenen naar parameters

De tweede en derde student gaan Het onderstaande tot 'Groepsoverleg' uitwerken bij *opdracht 2b* in de template.

## Analyse: Bepalen parameters
In de analyse fase van ontwerpen gaat het om het uitwerken van de opdracht (of de wensen van de klant binnen een bedrijf) tot criteria waar het ontwerp aan moet voldoen. Dit dient dan als input voor de volgende fase: synthese, waarin je ideeen gaat bedenken. Bij parametrisch ontwerpen gebruik je de analyse fase om te bepalen welke parameters belangrijk zijn, hoe deze je ontwerp beinvloeden en tot slot wat de eisen aan deze parameters zijn. Dat gaan we hier ook stap voor stap doen.

De parameters waar je als ontwerper invloed op hebt in dit ontwerp zijn massa (m) en veerconstante (C). Denk terug aan het college en zie eventueel deze [video over theorie op Youtube](https://www.youtube.com/watch?v=XDLgnwhsOfM). De eisen aan het ontwerp zijn dat een trilling van 5Hz gedempt wordt met een factor 3 en dat deze op het horizontale vlak stabiel is. Reken uit welke kantelfrequentie (ook wel cut-off frequency of Eigen frequency) het massa-veer-systeem dat je gaat ontwerpen moet hebben. Schrijf dit op in de template.
   
Plot vervolgens in het template hoe de amplitude overdracht ($\left|\frac{A_{out}}{A_{in}}\right|$ in het college) voor je berekende kantelfrequentie afhangt van de frequentie van de trilling van de vloer ($f_{0}$). Zorg dat de x-as uitgedrukt is in Hz en plot beide assen op een logaritmische schaal. Dit soort grafieken heet een 'Bode plot' en heb je al een keer gezien bij het vak voortgezette analyse en het Natuurkundig Practicum. 

In het college hebben we laten zien dat je een gegeven kantelfrequentie ook kan omrekenen tot een $\Delta x$, het verschil in lengte van de veer tussen de situaties wanneer je de massa er volledig afhaalt en wanneer je deze terug zet. Bereken in het template wat de minimale $\Delta x$ is die je nodig hebt om aan de ontwerpeis te voldoen.

De berekende $\Delta x$ is het grensgeval waar je opstelling net aan de eisen voldoet. Echter: als je gaat bouwen heb je te maken met onnauwkeurigheden in je constructie: is bijvoorbeeld $\Delta x$ wel precies gemeten? Verder is de formule die we gebruiken een benadering: zo verwaarlozen we het effect van demping. Het is dus handig om in je ontwerp te mikken op een veiligere $\Delta x$ dan precies op de grens van de eis. 

Plot bij opdracht 3 in de template een grafiek voor de door jouw berekende $\Delta x$ waar je massa op de x-as en veerconstante op de y-as zet. Zet in dezelfde grafiek ook lijnen die horen bij een twee keer zo grote en vijf keer zo grote $\Delta x$. Zorg voor goede labels bij de verschillende lijnen. **Laat je grafiek aan je TA zien.**"
   
In jullie plot kan je zelf zien wat je moet doen om een hogere $\Delta x$ te bereiken en zo dus een lagere kantelfrequentie en dus een lagere amplitude overdracht bij een gegeven verstoringsfrequentie te halen. Je kan twee dingen veranderen om je $\Delta x$ te verhogen. Geef die aan bij opdracht 4 in de template.

## Groepsoverleg en laten zien sanity check
Als je jullie twee taken hebt uitgevoerd kom je als groep samen om te beslissen op welke $\Delta x$ je gaat mikken in jullie ontwerp. Eerst presenteer je aan elkaar kort je bevindingen van je individuele taak. Daarna neem je als groep een beslissing: op welke $\Delta x$ ga je mikken in je ontwerp. Noteer hieronder je beslissing en **laat aan je TA zien**:

- Je werkende Arduino opstelling
- de grafiek van $\Delta x$ die je hierboven gemaakt hebt. 

Leg deze keuze vast bij opdracht 4 in de template.
## Synthese
Je weet nu welke $\Delta x$ je minimaal dient te bereiken. Rekening houdend met de materialen die je voorhande hebt: Maak een schets van je beoogde massa-veer systeem. Denk daarbij aan:

- wat ga je als veer / verend materiaal gebruiken. (dus niet: welke veerconstante, maar: welk fysiek ding ga je als veer / verend materiaal gebruiken?)
- wat ga je als massa gebruiken (dus niet: hoe zwaar is dat ding, maar: welk ding)
- hoe ga je je massa aan je veer bevestigen?

Vervang bij opdracht 5 het TU Delft logo in de template door jullie schets.

## Simulatie
Voordat je je massa-veer systeem gaat bouwen doe je eerst een simulatie: test of je $\Delta x$ gehaald hebt. Bevestig zo snel en makkelijk mogelijk je massa aan je veer / verend materiaal. **Bouw dus nog niet de hele opstelling, maar test alleen de massa en veer. Dit moet niet meer dan 5 minuten duren.** Wordt de veer met minimaal $\Delta x$ ingeduwd of uitgerekt? **Laat dit aan je TA zien** voordat je verder gaat met je hele opstelling bouwen!"

## Evaluatie en Beslissing
Vul de evaluatie en beslissing in bij opdracht 6 in de template.

## Fabricage
Maak nu het massa-veer systeem dat je ontworpen had. **Laat voordat je gaat meten je opstelling aan je TA zien.** (als je TA druk is, begin met meten, maar zorg wel dat je TA je opstelling gezien heeft, anders krijg je misschien te laat te horen dat er iets niet in orde is!)"
   
## Evaluatie
Nu gaan jullie meten of het daadwerkelijk gelukt is de amplitude-overdracht die geëist is te behalen.

#### extra sanity check
De metingen kunnen best tijdrovend zijn. Als sanity-check: til je massa op (of duw hem omhoog) totdat je veer / verend materiaal niet meer onder spanning staat. Heb je je beoogde $\Delta x$ gehaald? Zo niet, ga dan snel je opstelling verbeteren (stappen terug in de ontwerp cyclus) tot dit wel gelukt is. Denk aan de grafiek van veerconstante versus massa: wat kan je doen om in jouw ontwerp $\Delta x$ groter en dus de kantelfrequentie lager te maken?

### Meetplan
Je gaat bij verschillende meting doen van het gedrag van je opstelling. De frequenties die ik aanraad dat je doet zijn ongeveer de volgende, maar misschien wil je dit op basis van je ontwerp aanpassen. Als je dat doet: prima. Je mag (natuurlijk) meer metingen doen, maar drie is het minimum. Zorg er altijd voor dat je zowel lager, als hoger, dan je kantelfrequentie minimaal één meting hebt en zorg ervoor dat op basis van je metingen geconcludeerd kan worden dat je opstelling aan de eis van een factor 3 amplitude afname bij 5Hz voldoet

- 1 Hz of 60 beats per minute (bpm)
- 3 Hz of 180 bpm
- 5 Hz of 300 bpm (of zo dicht bij als het je lukt te komen, dit is heel snel)

### Metingen doen
In het college en in de videos is uitgelegd hoe je metingen kan doen met je Arduino en de amplitude overdracht kan bepalen. 

#### filmpje resultaat
Je moet een filmpje maken van je opstelling en je meting op je scherm. Doe dit bij een frequentie die hoger (sneller) is dan de eis, of bij een lagere frequentie waarbij je de factor van 3 in ampliture afname al haalt. Dan kunnen we namelijk in het filmpje zien dat jullie opstelling 'werkt' volgens de eis. Zorg ervoor dat je filmpje niet langer dan 30 seconden is (en liefst korter)

**Dit filmpje lever je op Brightspace in, niet naar Vocareum uploaden!**

### Resultaat metingen
Maak opnieuw de grafiek van amplitude overdracht versus frequentie die je aan het einde van Evaluatie ook gemaakt hebt (dus met twee overdrachten) en voeg daar je meetpunten aan toe. Doe dit bij opdracht 7 in de template. 
   
### Iteratie?
Kijk of het nodig is om nog een iteratie te doen. Dat kan het geval zijn als:

- Jullie opstelling nog niet aan de minimale eis voldoet. 
- Door verbeteringen toe te voegen (of weg te halen!) tot een nog beter resultaat gaat leiden en er nog genoeg tijd is om deze verbeteringen aan te brengen.

Als je gaat itereren, kopieer dan benodigde cellen in het template. Leg goed je proces vast in het template zodat wij zien wat je gedaan hebt. Lever sowieso een foto, met korte beschrijving, van je uiteindelijke opstelling in zodat we kunnen zien wat er gemaakt is.

## Leerdoelen
Lees de leerdoelen nog eens terug. In de cel bij opdracht 8 in de template kan je met twee grafieken die je vandaag als het goed is al gemaakt heb laten zien dat je de leerdoelen onder de knie hebt. Als je de grafieken als figuren hebt opgeslagen, kan je deze makkelijk bij opdracht 8 in het template invoegen zonder exta python te hoeven schrijven of kopieren. Je kan ze ook opnieuw uitrekenen, maar let dan heel goed op dat door de code te runnen je misschien niet precies dezelfde resultaten als erboven krijgt wanneer je niet netjes hebt geprogammeerd met namen van variabellen.
      
## Inleveren resultaten
Als alles gelukt is, kan je je resultaten inleveren. **Laat voordat je dit doet je resultaten aan je TA zien ter controle!**

- Controleer eerst nog goed of alles klopt. Klik boven in het template op Kernel -> Restart and Run all en check of er geen errors zijn. 
- Één student opent de opdracht in Vocareum en nodigt de andere twee studenten uit.
- upload het template en alle bestanden die nodig zijn naar vocareum
- klik ook in Vocareum op op Kernel -> Restart and Run all en controleer of alles goed staat
- pas dan klik je op submit en daarna op end lab.

Op Brightspace is een aparte assignment waar je de video moet inleveren. Zet deze video niet bij het template in Vocareum!

## Samenwerking feedback geven, noteren en inleveren
Net als bij elke workshop geef je elkaar weer feedback op de samenwerking. Kijk als nodig nog even de videos daarvan terug. De feedback die je krijgt noteer je in je logboek en dat lever je weer in.

## Opruimen en door TA af laten tekenen dat je weg gaat
Als alles ingeleverd is ruim je je tafel op. **Laat je TA controleren dat je tafel er ok uitziet voordat je weg gaat.**
