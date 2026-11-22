# 4. Polynomdivisjon

Polynomdivisjon er vanlig divisjon (som $847 : 7$), bare med bokstaver. Den brukes til å **faktorisere** polynomer og **løse likninger** av høyere grad.

## Nullpunktsetningen (faktorteoremet)

> Hvis $P(a) = 0$, så går divisjonen $P(x) : (x - a)$ opp, og $(x - a)$ er en faktor i $P(x)$.

Det motsatte gjelder også: Hvis $(x - a)$ er en faktor, så er $P(a) = 0$.

**Restsetningen:** Når du deler $P(x)$ på $(x - a)$, blir resten lik $P(a)$.

## Slik gjør du polynomdivisjon

**Eksempel:** $(x^3 - 2x^2 - 5x + 6) : (x - 1)$

Sjekk først: $P(1) = 1 - 2 - 5 + 6 = 0$. Divisjonen går altså opp.

Gjenta disse fire stegene til du er ferdig:

1. **Del** første ledd i det som er igjen på $x$: $x^3 : x = x^2$
2. **Gang** svaret med hele divisoren: $x^2(x - 1) = x^3 - x^2$
3. **Trekk fra:** $(x^3 - 2x^2) - (x^3 - x^2) = -x^2$
4. **Flytt ned** neste ledd: $-x^2 - 5x$

```
  (x³ − 2x² − 5x + 6) : (x − 1) = x² − x − 6
 −(x³ −  x²)
  ─────────
       −x² − 5x
      −(−x² +  x)
       ─────────
             −6x + 6
            −(−6x + 6)
             ─────────
                     0
```

Altså er $x^3 - 2x^2 - 5x + 6 = (x - 1)(x^2 - x - 6) = (x - 1)(x - 3)(x + 2)$.

## Strategi for å løse tredjegradslikninger

1. **Gjett en løsning.** Prøv tall som går opp i konstantleddet: $\pm 1, \pm 2, \pm 3, \dots$
2. **Polynomdivisjon** med $(x - \text{løsningen})$. Da får du et andregradsuttrykk.
3. **Løs andregradslikningen** med abc-formelen eller faktorisering.

## Divisjon med rest

Når divisjonen ikke går opp, skriver vi

$$P(x) = (x - a) \cdot Q(x) + R \qquad\text{eller}\qquad \frac{P(x)}{x - a} = Q(x) + \frac{R}{x - a}$$

Dette er nyttig for rasjonale funksjoner. Hvis telleren har høyere grad enn nevneren, får grafen en **skrå asymptote** $y = Q(x)$.

## Oppgaver

#### Oppgave 4.1 (lett)
Utfør divisjonen $(x^2 + 5x + 6) : (x + 2)$.

<details markdown="1"><summary>Vis fasit</summary>

$x + 3$. (Kontroll: $(x + 2)(x + 3) = x^2 + 5x + 6$ ✓)
</details>

#### Oppgave 4.2 (middels)
Utfør divisjonen $(x^3 - 8) : (x - 2)$.

<details markdown="1"><summary>Vis fasit</summary>

Tips: Skriv $x^3 + 0x^2 + 0x - 8$, så du har plass til alle ledd.

Svar: $x^2 + 2x + 4$
</details>

#### Oppgave 4.3 (middels)
Utfør divisjonen $(2x^3 + 3x^2 - x + 5) : (x + 1)$. Hva blir resten? Kontroller resten med restsetningen.

<details markdown="1"><summary>Vis fasit</summary>

$(2x^3 + 3x^2 - x + 5) = (x + 1)(2x^2 + x - 2) + 7$

Resten er 7. Kontroll: $P(-1) = -2 + 3 + 1 + 5 = 7$ ✓
</details>

#### Oppgave 4.4 (middels)
Løs likningen $x^3 - 6x^2 + 11x - 6 = 0$.

<details markdown="1"><summary>Vis fasit</summary>

Prøv $x = 1$: $1 - 6 + 11 - 6 = 0$ ✓

$(x^3 - 6x^2 + 11x - 6) : (x - 1) = x^2 - 5x + 6 = (x - 2)(x - 3)$

Løsninger: $x = 1$, $x = 2$ og $x = 3$.
</details>

#### Oppgave 4.5 (middels)
Faktoriser $P(x) = x^3 + x^2 - 4x - 4$.

<details markdown="1"><summary>Vis fasit</summary>

Enten med polynomdivisjon ($P(-1) = 0$), eller ved å gruppere:

$x^2(x + 1) - 4(x + 1) = (x + 1)(x^2 - 4) = (x + 1)(x - 2)(x + 2)$
</details>

#### Oppgave 4.6 (utfordring)
Løs ulikheten $x^3 - 6x^2 + 11x - 6 > 0$.

<details markdown="1"><summary>Vis fasit</summary>

Fra oppgave 4.4: $(x - 1)(x - 2)(x - 3) > 0$.

| | $x < 1$ | $1 < x < 2$ | $2 < x < 3$ | $x > 3$ |
|---|---|---|---|---|
| $x - 1$ | − | + | + | + |
| $x - 2$ | − | − | + | + |
| $x - 3$ | − | − | − | + |
| Produkt | − | + | − | + |

Svar: $1 < x < 2$ eller $x > 3$.
</details>

#### Oppgave 4.7 (middels)
Bestem $k$ slik at $(x - 2)$ er en faktor i $P(x) = x^3 + kx - 4$.

<details markdown="1"><summary>Vis fasit</summary>

Krav: $P(2) = 0$. $8 + 2k - 4 = 0 \Rightarrow k = -2$.
</details>

#### Oppgave 4.8 (utfordring)
Skriv $f(x) = \dfrac{x^2 + 1}{x - 1}$ på formen $Q(x) + \dfrac{R}{x - 1}$. Hva blir den skrå asymptoten?

<details markdown="1"><summary>Vis fasit</summary>

$(x^2 + 1) : (x - 1) = x + 1$ med rest $2$. Altså er $f(x) = x + 1 + \dfrac{2}{x - 1}$.

Når $x$ blir veldig stor, går $\dfrac{2}{x - 1}$ mot 0, så den skrå asymptoten er $y = x + 1$. Den vertikale asymptoten er $x = 1$.
</details>
