# 1. Tall og algebra

Algebra er å regne med bokstaver. Alt du lærer senere i 1T bygger på dette, så det lønner seg å bli trygg her.

## Potensregler

En potens $a^n$ betyr at $a$ ganges med seg selv $n$ ganger. $a$ kalles **grunntallet** og $n$ **eksponenten**.

| Regel | Eksempel |
|---|---|
| $a^m \cdot a^n = a^{m+n}$ | $x^3 \cdot x^4 = x^7$ |
| $\dfrac{a^m}{a^n} = a^{m-n}$ | $\dfrac{x^5}{x^2} = x^3$ |
| $(a^m)^n = a^{m \cdot n}$ | $(x^2)^3 = x^6$ |
| $(a \cdot b)^n = a^n \cdot b^n$ | $(2x)^3 = 8x^3$ |
| $\left(\dfrac{a}{b}\right)^n = \dfrac{a^n}{b^n}$ | $\left(\dfrac{x}{3}\right)^2 = \dfrac{x^2}{9}$ |
| $a^0 = 1$ | $5^0 = 1$ |
| $a^{-n} = \dfrac{1}{a^n}$ | $2^{-3} = \dfrac{1}{8}$ |
| $a^{\frac{1}{n}} = \sqrt[n]{a}$ | $9^{\frac{1}{2}} = \sqrt{9} = 3$ |
| $a^{\frac{m}{n}} = \left(\sqrt[n]{a}\right)^m$ | $8^{\frac{2}{3}} = 2^2 = 4$ |

> ⚠️ **Vanlig feil:** $(a+b)^2$ er **ikke** $a^2 + b^2$. Potensregelen $(ab)^n = a^n b^n$ gjelder bare for *gange*, ikke for pluss.

**Triks:** Når tallene er forskjellige, prøv å skrive dem med samme grunntall. For eksempel er $9 = 3^2$ og $27 = 3^3$.

## Standardform

Store og små tall skrives på **standardform**: $a \cdot 10^k$, der $1 \le a < 10$ og $k$ er et helt tall.

- $340\,000 = 3{,}4 \cdot 10^5$ (kommaet flyttes 5 plasser til venstre)
- $0{,}0072 = 7{,}2 \cdot 10^{-3}$ (kommaet flyttes 3 plasser til høyre)

## Kvadratsetningene

$$(a+b)^2 = a^2 + 2ab + b^2 \qquad \text{(1. kvadratsetning)}$$

$$(a-b)^2 = a^2 - 2ab + b^2 \qquad \text{(2. kvadratsetning)}$$

$$(a+b)(a-b) = a^2 - b^2 \qquad \text{(konjugatsetningen)}$$

Kvadratsetningene brukes begge veier: til å **gange ut** og til å **faktorisere**.

## Faktorisering

Å faktorisere betyr å skrive et uttrykk som et produkt (noe ganget med noe). Prøv i denne rekkefølgen:

1. **Felles faktor:** $6x^2 + 9x = 3x(2x + 3)$
2. **Kvadratsetning baklengs:** $x^2 - 10x + 25 = (x-5)^2$ og $x^2 - 16 = (x+4)(x-4)$
3. **Andregradsuttrykk med nullpunkter:** Hvis $ax^2 + bx + c = 0$ har løsningene $x_1$ og $x_2$, så er

$$ax^2 + bx + c = a(x - x_1)(x - x_2)$$

## Rasjonale uttrykk (brøker med bokstaver)

- **Forkorting:** Du kan bare forkorte **faktorer**, aldri ledd. Faktoriser teller og nevner først.

$$\frac{x^2 - 9}{2x + 6} = \frac{(x+3)(x-3)}{2(x+3)} = \frac{x-3}{2}$$

- **Pluss og minus:** Finn fellesnevner, akkurat som med vanlige brøker.

> ⚠️ **Vanlig feil:** $\dfrac{x + 3}{3} \ne x$. Her er $3$ et *ledd* i telleren, ikke en faktor.

## Identitet, likning, uttrykk og funksjon

Dette er et eget kompetansemål, og det er populært på muntlig eksamen!

| Begrep | Hva er det? | Eksempel |
|---|---|---|
| **Uttrykk** | En «regnestykke-bit» uten likhetstegn | $2x + 3$ |
| **Likning** | To uttrykk med likhetstegn som er sanne for *noen* verdier av $x$ | $2x + 3 = 7$ (sann bare for $x = 2$) |
| **Identitet** | En likhet som er sann for *alle* verdier av $x$ | $(x+1)^2 = x^2 + 2x + 1$ |
| **Funksjon** | En regel som gir nøyaktig én $y$-verdi for hver $x$-verdi | $f(x) = 2x + 3$ |

## Eksempler

**Eksempel 1:** Forenkle $\dfrac{2^5 \cdot 4^{-1}}{8}$.

Skriv alt med grunntall 2: $\dfrac{2^5 \cdot (2^2)^{-1}}{2^3} = \dfrac{2^5 \cdot 2^{-2}}{2^3} = 2^{5 - 2 - 3} = 2^0 = 1$

**Eksempel 2:** Faktoriser $x^2 + 2x - 8$.

Løs $x^2 + 2x - 8 = 0$. To tall som ganget blir $-8$ og summert blir $2$: $4$ og $-2$. Altså er $x^2 + 2x - 8 = (x + 4)(x - 2)$.

**Eksempel 3:** Trekk sammen $\dfrac{2}{x} + \dfrac{3}{x+1}$.

Fellesnevner er $x(x+1)$:

$$\frac{2(x+1)}{x(x+1)} + \frac{3x}{x(x+1)} = \frac{2x + 2 + 3x}{x(x+1)} = \frac{5x + 2}{x(x+1)}$$

## Oppgaver

#### Oppgave 1.1 (lett)
Forenkle $\dfrac{a^3 \cdot a^{-1}}{a^4}$.

<details markdown="1"><summary>Vis fasit</summary>

$a^{3 + (-1) - 4} = a^{-2} = \dfrac{1}{a^2}$
</details>

#### Oppgave 1.2 (lett)
Regn ut $(2x^2y)^3$.

<details markdown="1"><summary>Vis fasit</summary>

$2^3 \cdot (x^2)^3 \cdot y^3 = 8x^6y^3$
</details>

#### Oppgave 1.3 (lett)
a) Skriv $0{,}000045$ på standardform.
b) Regn ut $(3 \cdot 10^5) \cdot (4 \cdot 10^{-2})$ og skriv svaret på standardform.

<details markdown="1"><summary>Vis fasit</summary>

a) $4{,}5 \cdot 10^{-5}$

b) $3 \cdot 4 \cdot 10^{5 + (-2)} = 12 \cdot 10^3 = 1{,}2 \cdot 10^4$
</details>

#### Oppgave 1.4 (middels)
Forenkle $\dfrac{3^4 \cdot 9^{-1}}{27}$.

<details markdown="1"><summary>Vis fasit</summary>

Skriv med grunntall 3: $\dfrac{3^4 \cdot 3^{-2}}{3^3} = 3^{4 - 2 - 3} = 3^{-1} = \dfrac{1}{3}$
</details>

#### Oppgave 1.5 (lett)
Gang ut parentesen: $(2x - 3)^2$.

<details markdown="1"><summary>Vis fasit</summary>

Andre kvadratsetning: $(2x)^2 - 2 \cdot 2x \cdot 3 + 3^2 = 4x^2 - 12x + 9$
</details>

#### Oppgave 1.6 (middels)
Faktoriser uttrykkene:
a) $4x^2 - 25$  b) $x^2 + 6x + 9$  c) $x^2 - x - 6$

<details markdown="1"><summary>Vis fasit</summary>

a) Konjugatsetningen: $(2x + 5)(2x - 5)$

b) Første kvadratsetning: $(x + 3)^2$

c) Nullpunktene er $x = 3$ og $x = -2$, så $(x - 3)(x + 2)$
</details>

#### Oppgave 1.7 (middels)
Forkort $\dfrac{x^2 - 4}{x^2 + 4x + 4}$.

<details markdown="1"><summary>Vis fasit</summary>

$\dfrac{(x+2)(x-2)}{(x+2)^2} = \dfrac{x - 2}{x + 2}$
</details>

#### Oppgave 1.8 (middels)
Regn ut $8^{\frac{2}{3}}$ og skriv $\sqrt[3]{x} \cdot \sqrt{x}$ som én potens.

<details markdown="1"><summary>Vis fasit</summary>

$8^{\frac{2}{3}} = \left(\sqrt[3]{8}\right)^2 = 2^2 = 4$

$x^{\frac{1}{3}} \cdot x^{\frac{1}{2}} = x^{\frac{1}{3} + \frac{1}{2}} = x^{\frac{5}{6}}$
</details>

#### Oppgave 1.9 (utfordring)
Trekk sammen og forkort $\dfrac{1}{x - 1} - \dfrac{2}{x^2 - 1}$.

<details markdown="1"><summary>Vis fasit</summary>

Siden $x^2 - 1 = (x+1)(x-1)$, er fellesnevner $(x+1)(x-1)$:

$$\frac{x + 1}{(x+1)(x-1)} - \frac{2}{(x+1)(x-1)} = \frac{x - 1}{(x+1)(x-1)} = \frac{1}{x + 1}$$

</details>

#### Oppgave 1.10 (utfordring)
a) Er $(x + 1)^2 = x^2 + 1$ en identitet? Begrunn svaret.
b) Vis at $(n+1)^2 - n^2$ alltid er et oddetall når $n$ er et helt tall.

<details markdown="1"><summary>Vis fasit</summary>

a) Nei. Prøv $x = 1$: venstre side blir $4$, høyre side blir $2$. Ett moteksempel holder for å vise at det ikke er en identitet. (Det er en *likning*, som bare er sann for $x = 0$.)

b) $(n+1)^2 - n^2 = n^2 + 2n + 1 - n^2 = 2n + 1$. Et tall på formen $2n + 1$ er alltid et oddetall.
</details>
