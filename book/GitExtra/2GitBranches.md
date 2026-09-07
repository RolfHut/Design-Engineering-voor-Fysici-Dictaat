# Git Branches

Als je de *repo* met de opdracht hebt *geforkt* dan kan je ook alle *branches* mee krijgen, voor DEF-D heb je alleen de *branch main*.
Een *branch* is een kopie van de *repo*, dit kan een kopie zijn van *main*, maar ook weer van een andere *branch*.
Jullie gaan een kopie van *main* maken.
Een *branch* wordt gebruikt om aan verschillende functionaliteiten te werken, voor ons betekent dat: een *branch* voor elke opdracht!
Jullie eerste *branch* zou iets zijn als: `introductie`.
Maak de *branch* voor de opdracht pas aan als je er ook echt aan gaat beginnen.

![Branche voorbeeld.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/2_1_branches.png)
*An illustration of branching in Git. Taken from [here](https://book.the-turing-way.org/reproducible-research/vcs/vcs-git-branches/). Illustration by Scriberia. Used under a CC-BY 4.0 licence. DOI: [The Turing Way Community & Scriberia (2024)](https://zenodo.org/records/13882307).*

## Voorbeeld: Branch maken

Nu je de *repo* op je eigen account hebt *geforkt*, klikken we op de dropdown van de *branches*:

![Branch plek.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/2_2_plek_branches.png)

Eerst maken we een `inprogress` *branch* aan, daar zetten we alle opdrachten in die klaar zijn. 

![Branch aanmaken.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/2_2_5_inprogress.png)

**Switch weer terug naar main.**
Dan om de nieuwe `opdracht` branch aan te maken typen we in de dropdown: 'opdracht' en klikken we: 'create branch'.
Zorg dat je vanuit `main` de opdracht *branch* aanmaakt.

![Branch aanmaken.](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/2_3_maak_branches.png)

In hetzelfde dropdown-menu als eerst kan je nu switchen tussen de *branches*.

> [!NOTE]
> Je zou nu 3 *branches* moeten hebben: `main`, `inprogress` en `<opdracht>`.

## Voorbeeld: naar je branch switchen in VSCode

Om dit in VSCode te doen, gaan we eerst jullie *repo* *clonen* naar VSCode en dan de goeie *branch* in.
Voor een reminder naar hoe je moet *clonen* zie [hier hoe het ook alweer moet](https://contemporary-physicslab.github.io/thermolab/intro-1/).
In de terminal kan je dit typen nadat je *gecloned* hebt: `git checkout <opdracht>`.

Het kan ook via deze manier:

1. ga naar het menu van de *repo* in VSCode:

![Switchen naar de goede branch](https://raw.githubusercontent.com/Design-Engineering-voor-Fysici/plaatjes-DEF/main//figures/git/2_4_howto_switch_to_branch.png)

2. klik dan op de nieuwe `opdracht` branch.

Pas als je in de goede *branch* zit, ga je werken aan je opdracht!

### Terminal (optioneel)

Je kan als je dat wilt ook werken met de command line (ook wel terminal genoemd). 
In dat geval zijn dit de commando's die je gebruikt:

Branch maken en meteen ernaar toe switchen:
`git checkout -b <naam van je nieuwe branch>`.

Anders kan je `git checkout <branchnaam>` gebruiken.
