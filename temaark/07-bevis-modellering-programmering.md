# 7. Bevis, modellering og programmering

Disse temaene går på tvers av hele faget, og de er viktige på muntlig eksamen.

## Bevis

Et **bevis** er en logisk forklaring som viser at noe er sant i *alle* tilfeller, ikke bare i noen eksempler.

### Nyttige skrivemåter

| Hva | Skrives som ($n$ er et helt tall) |
|---|---|
| partall | $2n$ |
| oddetall | $2n + 1$ |
| tre påfølgende tall | $n,\ n + 1,\ n + 2$ |
| delelig med 3 | $3 \cdot (\text{et helt tall})$ |

### Typer bevis

- **Direkte bevis:** Start med det du vet, og regn deg fram til påstanden.
- **Moteksempel:** For å vise at en påstand er *usann*, holder det med **ett** eksempel der den ikke stemmer.
- **Eksempler er ikke bevis:** At noe stemmer for $n = 1, 2, 3$ betyr ikke at det stemmer for alle $n$.

**Eksempel:** Vis at summen av to oddetall alltid er et partall.

$(2m + 1) + (2n + 1) = 2m + 2n + 2 = 2(m + n + 1)$. Dette er 2 ganget med et helt tall, altså et partall. ∎

## Modellering

En **modell** er en funksjon som beskriver noe fra virkeligheten. Slik jobber du:

1. **Forstå situasjonen.** Hva er $x$, hva er $y$, og hvilke enheter har de?
2. **Velg funksjonstype.** Lineær (lik økning), eksponentiell (lik prosentvis økning), andregrads (topp eller bunn) eller annen?
3. **Lag modellen**, for eksempel med regresjon i GeoGebra.
4. **Bruk modellen** til å svare på spørsmål.
5. **Vurder modellen:** Hvor godt passer den? For hvilke verdier er den gyldig? Hva tar den ikke hensyn til?

> 💡 Å vurdere modellen kritisk er det som skiller en god besvarelse fra en veldig god.

## Programmering med Python

I 1T skal du kunne bruke programmering til å løse matematiske problemer. Her er det viktigste:

```python
# Variabler og utskrift
a = 5
print("a er", a)

# Funksjoner
def f(x):
    return x**2 - 4*x + 3      # x**2 betyr x i andre

print(f(2))                    # skriver ut -1

# for-løkke: lag en verditabell
for x in range(0, 5):          # x = 0, 1, 2, 3, 4
    print(x, f(x))

# while-løkke: gjenta så lenge noe er sant
beløp = 10000
år = 0
while beløp < 20000:
    beløp = beløp * 1.03
    år = år + 1
print("Doblet etter", år, "år")

# if-setning
if f(1) == 0:
    print("x = 1 er et nullpunkt")
```

### Halveringsmetoden (finne nullpunkt numerisk)

Hvis $f(a)$ og $f(b)$ har ulikt fortegn, ligger det et nullpunkt mellom $a$ og $b$. Halver intervallet om og om igjen:

```python
def f(x):
    return x**3 - x - 1

a, b = 1, 2
while b - a > 0.0001:
    m = (a + b) / 2
    if f(a) * f(m) < 0:    # ulikt fortegn: nullpunktet er i venstre halvdel
        b = m
    else:
        a = m
print("Nullpunkt ca.", round(m, 4))
```

Du kan kjøre Python gratis i nettleseren, for eksempel på [trinket.io](https://trinket.io/python3) eller i [NDLAs Python-ressurser](https://ndla.no/f/matematikk-1t/be2ae5a11bba).

## Oppgaver

#### Oppgave 7.1 (lett)
Vis at summen av tre påfølgende hele tall alltid er delelig med 3.

<details markdown="1"><summary>Vis fasit</summary>

$n + (n + 1) + (n + 2) = 3n + 3 = 3(n + 1)$. Dette er 3 ganget med et helt tall, altså delelig med 3. ∎
</details>

#### Oppgave 7.2 (middels)
Vis at produktet av to oddetall alltid er et oddetall.

<details markdown="1"><summary>Vis fasit</summary>

$(2m + 1)(2n + 1) = 4mn + 2m + 2n + 1 = 2(2mn + m + n) + 1$

Dette er på formen $2k + 1$, altså et oddetall. ∎
</details>

#### Oppgave 7.3 (middels)
Påstand: «$n^2 + n + 41$ er et primtall for alle naturlige tall $n$.» Stemmer det?

<details markdown="1"><summary>Vis fasit</summary>

Nei. Moteksempel: $n = 40$ gir $1600 + 40 + 41 = 1681 = 41 \cdot 41$, som ikke er et primtall.

(Påstanden stemmer for $n = 0, 1, \dots, 39$. Dette viser hvorfor mange eksempler ikke er et bevis!)
</details>

#### Oppgave 7.4 (utfordring)
Vis at differansen mellom kvadratene av to påfølgende oddetall alltid er delelig med 8.

<details markdown="1"><summary>Vis fasit</summary>

To påfølgende oddetall: $2n + 1$ og $2n + 3$.

$(2n + 3)^2 - (2n + 1)^2 = (4n^2 + 12n + 9) - (4n^2 + 4n + 1) = 8n + 8 = 8(n + 1)$ ∎
</details>

#### Oppgave 7.5 (middels)
Du setter inn 10 000 kr i banken med 3 % rente per år. Skriv et Python-program som finner hvor mange år det tar før beløpet er doblet.

<details markdown="1"><summary>Vis fasit</summary>

Se `while`-løkka i teorien over. Programmet skriver ut **24 år**.

Kontroll: $1{,}03^{23} \approx 1{,}97$ og $1{,}03^{24} \approx 2{,}03$.
</details>

#### Oppgave 7.6 (utfordring)
Bruk halveringsmetoden (programmet over) til å finne nullpunktet til $f(x) = x^3 - x - 1$ mellom 1 og 2. Kontroller svaret i GeoGebra.

<details markdown="1"><summary>Vis fasit</summary>

Nullpunktet er $x \approx 1{,}3247$.
</details>

#### Oppgave 7.7 (utfordring)
En kopp kaffe er 90 °C. Temperaturen synker slik:

| Minutter | 0 | 5 | 10 | 15 |
|---|---|---|---|---|
| °C | 90 | 70 | 56 | 46 |

a) Lag en lineær modell og en eksponentiell modell i GeoGebra.
b) Hvilken passer best? Hva sier modellene om temperaturen etter 2 timer? Er det realistisk hvis romtemperaturen er 20 °C?

<details markdown="1"><summary>Vis fasit</summary>

a) Lineær regresjon gir omtrent $T(t) = -2{,}92t + 87{,}4$. Eksponentiell regresjon gir omtrent $T(t) = 88{,}8 \cdot 0{,}956^t$. (Små avvik avhengig av avrunding er helt greit.)

b) Den eksponentielle passer best, fordi temperaturen synker mindre og mindre for hvert minutt. Etter 120 minutter gir den lineære modellen en negativ temperatur (ca. −260 °C), som er umulig. Den eksponentielle gir under 1 °C, som også er feil, fordi kaffen aldri blir kaldere enn rommet (20 °C). Ingen av modellene er gyldige over lang tid. En bedre modell ville vært $T(t) = 20 + 70 \cdot b^t$, som nærmer seg romtemperaturen.
</details>
