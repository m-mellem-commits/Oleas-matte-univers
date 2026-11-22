# 3. Funksjoner

En **funksjon** er en regel som gir nøyaktig én $y$-verdi for hver $x$-verdi. Vi skriver $f(x)$, som leses «f av x».

## Viktige begreper

| Begrep | Betydning |
|---|---|
| **Definisjonsmengde** $D_f$ | Alle $x$-verdier funksjonen er definert for |
| **Verdimengde** $V_f$ | Alle $y$-verdier funksjonen kan få |
| **Nullpunkt** | Der grafen skjærer $x$-aksen: løs $f(x) = 0$ |
| **Skjæring med $y$-aksen** | Regn ut $f(0)$ |
| **Toppunkt / bunnpunkt** | Høyeste / laveste punkt i et område (ekstremalpunkt) |
| **Asymptote** | En linje grafen nærmer seg, men aldri når |

## Lineære funksjoner

$$f(x) = ax + b$$

- $a$ er **stigningstallet**: hvor mye $y$ øker når $x$ øker med 1.
- $b$ er **konstantleddet**: der grafen skjærer $y$-aksen.

**Stigningstall mellom to punkter:** $a = \dfrac{y_2 - y_1}{x_2 - x_1}$

**Ettpunktsformelen:** Linja gjennom $(x_1, y_1)$ med stigningstall $a$ er $y - y_1 = a(x - x_1)$.

## Andregradsfunksjoner

$$f(x) = ax^2 + bx + c$$

Grafen er en **parabel**.

- $a > 0$: parabelen er et «smil» 🙂 og har et **bunnpunkt**.
- $a < 0$: parabelen er «sur» 🙁 og har et **toppunkt**.
- **Symmetrilinje:** $x = -\dfrac{b}{2a}$. Toppunktet eller bunnpunktet ligger på denne linja.

Tre nyttige skrivemåter:

| Form | Hva du ser direkte |
|---|---|
| $f(x) = ax^2 + bx + c$ | skjæring med $y$-aksen: $(0, c)$ |
| $f(x) = a(x - x_1)(x - x_2)$ | nullpunktene $x_1$ og $x_2$ |
| $f(x) = a(x - p)^2 + q$ | topp- eller bunnpunktet $(p, q)$ |

## Polynomfunksjoner

En polynomfunksjon av grad $n$ ser slik ut: $f(x) = a_n x^n + \dots + a_1 x + a_0$.

- Den har **høyst $n$ nullpunkter**.
- Den har **høyst $n - 1$ topp- og bunnpunkter**.
- Tredjegradsfunksjoner ($n = 3$) går fra $-\infty$ til $\infty$ (hvis $a > 0$) og har ofte et toppunkt og et bunnpunkt.

## Rasjonale funksjoner

En rasjonal funksjon er en brøk av to polynomer, for eksempel $f(x) = \dfrac{2x + 1}{x - 3}$.

- **Vertikal asymptote:** der nevneren er 0 (og telleren ikke er 0). Her: $x = 3$.
- **Horisontal asymptote** for $f(x) = \dfrac{ax + b}{cx + d}$: $y = \dfrac{a}{c}$. Her: $y = 2$.
- **Definisjonsmengde:** alle tall unntatt der nevneren er 0.

## Eksponentialfunksjoner

$$f(x) = a \cdot b^x$$

- $a$ er **startverdien** (verdien når $x = 0$).
- $b$ er **vekstfaktoren**. $b > 1$ betyr vekst, $0 < b < 1$ betyr nedgang.
- **Fra prosent til vekstfaktor:** $b = 1 + \dfrac{p}{100}$. Økning på 4 % gir $b = 1{,}04$. Nedgang på 25 % gir $b = 0{,}75$.

Eksponentiell vekst betyr at noe øker med **samme prosent** hver gang, ikke med samme antall.

## Potensfunksjoner

$$f(x) = a \cdot x^b$$

Her står $x$ i grunntallet (i eksponentialfunksjoner står $x$ i eksponenten). Eksempel: arealet av en sirkel, $A(r) = \pi r^2$.

## Modellering og regresjon

Når du har måledata, kan du finne en funksjon som passer:

1. Legg inn punktene i GeoGebra (regneark eller liste).
2. Se på punktene. Hvilken funksjonstype ligner det på?
3. Bruk regresjon: `RegPoly(liste, grad)`, `RegEksp(liste)` eller `RegPot(liste)`.
4. **Vurder modellen:** Passer den til dataene? Gir den mening for store eller små $x$? Over hvilket tidsrom er den gyldig?

## Nyttige GeoGebra-kommandoer

| Kommando | Gjør |
|---|---|
| `Nullpunkt(f)` | finner nullpunkter |
| `Ekstremalpunkt(f)` | finner topp- og bunnpunkter |
| `Skjæring(f, g)` | finner skjæringspunkter mellom to grafer |
| `Asymptote(f)` | finner asymptoter |
| `f(x) = ... , 0 ≤ x ≤ 10` | tegner grafen bare på et intervall |

## Oppgaver

#### Oppgave 3.1 (lett)
Finn likningen for linja gjennom $(1, 3)$ og $(4, 9)$.

<details markdown="1"><summary>Vis fasit</summary>

$a = \dfrac{9 - 3}{4 - 1} = 2$. Ettpunktsformelen: $y - 3 = 2(x - 1)$, så $y = 2x + 1$.
</details>

#### Oppgave 3.2 (lett)
Gitt $f(x) = x^2 - 4x + 3$. Finn nullpunktene, symmetrilinja, bunnpunktet og skjæringen med $y$-aksen.

<details markdown="1"><summary>Vis fasit</summary>

- Nullpunkter: $(x - 1)(x - 3) = 0$, altså $x = 1$ og $x = 3$
- Symmetrilinje: $x = -\dfrac{-4}{2 \cdot 1} = 2$
- Bunnpunkt: $f(2) = 4 - 8 + 3 = -1$, altså $(2, -1)$
- Skjæring med $y$-aksen: $(0, 3)$
</details>

#### Oppgave 3.3 (middels)
Skriv $f(x) = 2x^2 + 8x + 5$ på formen $a(x - p)^2 + q$, og finn bunnpunktet.

<details markdown="1"><summary>Vis fasit</summary>

$2x^2 + 8x + 5 = 2(x^2 + 4x) + 5 = 2(x^2 + 4x + 4) - 8 + 5 = 2(x + 2)^2 - 3$

Bunnpunkt: $(-2, -3)$.
</details>

#### Oppgave 3.4 (middels)
Gitt $f(x) = \dfrac{2x + 1}{x - 3}$. Finn definisjonsmengden, nullpunktet og asymptotene.

<details markdown="1"><summary>Vis fasit</summary>

- $D_f = \mathbb{R} \setminus \{3\}$ (alle tall unntatt 3)
- Nullpunkt: $2x + 1 = 0$, altså $x = -\dfrac{1}{2}$
- Vertikal asymptote: $x = 3$
- Horisontal asymptote: $y = \dfrac{2}{1} = 2$
</details>

#### Oppgave 3.5 (lett)
Finn vekstfaktoren:
a) økning på 4 %  b) nedgang på 25 %  c) økning på 120 %

<details markdown="1"><summary>Vis fasit</summary>

a) $1{,}04$  b) $0{,}75$  c) $2{,}20$
</details>

#### Oppgave 3.6 (middels)
En bil koster 300 000 kr ny og taper 15 % av verdien hvert år.
a) Lag en funksjon $V(x)$ for verdien etter $x$ år.
b) Hva er bilen verdt etter 4 år?
c) Når er bilen verdt mindre enn 100 000 kr? (Bruk gjerne GeoGebra.)

<details markdown="1"><summary>Vis fasit</summary>

a) $V(x) = 300\,000 \cdot 0{,}85^x$

b) $V(4) = 300\,000 \cdot 0{,}85^4 \approx 156\,602$ kr

c) Løs $300\,000 \cdot 0{,}85^x = 100\,000$. GeoGebra gir $x \approx 6{,}8$. Bilen er altså verdt under 100 000 kr etter ca. 6,8 år, det vil si i løpet av det sjuende året.
</details>

#### Oppgave 3.7 (middels)
Finn nullpunktene til $f(x) = x^3 - 3x$.

<details markdown="1"><summary>Vis fasit</summary>

$x(x^2 - 3) = 0$, så $x = 0$ eller $x^2 = 3$.

Nullpunkter: $x = 0$, $x = \sqrt{3}$ og $x = -\sqrt{3}$.
</details>

#### Oppgave 3.8 (lett)
Arealet av en sirkel er $A(r) = \pi r^2$. Hva skjer med arealet når radien dobles?

<details markdown="1"><summary>Vis fasit</summary>

$A(2r) = \pi (2r)^2 = 4\pi r^2 = 4 \cdot A(r)$. Arealet blir **fire ganger** så stort.
</details>

#### Oppgave 3.9 (utfordring)
Tabellen viser antall følgere på en konto:

| År | 0 | 1 | 2 | 3 |
|---|---|---|---|---|
| Følgere (tusen) | 50 | 60 | 72 | 86,4 |

a) Hvilken funksjonstype passer? Begrunn.
b) Finn en modell.
c) Hvor mange følgere gir modellen etter 10 år? Er det realistisk?

<details markdown="1"><summary>Vis fasit</summary>

a) $60 / 50 = 1{,}2$, $72 / 60 = 1{,}2$ og $86{,}4 / 72 = 1{,}2$. Samme prosentvise økning hvert år, så det er en **eksponentialfunksjon**.

b) $F(x) = 50 \cdot 1{,}2^x$ (tusen følgere). `RegEksp` i GeoGebra gir det samme.

c) $F(10) = 50 \cdot 1{,}2^{10} \approx 309{,}6$, altså ca. 310 000 følgere. Det er usikkert om veksten kan fortsette så lenge. Eksponentiell vekst flater ofte ut i virkeligheten, så modellen er nok mest pålitelig for de nærmeste årene.
</details>
