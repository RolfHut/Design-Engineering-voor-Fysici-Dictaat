# Programmeren deel 2

Het programma Button is meer uitgebreid dan we eerder hebben gezien.
We gaan stap voor stap door het programma.

We hebben te maken met twee poorten waar iets moet gebeuren. 
Pin 2 wordt uit gelezen en pin 13 moet een uitvoer zijn. 
De waarden van de pin moet niet veranderen. 
Dit is een constante (const). 
Het is een gehele waarde, een integer (int).
We geven pin 2 een herkenbare naam, pin 2 heet nu buttonPin. 
Pin 13 heeft de naam ledPin gekregen.
```
const int buttonPin = 2;
const int ledPin = 13;
```

We willen straks weten wat ‘de staat’ van de knop is. 
Deze kan 1 of 0 zijn. 
We moeten even vertellen dat we de staat van de knop willen weten en straks willen vergelijken. 
Voordat we het programma laten draaien is de buttonState 0.
```
int buttonState = 0;
```

Zoals gezegd, we moeten even vertellen dat de ledPin een OUTPUT is en de buttonPin een INPUT. 
Zo, dat weten ze nu dan ook…
```
void setup(){
    pinMode(ledPin, OUTPUT);
    pinMode(buttonPin, INPUT);
}
```

Er moet iets gebeuren als de knop wordt ingedrukt. 
Aan het begin van de loop wordt de knop dus uitgelezen(eigenlijk wordt er dus alleen gecontroleerd of er een 5,0 V spanning over de weerstand staat). 
Daarna volgt een **if**-statement. 
Als (**if**) de knop is ingedrukt (buttonState == HIGH) dan moet de LED gaan branden(digitalWrite(ledPin, HIGH);). 
In alle andere gevallen (**else**), moet de LED niet branden (digitalWrite(ledPin,LOW);).
```
void loop(){
    buttonState = digitalRead(buttonPin);
    if (buttonState == HIGH){
        digitalWrite(ledPin, HIGH);
    }
    else{
        digitalWrite(ledPin, LOW);
    }
}
```

Het is een makkelijk if-statement. 
Je kan ook meerdere voorwaarden stellen. 
Als je twee knoppen tegelijk in moet drukken voordat de LED gaat branden zet je && tussen de tekens (if buttonState1 == HIGH && buttonState 2 ==HIGH){}). 
Je kan ook het teken || gebruiken. Dan moet of de ene voorwaarde gelden of de andere.
```
void loop(){
    buttonState = digitalRead(buttonPin);
    if (buttonState == HIGH && state == LOW){
        state = HIGH;
    }
    if (buttonState == HIGH && state == HIGH){
        state = LOW;
    }
    digitalWrite(ledPin,state);
    delay (100);
}
```

Helaas blijft het lampje nu niet branden. 
Je kan er wel voor zorgen dat je met één knop het lampje aan en uit kan zetten. 

Vergeet niet de nieuwe variabele (int) te definiëren aan het begin!
