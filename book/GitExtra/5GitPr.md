# Git Pull Request

Met een *Pull Request* vraag je aan je samenwerkers (in bij DEF: aan je hoofdTAs) toestemming om de wijzigingen in jouw *branch* toe te voegen aan de *branch* waar de *pull request* naar toe gaat, in ons geval de `inprogress` *branch*.
Om nu jullie opdracht na te laten kijken en terug te *mergen* met jullie `inprogress` *branch* gaan we een *pull request* (PR) doen.
De *pull request* doe je als je klaar bent met de opdracht.
GitHub kijkt dan of alles klopt en runt checks die wij hebben toegevoegd.

## Nakijken

Om na te kijken gebruiken wij het review-systeem van Git in de *PRs*.
Als de *PR* is aangemaakt kan je rechts bovenin een *reviewer* aanklikken en zet je de link van de *PR* in de bijbehorende assignment op Brightspace.
De reviewer moet jullie TA worden, deze gaat dan nakijken en laat wat comments achter en vraagt misschien om verandering als we vinden dat het nog niet helemaal correct is.
Als dit zo is, dan moeten jullie aanpassingen gaan maken, dit kan gewoon weer in dezelfde *branch* met nieuwe *commits* (vb: commentaar verwerken).
Zodra je alles hebt verbeterd, vraag je opnieuw de review aan van je TA.

Op Brightspace houden we uiteindelijk bij of de opdracht namelijk succesvol is afgerond

## Voorbeeld

Nu alles is gesynct op mijn GitHub account ga ik een *pull request* doen van mijn `opdracht` branch naar `inprogress`.

1. Ik klik op 'Compare & pull request': 

![Pull request starten.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/6_1_compare.png)

2. Nu zijn we in het *pull request* menu: 

![Pull request menu.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/6_2_in_pr.png)

3. We moeten zorgen dat we **niet** een *PR* openen naar de DEF-D opdrachten *repo*, maar naar jouw eigen `inprogress` *branch*, dit doe je hier: 

![Base veranderen naar jouw eigen `inprogress` branch.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/6_3_verander_base_repo.png)

![Base veranderen naar jouw eigen `inprogress` branch deel 2.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/6_3_5_verander_base_repo.png)


4. Bij *reviewers* moet je jouw nakijker toevoegen, in mijn geval is dit hoofdTA: MartijnSonneveld.
   - Je hoort op de dag zelf wie jouw nakijker is.
5. Zet nu de link van jouw *PR* op de juiste plek in Brightspace.
    - Voor DEF-D moet je meestal zodra je je *pull request* hebt aangemaakt dit op Brightspace melden in een assignment. Dat is belangrijk om voor je DEF-D onderwijs je punten te krijgen. Dat doe je door de URL/link te kopieren. Dus de link van de pagina van je *PR* to kopiëren en die te plakken in de juiste assignment op Brightspace.
6. Martijn heeft nagekeken en was niet tevreden: 

![Feedback: niet goed genoeg.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/6_4_review_niet_geaccepteerd.png)

7. Ik maak veranderingen en commit en push die, daarna kan ik nog een review aanvragen van Martijn: 

![Nieuwe review aanmaken.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/6_5_rerequest_review.png)

8. Deze keer vond Martijn het goed!

![Feedback: goed gekeurd.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/6_6_feedback_verwerkt.png) 

Nu willen we mergen met de `inprogress` *branch*, *squash & merge* om precies te zijn!
    
Nu het is goedgekeurd door de TA en zal hij zorgen dat alles op jullie `inprogress` *branch* komt!
Dit doet hij door deze stappen te volgen:

- ![Branches mergen.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/6_7_merge.png)

- ![Squash mergen selecteren.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/6_8_squash_merge.png)

- Dan kunnen we de *branch* deleten: 

![De branch verwijderen.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/6_9_delete_branch.png)
 
### Automatische Checks

Wij hebben een paar automatische checks toegevoegd, de TA's kijken pas na als al die checks zijn goed gegaan.
Vraag dus ook pas voor een review als de checks goed zijn gekeurd. 
Als de checks niet goed zijn, lees goed wat er mis is, pas dat aan in je opdracht, *commit & push* opnieuw, dan gaan de checks opnieuw kijken of het nu wel in orde is.

![Checks zijn niet goed.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/automatische_check_niet_blij.png)

![De checks zijn goed.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/automatische_check_wel_blij.png)

### Deel je werk met je groepsgenoot

Als je je werk wilt delen met je groepsgenoten, zodat hun *repo* ook geüpdate is met jullie opdracht, kan dit ook via een *PR*.
Maak dus nog een *PR* aan vanuit jouw *branch* waar je in hebt gewerkt, naar de `inprogress` branch van de forks van je groepsgenoten.
1. Maak dus nog een *PR* aan en kies hier je groepsgenoten: 

![Werk delen met je groepsgenoot.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/6_10_deel_met_medestudenten.png)

2. Mijn groepsgenoot is Danielle, ik push mijn `opdracht` *branch* naar haar `inprogress` *branch*: 

![Pull request naar je medestudent.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/6_11_pr_groepsgenoot.png)

3. Zij moet dan ook de reviewer zijn, samen met de hoofdTA, en de *PR* pas accepteren als de TA de normale *PR* heeft goedgekeurd.