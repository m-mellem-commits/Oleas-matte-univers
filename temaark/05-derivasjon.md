# 5. Vekstfart og derivasjon

Den deriverte forteller **hvor fort noe endrer seg** akkurat nå. Det er som speedometeret i en bil.

## Gjennomsnittlig vekstfart

Hvor mye endrer funksjonen seg i gjennomsnitt per enhet fra $x = a$ til $x = b$?

$$\text{gjennomsnittlig vekstfart} = \frac{f(b) - f(a)}{b - a}$$

Geometrisk er dette **stigningstallet til linja (sekanten)** gjennom punktene $(a, f(a))$ og $(b, f(b))$.

## Momentan vekstfart og den deriverte

La de to punktene komme nærmere og nærmere hverandre. Da blir sekanten til en **tangent**. Stigningstallet til tangenten i $x = a$ kaller vi den **deriverte**, $f'(a)$.

**Definisjonen av den deriverte:**

$$f'(x) = \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}$$

**Eksempel:** For $f(x) = x^2$:

$$\frac{(x + h)^2 - x^2}{h} = \frac{x^2 + 2xh + h^2 - x^2}{h} = \frac{2xh + h^2}{h} = 2x + h \;\xrightarrow{h \to 0}\; 2x$$

Altså er $f'(x) = 2x$.

## Derivasjonsregler

| Funksjon | Derivert |
|---|---|
| $c$ (konstant) | $0$ |
| $x$ | $1$ |
| $x^n$ | $n \cdot x^{n-1}$ |
| $c \cdot f(x)$ | $c \cdot f'(x)$ |
| $f(x) + g(x)$ | $f'(x) + g'(x)$ |

**Eksempel:** $f(x) = 4x^3 - 5x^2 + 2x - 7$ gir $f'(x) = 12x^2 - 10x + 2$.

## Tangentlikning

Tangenten til $f$ i punktet $x = a$:

$$y - f(a) = f'(a)(x - a)$$

**Oppskrift:** (1) Regn ut $f(a)$. (2) Finn $f'(x)$ og regn ut $f'(a)$. (3) Sett inn i formelen.

## Drøfting: hvor stiger og synker grafen?

| Fortegn til $f'(x)$ | Grafen … |
|---|---|
| $f'(x) > 0$ | stiger |
| $f'(x) < 0$ | synker |
| $f'(x) = 0$ | har horisontal tangent (mulig topp- eller bunnpunkt) |

**Oppskrift for topp- og bunnpunkter:**
1. Finn $f'(x)$.
2. Løs $f'(x) = 0$.
3. Lag fortegnslinje for $f'(x)$.
4. Fra + til − gir **toppunkt**. Fra − til + gir **bunnpunkt**.
5. Regn ut $y$-verdien ved å sette inn i $f(x)$ (ikke i $f'(x)$!).

## Tolkning med enheter

Hvis $h(t)$ er høyden i meter etter $t$ sekunder, er $h'(t)$ farten i **meter per sekund**. Enheten til den deriverte er alltid

$$\frac{\text{enheten til } y}{\text{enheten til } x}$$

> 💡 **På muntlig eksamen:** Kunne forklare med egne ord: «Den deriverte er stigningstallet til tangenten, og den forteller hvor raskt funksjonen endrer seg i et bestemt punkt.»

## Oppgaver

#### Oppgave 5.1 (lett)
Finn den gjennomsnittlige vekstfarten til $f(x) = x^2$ fra $x = 1$ til $x = 3$.

<details markdown="1"><summary>Vis fasit</summary>

$\dfrac{f(3) - f(1)}{3 - 1} = \dfrac{9 - 1}{2} = 4$
</details>

#### Oppgave 5.2 (lett)
Deriver $f(x) = 3x^4 - 2x^2 + 5x - 7$.

<details markdown="1"><summary>Vis fasit</summary>

$f'(x) = 12x^3 - 4x + 5$
</details>

#### Oppgave 5.3 (lett)
Deriver $g(x) = \dfrac{1}{3}x^3 - 4x$.

<details markdown="1"><summary>Vis fasit</summary>

$g'(x) = \dfrac{1}{3} \cdot 3x^2 - 4 = x^2 - 4$
</details>

#### Oppgave 5.4 (middels)
Finn likningen for tangenten til $f(x) = x^2 - 3x$ i punktet der $x = 1$.

<details markdown="1"><summary>Vis fasit</summary>

$f(1) = 1 - 3 = -2$. $f'(x) = 2x - 3$, så $f'(1) = -1$.

$y - (-2) = -1(x - 1) \Rightarrow y = -x - 1$
</details>

#### Oppgave 5.5 (middels)
Finn punktet på grafen til $f(x) = x^2 - 4x + 1$ der tangenten er horisontal.

<details markdown="1"><summary>Vis fasit</summary>

$f'(x) = 2x - 4 = 0 \Rightarrow x = 2$. $f(2) = 4 - 8 + 1 = -3$. Punktet er $(2, -3)$.
</details>

#### Oppgave 5.6 (middels)
Gitt $f(x) = x^3 - 3x^2$. Finn hvor grafen stiger og synker, og finn topp- og bunnpunktene.

<details markdown="1"><summary>Vis fasit</summary>

$f'(x) = 3x^2 - 6x = 3x(x - 2)$. Nullpunkter: $x = 0$ og $x = 2$.

| | $x < 0$ | $0 < x < 2$ | $x > 2$ |
|---|---|---|---|
| $3x$ | − | + | + |
| $x - 2$ | − | − | + |
| $f'(x)$ | + | − | + |

Grafen stiger for $x < 0$ og $x > 2$, og synker for $0 < x < 2$.

Toppunkt: $(0, f(0)) = (0, 0)$. Bunnpunkt: $(2, f(2)) = (2, 8 - 12) = (2, -4)$.
</details>

#### Oppgave 5.7 (middels)
Temperaturen en dag er gitt ved $T(t) = -0{,}5t^2 + 4t + 10$, der $T$ er i °C og $t$ er timer etter kl. 08.
a) Finn $T'(2)$ og forklar hva tallet betyr.
b) Når er det varmest, og hvor varmt er det da?

<details markdown="1"><summary>Vis fasit</summary>

a) $T'(t) = -t + 4$, så $T'(2) = 2$. Klokka 10 stiger temperaturen med 2 °C per time.

b) $T'(t) = 0$ gir $t = 4$, altså kl. 12. $T(4) = -8 + 16 + 10 = 18$ °C.
</details>

#### Oppgave 5.8 (utfordring)
Bruk definisjonen av den deriverte til å vise at $f(x) = 3x^2$ har $f'(x) = 6x$.

<details markdown="1"><summary>Vis fasit</summary>

$$\frac{3(x + h)^2 - 3x^2}{h} = \frac{3x^2 + 6xh + 3h^2 - 3x^2}{h} = \frac{6xh + 3h^2}{h} = 6x + 3h$$

Når $h \to 0$, går dette mot $6x$. Altså er $f'(x) = 6x$.
</details>

#### Oppgave 5.9 (utfordring)
Du har 40 meter gjerde og skal lage en rektangulær innhegning inntil en vegg (veggen trenger ikke gjerde). Hvor stort kan arealet bli?

<details markdown="1"><summary>Vis fasit</summary>

La $x$ være lengden på de to sidene som står ut fra veggen. Siden parallelt med veggen blir $40 - 2x$.

$A(x) = x(40 - 2x) = 40x - 2x^2$, der $0 < x < 20$.

$A'(x) = 40 - 4x = 0 \Rightarrow x = 10$. Fortegnet til $A'$ går fra + til −, så dette er et toppunkt.

$A(10) = 10 \cdot 20 = 200$. Største areal er **200 m²** (10 m × 20 m).
</details>
