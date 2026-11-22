# 2. Likninger, likningssett og ulikheter

Å løse en likning betyr å finne de verdiene av $x$ som gjør at venstre og høyre side blir like.

## Gylne regel

Du kan gjøre (nesten) hva du vil med en likning, **så lenge du gjør det samme på begge sider**: legge til, trekke fra, gange eller dele (men aldri dele på 0).

## Førstegradslikninger

Samle $x$-ledd på én side og tall på den andre.

$$3x + 5 = x - 7 \;\Rightarrow\; 2x = -12 \;\Rightarrow\; x = -6$$

**Med brøker:** Gang alle ledd med fellesnevneren først, så forsvinner brøkene.

## Andregradslikninger

En andregradslikning kan skrives som $ax^2 + bx + c = 0$, der $a \ne 0$.

### abc-formelen

$$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

Uttrykket under rottegnet, $D = b^2 - 4ac$, kalles **diskriminanten**:

| Diskriminant | Antall løsninger |
|---|---|
| $D > 0$ | to løsninger |
| $D = 0$ | én løsning |
| $D < 0$ | ingen løsning |

### Snarveier (ofte raskere enn abc-formelen)

- **Mangler konstantledd** ($c = 0$): Sett $x$ utenfor. $x^2 - 5x = 0 \Rightarrow x(x - 5) = 0 \Rightarrow x = 0$ eller $x = 5$.
- **Mangler $x$-ledd** ($b = 0$): $x^2 = 9 \Rightarrow x = \pm 3$.
- **Produktregelen:** Hvis $A \cdot B = 0$, så er $A = 0$ eller $B = 0$.

> ⚠️ **Vanlig feil:** Del aldri på $x$ for å «forenkle» $x^2 = 5x$. Da mister du løsningen $x = 0$.

### Fullstendige kvadraters metode

Denne metoden viser *hvorfor* abc-formelen virker, og knytter andregradslikninger til kvadratsetningene. Legg til det som mangler for å få et fullstendig kvadrat:

$$x^2 + 6x + 5 = 0 \;\Rightarrow\; x^2 + 6x + 9 = 4 \;\Rightarrow\; (x + 3)^2 = 4 \;\Rightarrow\; x + 3 = \pm 2$$

Altså er $x = -1$ eller $x = -5$. Tallet du legger til, er alltid $\left(\frac{b}{2}\right)^2$.

## Rasjonale likninger (x i nevneren)

1. Finn verdiene som gjør nevneren lik 0. Disse er **ikke lov**.
2. Gang med fellesnevner og løs.
3. **Sjekk** at svaret ikke er en av de forbudte verdiene.

## Likningssett

To likninger med to ukjente. Tre metoder:

- **Innsettingsmetoden:** Løs den ene likningen for $y$ (eller $x$), og sett inn i den andre.
- **Addisjonsmetoden:** Legg sammen likningene slik at én ukjent forsvinner.
- **Grafisk:** Tegn begge grafene. Skjæringspunktene er løsningene. (I GeoGebra: `Skjæring(f, g)`.)

## Ulikheter

Ulikheter løses nesten som likninger, med **ett viktig unntak**:

> ⚠️ Når du ganger eller deler med et **negativt** tall, må du **snu ulikhetstegnet**.
> $-2x > 6 \;\Rightarrow\; x < -3$

### Andregradsulikheter og fortegnslinjer

1. Flytt alt over på én side, slik at det står 0 på den andre.
2. Faktoriser.
3. Lag en **fortegnslinje** for hver faktor, og en for produktet.
4. Les av hvor produktet er positivt eller negativt.

**Eksempel:** $x^2 - x - 6 \le 0$, altså $(x - 3)(x + 2) \le 0$.

| | $x < -2$ | $-2 < x < 3$ | $x > 3$ |
|---|---|---|---|
| $x + 2$ | − | + | + |
| $x - 3$ | − | − | + |
| Produkt | **+** | **−** | **+** |

Produktet er negativt eller null for $-2 \le x \le 3$.

> ⚠️ For **rasjonale ulikheter** (x i nevneren) skal du aldri gange med nevneren, fordi du ikke vet om den er positiv eller negativ. Bruk fortegnslinje i stedet.

## Eksponentiallikninger

Likninger som $1{,}05^x = 2$ løser du i 1T digitalt, for eksempel med CAS i GeoGebra: `Løs(1.05^x = 2)` gir $x \approx 14{,}2$.

## Oppgaver

#### Oppgave 2.1 (lett)
Løs likningen $3(x - 2) = 2x + 5$.

<details markdown="1"><summary>Vis fasit</summary>

$3x - 6 = 2x + 5 \Rightarrow x = 11$
</details>

#### Oppgave 2.2 (middels)
Løs likningen $\dfrac{x}{2} - \dfrac{x - 1}{3} = 2$.

<details markdown="1"><summary>Vis fasit</summary>

Gang alle ledd med 6: $3x - 2(x - 1) = 12 \Rightarrow 3x - 2x + 2 = 12 \Rightarrow x = 10$

Pass på minustegnet foran brøken: $-2(x - 1) = -2x + 2$.
</details>

#### Oppgave 2.3 (lett)
Løs $x^2 - 5x + 6 = 0$.

<details markdown="1"><summary>Vis fasit</summary>

$(x - 2)(x - 3) = 0$, altså $x = 2$ eller $x = 3$.
</details>

#### Oppgave 2.4 (middels)
Løs $2x^2 + 3x - 2 = 0$ med abc-formelen.

<details markdown="1"><summary>Vis fasit</summary>

$a = 2,\ b = 3,\ c = -2$. $D = 3^2 - 4 \cdot 2 \cdot (-2) = 9 + 16 = 25$.

$$x = \frac{-3 \pm 5}{4} \quad\Rightarrow\quad x = \frac{1}{2} \text{ eller } x = -2$$

</details>

#### Oppgave 2.5 (lett)
Hvor mange løsninger har $x^2 + 4x + 5 = 0$?

<details markdown="1"><summary>Vis fasit</summary>

$D = 16 - 20 = -4 < 0$, så likningen har **ingen** løsning.
</details>

#### Oppgave 2.6 (lett)
Løs $3x^2 = 12x$.

<details markdown="1"><summary>Vis fasit</summary>

$3x^2 - 12x = 0 \Rightarrow 3x(x - 4) = 0 \Rightarrow x = 0$ eller $x = 4$.
</details>

#### Oppgave 2.7 (middels)
Løs $x^2 + 6x + 5 = 0$ ved å bruke fullstendige kvadraters metode.

<details markdown="1"><summary>Vis fasit</summary>

$x^2 + 6x = -5$. Legg til $\left(\frac{6}{2}\right)^2 = 9$ på begge sider: $(x + 3)^2 = 4$, så $x + 3 = \pm 2$.

$x = -1$ eller $x = -5$.
</details>

#### Oppgave 2.8 (lett)
Løs likningssettet

$$\begin{cases} 2x + y = 7 \\ x - y = 2 \end{cases}$$

<details markdown="1"><summary>Vis fasit</summary>

Addisjonsmetoden: Legg sammen likningene og få $3x = 9$, så $x = 3$. Sett inn: $3 - y = 2$, så $y = 1$.
</details>

#### Oppgave 2.9 (middels)
Løs likningssettet

$$\begin{cases} y = x^2 - 1 \\ y = x + 1 \end{cases}$$

<details markdown="1"><summary>Vis fasit</summary>

$x^2 - 1 = x + 1 \Rightarrow x^2 - x - 2 = 0 \Rightarrow (x - 2)(x + 1) = 0$.

$x = 2,\ y = 3$ eller $x = -1,\ y = 0$. Grafisk er dette de to punktene der linja skjærer parabelen.
</details>

#### Oppgave 2.10 (lett)
Løs ulikheten $5 - 2x > 1$.

<details markdown="1"><summary>Vis fasit</summary>

$-2x > -4$. Del på $-2$ og snu tegnet: $x < 2$.
</details>

#### Oppgave 2.11 (middels)
Løs ulikheten $x^2 - x - 6 \le 0$.

<details markdown="1"><summary>Vis fasit</summary>

$(x - 3)(x + 2) \le 0$. Fortegnslinjen (se teorien over) gir $-2 \le x \le 3$.
</details>

#### Oppgave 2.12 (utfordring)
Løs ulikheten $\dfrac{x - 1}{x + 2} \ge 0$.

<details markdown="1"><summary>Vis fasit</summary>

Teller er 0 for $x = 1$, nevner er 0 for $x = -2$ (ikke lov).

| | $x < -2$ | $-2 < x < 1$ | $x > 1$ |
|---|---|---|---|
| $x - 1$ | − | − | + |
| $x + 2$ | − | + | + |
| Brøk | + | − | + |

Svar: $x < -2$ eller $x \ge 1$. ($x = -2$ er ikke med, fordi nevneren da er 0.)
</details>

#### Oppgave 2.13 (utfordring)
Løs likningen $\dfrac{x}{x - 2} = \dfrac{2}{x - 2} + 3$.

<details markdown="1"><summary>Vis fasit</summary>

$x = 2$ er ikke lov. Gang med $(x - 2)$: $x = 2 + 3(x - 2) \Rightarrow x = 3x - 4 \Rightarrow x = 2$.

Men $x = 2$ er forbudt! Likningen har derfor **ingen løsning**. Dette er grunnen til at du alltid må sjekke svaret.
</details>
