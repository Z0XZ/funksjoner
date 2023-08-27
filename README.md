# Funksjoner i Python

En funksjon i Python er en blokk med kode som kun kjører når man kaller på den.
En funksjon kan motta data (parametre), og den kan returnere data som et resultat.
Vi har tidligere brukt mange av de innebygde funksjonene i Python som `print()`, `input()`, `len()`.

Fordelene med funksjoner:

- **Gjenbruk**: Du kan bruke den samme funksjonen mange ganger i programmet ditt uten å måtte skrive koden på nytt.
- **Ryddighet**: Funksjoner lar deg dele opp programmet ditt i små deler. Dette gjør koden lettere å lese og forstå.
- **Enkel endring**: Hvis du vil endre hvordan en del av programmet fungerer, kan du bare endre funksjonen. Dette betyr at du ikke risikerer å "ødelegge" resten av programmet ditt ved en feiltakelse.

Funksjoner brukes overalt i programmering. De kan være enkle, som å legge sammen to tall, eller veldig kompliserte, som å laste inn en nettside.

## Eksempler

1. **En enkel funksjon**:

```Python
def si_hei():
   print("Hei der!")

si_hei() # Dette sier "Hei der!"
```

2. **Funksjon som sier hei til deg**:

```Python
def si_hei_til(navn):
   print(f"Hei, {navn}!")

si_hei_til("Anna") # Dette vil si "Hei, Anna!"
```

3. **Funksjon som regner ut noe**:

```Python
def pluss(tall1, tall2):
   return tall1 + tall2

resultat = pluss(2, 3) # 'resultat' blir 5
```

## Oppgave 1

Lag en funksjon som tar et navn som input og i tillegg skriver printer litt ekstra tekst over og under hilsenen. Et eksempel på noe som kan printes ut hver gang funksjonen kalles på kan være:

```
"Dette var et veldig trivelig navn"
"Heisann {navn}, kjekt å hilse på deg!"
"Du er velkommen her senere, så ofte du vil :)"
```

Når du har laget funksjonen kan du kalle på den.

## Oppgave 2

Lag en funksjon som tar to tall og sier hvilket som er det største og hvor mye større dette tallet er enn det andre.

## Oppgave 3

Du skal nå lage din helt egen random-funksjon. Funksjonen skal ha én parameter; antall.
Funksjonen skal bruke random-biblioteket til å lage tilfeldige tall. Funksjonen du lager skal gjøre følgende:

1. Bruke `random.randint(0,50)`-funksjonen til å lage et tilfeldig tall mellom 0 og 50 som blir lagret i en variabel
2. Legge til denne verdien til en liste.
3. Fortsette å gjøre dette så mange ganger som argumentet tilsier (kaller man på funksjonen med verdien 20 skal altså prosessen over repeteres 20 ganger).
4. Til slutt skal den ferdige listen returneres av funksjonen.

I programmet du skriver kan du godt også printe ut resultatet av funksjonen for å se at ting fungerer riktig.

## Oppgave 4 - Baklengsfunksjonen

Du skal nå lage en funksjon som tar en tekst som input fra brukeren og printer alt baklengs tilbake. F.eks. om vi putter inn "Heisann!", skal vi få ut "!nnasieH".

For å få til dette kan det være nyttig å hente inspirasjon fra et lite script som gjør nettopp dette:

```Python
tekst = "Heisann!" # Variabel med en streng
omvendt_tekst = tekst[::-1] # Slicing-metode reversering

print(f"Teksten lest opp baklengs blir: {omvendt_tekst}")
```

<p style="font-size:12px; text-align:center">Eksempel 1</p>

### Del 1

1. Kopier koden over og se hva programmet gjør.
2. Gjør endringer i programmet slik at koden blir lagt inn i en funksjon.

### Del 2

Under ser du noen metoder som kan brukes på tekst i Python:

```Python
tekst = "Dette er en tekst!" #Variabel med en streng
print(tekst.upper()) # Metode 1
print(tekst.lower()) # Metode 2
print(tekst.capitalize()) # Metode 3
```

Test de tre ulike metodene og se på hva de gjør. Lag nye variabler som lagrer teksten når man bruker de ulike metodene.

Klarer du å lage programmet fra oppgave 1 slik at de store bokstavene forsvinner og det kun kommer stor bokstav i begynnelsen av ordet/setningen når man kjører programmet?

Eks: "Heisann" blir til "Nnasieh"
