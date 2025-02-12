# Schattend Rekenen

Als ingenieur is het essentieel om snel qualitatieve inschattingen te kunnen maken. Dit staat bekend als *Fermi schatting* of *schattend rekenen*. Voor wie naast de korte introductie die we binnen Design Engineering voor Fysici aanbieden meer over dit onderwerp wil leren raden we {cite:t}`Mahajan2014` en {cite:t}`Weinstein2008` aan.

## Doel:
Het binnen een ontwerpproces en/of binnen een ontwerpdiscussie snel (=uit het hoofd, dus
zonder rekenmachine en zonder internet) schatten van een grootheid $X$ binnen één orde
grootte, d.w.z. $\frac{1}{3} X \lesssim X_{\text{schat}} \lesssim 3 X$.

## Dit soort dingen moet je gewoon (uit je hoofd) kunnen en weten
Volumes en oppervlakten
* omtrek cirkel met diameter $D = \pi D \approx 3D$
* Oppervlakte cirkel met diameter $D = \frac{\pi}{4} D^2 \approx 0.8D^2$
* Oppervlakte bol met diameter $D = \pi D^2 \approx 3 D^2$
* Volume bol met diameter $D = \frac{\pi}{6}D^3 \approx 0.5D^3 $
* Volume bolschil met diameter D en dikte h $=\pi D^2 \approx 3 D^2 h $
* Volume cilinder met diameter D en hoogte H $= \frac{\pi}{4} D^2 H \approx 0.8 D^2 H$


Schattend (hoofd)rekenen in machten van 10
* $\sqrt{10} \approx 3$
* $\sqrt{3} \approx 1.7$
* $\frac{0.03 * 120 * 75}{0.013} = \frac{3 * 1.2 * 7.5 * 10^{-2} * 10^2 * 10^1}{1.3 * 10^{-2}} \approx \frac{3 * \cancel{1.2} * 7.5 * \cancel{10^{-2}} * \cancel{10^2} * 10^1}{\cancel{1.3} 10^{-2}} \approx 2*10^4$
* $\sqrt{0.005} = \sqrt{50 * 10^{-4}} = \sqrt{50} \sqrt{10^{-4}} \approx 7*10^{-2}$
* $15000^{1/3} = 15^{1/3} 1000^{1/3} \approx 2.5 * 10$ (want $2^3 = 8 < 15$ en $3^3 = 27 > 15$)
* $ln(1000) \approx ln\left( 3^6 \right) \approx ln\left( e^6 \right) \approx 6$ (in de tweede stap hebben we overschat, dus waarschijnlijk wat kleiner)
* $12^{3.5} = 12^3 * \sqrt{12} = 1.2^3 * 10^3 * \sqrt{12} \approx 1.6 * 10^3 * 3.5$ (want $3^2 = 9 < 12$ en $4^2 = 16 > 12$) $\approx 5.5 * 10^3$
* $e^2.5 \approx 3^2.5 \approx 3^2 \sqrt{3} \approx 9 * 1.5$ (want $1^2 = 1 < 3$ en $2^2 = 4 > 3 $) $\approx 13.5$ (maar we hebben overschat, dus waarschijnlijk wat kleiner)
* $(1.002)^3 \approx 1.006$ $\left(\text{want Taylor geeft }(1 + \epsilon)^\alpha \approx 1 + \epsilon \alpha \right)$
* $^{10}log(3000) = ^{10}log(3) + ^{10}log(1000) \approx 0.5 + 3 \approx 3.5$ (want $3 \approx \sqrt{10}$)

## Enkele uitgangspunten bij schattend rekenen

De volgende lijst aan uitgangspunten helpt je om een goede schatting te maken. Deze lijst staat binnen het vak Design Engineering voor Fysici bekend als 'methode Kleijn', naar prof. Chris Kleijn die het gastcollege schattend rekenen voor ingenieurs geeft. 

### Verdeel en heers
Splits een schatting waarbij je je geen enkele voorstelling kunt maken van de te
schatten grootheid op in deel-schattingen, die elk voor zich wél te schatten zijn).
Voorbeeld: soortelijke dichtheid = massa / volume = massa/(LxBxH)

### Kies handige deelschattingen
Splits een schatting op in handig gekozen deel-schattingen, die elk voor zich
makkelijk te schatten zijn.
Voorbeeld:
* massa vel papier = soortelijke dichtheid x L x B x dikte is geen handige keuze,
omdat de soortelijke dichtheid en de dikte moeilijk te schatten zijn.
* massa vel papier = 1/500 van de massa van een pak van 500 vel is veel handiger,
omdat de massa van zo’n pak papier redelijk te schatten is.

### De menselijke maat
Relateer een schatting van (onvoorstelbaar) kleine of grote grootheden aan (beter
te schatten) grootheden die een “menselijke maat” hebben.
Voorbeeld: de dikte van een vel papier is 1/500 van de dikte van een pak papier
met 500 vellen

### Praat met je rechter hersenhelft
1. Doe een beginschatting $X_0$.
2. Vermenigvuldig $X_0$ steeds met een factor 3, totdat je een schatting bereikt die
je “echt niet meer kunt geloven”. Noem dit $X_{max}$.
3. Deel $X_0$ steeds door een factor 3, totdat je een schatting bereikt die je “echt
niet meer kunt geloven”. Noem dit $X_{min}$.
4. Schat $X$ als $X_{schat} = \sqrt{X_{min} X_{max}}$

### Je weet meer dan je weet!
Gebruik grootheden die je wél weet/kent (vaak uit het dagelijks leven) om
onbekende grootheden te schatten.
Voorbeeld: de soortelijke dichtheid van water = $1 \text{ kg}/\text{dm}^3$, de soortelijke dichtheid
van ijzer $= 8 \text{ kg}/\text{dm}^3$. Graniet is zwaarder dan water maar lichter dan ijzer.

### Heb zelfvertrouwen!
Durf te schatten. Je kunt meer dan je denkt en je weet meer dan je weet.
Ontgroei het “er ontbreekt een gegeven dus ik kan de som niet maken” stadium.
