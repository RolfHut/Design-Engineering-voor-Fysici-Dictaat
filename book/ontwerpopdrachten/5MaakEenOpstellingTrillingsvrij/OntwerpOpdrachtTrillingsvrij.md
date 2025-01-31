# Parametrisch ontwerpen: Maak een meetopstelling trillingsvrij
De leerdoelen voor vandaag zijn:

- Inzien dat de parameters in een differentiaalvergelijking ontwerpparameters zijn die een ontwerpruimte opspannen.
- Op basis van een differentiaal vergelijking een keuze maken voor parameters en die vervolgens kunnen vertalen in een fysiek ontwerp.

Om die leerdoelen onder de knie te krijgen gaan jullie een opstelling maken die in staat is om een gevoelige meetopstelling te isoleren van trillingen van de buitenwereld. Je gaat dat doen door parametrisch te ontwerpen: we reduceren het ontwerpprobleem tot een gering aantal fysische parameters die we kunnen controleren. Dit notebook helpt je daar stap voor stap doorheen. Je moet meerdere dingen inleveren:

##### voor de lunch (sanity checks, aan je TA laten zien):
- een berekende grafiek die je bij je ontwerp nodig hebt (zie onder)
- laat zien dat je de Arduino werkend aangesloten hebt.

##### voor einde van de dag (ontwerpopdracht)
- dit notebook op Vocareum
- Een video bestand (liefst gif!) met een video die laat zien dat je opstelling 'werkt', op Brightspace
- je samenwerken feedback logboek op Brightspace.

### Groep aanmelden 
Deze opdracht doe je in groepen van 3 studenten. Je kan je groepsnummer en je medestudenten vinden op Brightspace onder Groups: ontwerpopdracht 5: Maak een meetopstelling trillingsvrij. Ga in vocareum naar het juiste notebook  (link op brightspace) en geef met de knop 'Send Invite' je groepsgenoten aan zodat jullie gezamelijk in dezelfde notebook kunnen werken. Uiteindelijk lever je dit notebook als groep in via Vocareum door op submit te klikken.

**Laat voor 11:00 aan je TA zien dat je succesvol samen in een groep zit!**

Als je groep om 11.00 niet compleet is, trek dan aan de bel door je TA erbij te roepen. Wij komen dan kijken wie er mist en schuiven met studenten in incomplete groepen om jullie in volledige groepen te krijgen.

### Samenwerken in Vocareum 
Om vertragingen en mogelijk verlies van werk te voorkomen is het essentieel om niet tegelijk in Vocareum te werken. Wat je het beste kan doen:
- Één student opent het notebook. Een andere student werkt met de Arduino.
- Als je grote bestanden wilt delen (video), doe dat dan via wetransfer of soortgelijke services. De student die Vocareum 'bedient' haalt de bestanden op en voegt ze aan het noteboek toe. Doe dit via 'control panel', dan 'my server' en dan 'upload'. Bestanden gedeeld via WhatsApp worden gecomprimeerd en kunnen dan essentiele details verliezen.
- Als je meetgegevens wilt delen, type die dan als bericht / email naar elkaar.

### Samenwerken
Overleg bij alles wat je in het notebook invult met je team: wat je inlevert is van jullie alle drie. Je zal dus goed moeten samenwerken. Jullie hebben allemaal als het goed is het hele notebook doorgelezen. Maak nu samen een planning waarin je aangeeft

- Hoe laat je bij de mijlpalen verwacht te zijn. Als je een mijlpaal niet haalt omdat je vast zit is het een goed idee om je TA om hulp te vragen
- Bij opsplitsen: wie welke actie gaat doen en hoe laat die klaar gaan zijn.
- Op welke tijden je als team pauzes neemt. Continu werken is niet effectief.

Vul bij opdracht 1 in de template de tabel in (en eventueel aan als je meer regels nodig hebt). **Laat de planning aan je TA zien. **De planning moet uiterlijk om **11.00** gezien zijn.

Jullie keuzes in de ontwerpcyclus kunnen betekenen dat je hieronder zelf cellen toevoegt of verwijdert aan het template. Dat is prima, zolang je ons maar laat zien welke ontwerpstappen je genomen hebt. Dus niet het notebook aan het einde van de rit invullen, maar gedurende het ontwerpen en maken continue invullen en aanpassen waar nodig. Succes!

## Opsplitsen: twee taken
Als voorbereiding ga je opsplitsen: één teamlid doet taak 1. Twee teamleden doen taak 2. Zodra je daarmee klaar bent heb je groepsoverleg waar je belangrijke beslissingen samen neemt. 

### Taak 1: sanity check Arduino & Processing software
Bekijk dit filmpje: [https://www.youtube.com/watch?v=VqTxH3CenRw](https://www.youtube.com/watch?v=VqTxH3CenRw) (link ook op Brightspace) waarin de docent uitlegt hoe je twee acceleratiemeters aansluit op je Arduino en een meting doet. **De docent zegt hierin dat je een video moet maken, dat hoeft niet meer. Deze youtube is uit de corona-tijd, je kan nu aan je TA laten zien dat het werkt!** Aan het einde moet je aan je groepsgenoten vertellen: 

- hoe makkelijk of moeilijk de setup is om mee te werken.
- hoe lang je verwacht dat het duurt om één meting te doen.
- welke nauwkeurigheid je verwacht te kunnen halen.

### Taak 2: ontwerp-eis omrekenen naar parameters

De tweede en derde student gaan Het volgende uitwerken bij opdracht 2 in de template.

## Analyse: Bepalen parameters\n",
In de analyse fase van ontwerpen gaat het om het uitwerken van de opdracht (of de wensen van de klant binnen een bedrijf) tot criteria waar het ontwerp aan moet voldoen. Dit dient dan als input voor de volgende fase: synthese, waarin je ideeen gaat bedenken. Bij parametrisch ontwerpen gebruik je de analyse fase om te bepalen welke parameters belangrijk zijn, hoe deze je ontwerp beinvloeden en tot slot wat de eisen aan deze parameters zijn. Dat gaan we hier ook stap voor stap doen.

De parameters waar je als ontwerper invloed op hebt in dit ontwerp zijn massa (m) en veerconstante (C). Denk terug aan het college en zie eventueel deze [video over theorie op Youtube](https://www.youtube.com/watch?v=XDLgnwhsOfM). De eisen aan het ontwerp zijn dat een trilling van 5Hz gedempt wordt met een factor 3 en dat deze op het horizontale vlak stabiel is. Reken uit welke kantelfrequentie (ook wel cut-off frequency of Eigen frequency) het massa-veer-systeem dat je gaat ontwerpen moet hebben. Schrijf dit op in de template.
   
Plot vervolgens hieronder hoe de amplitude overdracht ($\\left|\\frac{A_{out}}{A_{in}}\\right|$ in het college) voor je berekende kantelfrequentie afhangt van de frequentie van de trilling van de vloer ($f_{0}$). Zorg dat de x-as uitgedrukt is in Hz en plot beide assen op een logaritmische schaal. Dit soort grafieken heet een 'Bode plot' en heb je al een keer gezien bij het vak voortgezette analyse en het Natuurkundig Practicum. "



