## Oefen vraag: vermogen
Studenten willen hoeveel energie nodig om liter water te koken bepalen met onzekerheid van minder dan $5$%. 
Ze hebben waterkoker, twee multimeters en een stopwatch. 
Multimeters voor V en I hebben $2$% onzekerheid. Hoe nauwkeurig (in procenten) moet de stopwatch zijn?

### Antwoord
De formule voor vermogen is $P = V I$.
De formule voor energie is $E = P / t$
Dus $E = \frac{V I}{t}$
De fout in de energie is dan: $(\frac{u(E)}{E})^2 = (\frac{u(V)}{V})^2 + (\frac{u(I)}{I})^2 + (\frac{u(t)}{t})^2$

Wat we willen is dat de fout in de energie kleiner is dan $5$%, dus $(\frac{u(E)}{E}) \leq 5$%.

Dan krijgen we: $\sqrt{(\frac{u(V)}{V})^2 + (\frac{u(I)}{I})^2 + (\frac{u(t)}{t})^2} \leq 0.05$

Dit is hetzelfde als: $(\frac{u(V)}{V})^2 + (\frac{u(I)}{I})^2 + (\frac{u(t)}{t})^2 \leq (0.05)^2$

Dus we krijgen: $(\frac{u(t)}{t})^2 \leq (0.05)^2 - (\frac{u(V)}{V})^2 - (\frac{u(I)}{I})^2$

Invullen geeft: 
$(\frac{u(t)}{t})^2 \leq (0.05)^2 - (0.02)^2 - (0.02)^2$
Dus $(\frac{u(t)}{t})^2 \leq 0.0017$.

Met als eind antwoord: $(\frac{u(t)}{t}) \leq 0.041$ 
Dus minder dan $4.1$%.
