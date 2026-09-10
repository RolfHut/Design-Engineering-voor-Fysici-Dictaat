# Forking

Een *repository* (*repo*) *clonen* is handig om er zelf op jouw laptop aan te werken, maar hoe deel je nu wat jij hebt gedaan met je groepsgenoot?
Dit gaan we oplossen door de opdrachten eerst te *forken* naar je eigen GitHub-account.
In essentie kopiëer je dus eerst de *repo* naar jouw account en van daar *clone* je hem naar je eigen laptop. 
Dit betekent dat een kopie van de *repo*, met alle notebooks, daadwerkelijk op de harde schijf van jouw laptop staat en je eraan kan werken als je laptop niet met internet verbonden is. 
Je kan er dan aan werken in welke omgeving je wilt, veel van jullie gebruiken daarvoor VSCode.

Waarom? Nu kan je samen met je groepsgenoot werken aan de opdracht. Jullie hebben dezelfde *fork*, maar werken in je eigen *clone*. 
Zodra je een stuk werk af hebt kan je dat via GitHub makkelijk delen, want de github.com website houdt een versie van jullie *fork* bij. 
Het is natuurlijk niet de bedoeling dat jullie jullie werk *pushen* naar de DEF *repo* ;)

***Forken* doen we maar 1 keer!**
Dit zal voor de meeste op de kickoff dag gebeuren.

## Voorbeeld

We beginnen op de [DEF-D opdracht repo](https://github.com/Design-Engineering-voor-Fysici/opdrachten-DEF-D), deze gaan jullie *forken*.
*Forken* staat rechtsbovenin aangegeven:

![*Fork*: waar doe je dat.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main/figures/git/1_1_start_fork.png)

Klik op `Fork` dan kom je hier.

![De *fork* starten](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/1_2_create_fork.png)

Let op dat je **alleen** de main *branch* *forked* naar jouw account, verzin een *repo* naam en `Create fork`, ik hou de naam hetzelfde: 'opdrachten-DEF-D'.

Nice, je hebt nu de DEF *repo* op je eigen account!
Het zou er nu zo uit moeten zien, dan kan je door naar het volgende onderdeel.

![*Forken* is gelukt.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/1_3_forken_succeeded.png)

Dit is een andere manier om de *repo* te *clonen* van wat je [eerder hebt geleerd bij IP](https://contemporary-physicslab.github.io/thermolab/intro-1/).

**LEAVE NOOIT DE FORK**

### Collaborators toevoegen

Nodig nu je groepsgenoot uit voor jouw *repo*, of accepteer die van je groepsgenoot, mits dit nodig is.
**Nodig ook de 3 hoofdTA's uit**, dit is belangrijk voor nakijken later!
Hoe dit moet staat [hier](https://contemporary-physicslab.github.io/thermolab/intro-1/#je-partner-s-uitnodigen), bij `settings` zie je een tab *collaborators*.


#### hoofdTA GitHub accounts

- Martijn Sonneveld: MartijnSonneveld
- Sjoerd Hoogeman: SHoogeman

Als je het niet zeker weet, dan kan je [hier](https://github.com/orgs/Design-Engineering-voor-Fysici/teams/hoofd-ta/members) de hoofd TA's zien.


### Actions aanzetten

We hebben een aantal GitHub *actions* gemaakt die jullie gaan helpen: automatische checks. 
Deze moet je wel even aanzetten op je eigen Github page, zie dit screenshot:

![GitHub actions.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/1_4_actions.png)

En enable de workflows.

### Protecting main

Een goede eigenschap is om je main *branch* te *protecten*.
Zo bescherm je je werk waarvan je zeker weet dat het werkt! (Denk aan AWS die laatst omviel...)
Ook helpt het om kleine foutjes te spotten die jou zijn ontgaan.

Dit zorgt er ook voor dat je met *branches* moet werken!
Hiervoor gaan we op de GitHub page naar `settings --> branches --> Add branch rule`.

![Start van: protecting main.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/protect_main_1.png)

Druk op `Add branch rule`, geef de goede 'Ruleset Name', zet hem op active en geef de juiste branch targeting criteria, zet deze op default:

![Protecting main aanmaken.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/protect_main_2.png)

Scroll dan naar beneden en vink aan: 'Require a pull request before merging' en zet Required approvals op 1:

![Protecting main settings.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/protect_main_3.png)

Druk dan op `Create`!
