# 6. Trigonometri

Trigonometri handler om sammenhengen mellom **vinkler** og **sider** i trekanter.

> ⚠️ **Sjekk alltid at kalkulatoren står i grader (DEG)**, ikke radianer (RAD). Det er den vanligste feilen i trigonometri.

## Navn i trekanten

Vi kaller hjørnene $A$, $B$ og $C$. Siden **rett overfor** hjørnet $A$ heter $a$, siden overfor $B$ heter $b$, og siden overfor $C$ heter $c$.

## Rettvinklede trekanter

Sett fra vinkelen $v$:

$$\sin v = \frac{\text{motstående katet}}{\text{hypotenus}}$$

$$\cos v = \frac{\text{hosliggende katet}}{\text{hypotenus}}$$

$$\tan v = \frac{\text{motstående katet}}{\text{hosliggende katet}}$$

**Huskeregel:** *Mo-Hy, Ho-Hy, Mo-Ho* (sinus, cosinus, tangens).

**Pytagoras:** $a^2 + b^2 = c^2$, der $c$ er hypotenusen.

**Finne en vinkel:** Bruk den omvendte funksjonen. Hvis $\sin v = 0{,}5$, så er $v = \sin^{-1}(0{,}5) = 30°$.

## Eksakte verdier

| $v$ | $0°$ | $30°$ | $45°$ | $60°$ | $90°$ |
|---|---|---|---|---|---|
| $\sin v$ | $0$ | $\frac{1}{2}$ | $\frac{\sqrt{2}}{2}$ | $\frac{\sqrt{3}}{2}$ | $1$ |
| $\cos v$ | $1$ | $\frac{\sqrt{3}}{2}$ | $\frac{\sqrt{2}}{2}$ | $\frac{1}{2}$ | $0$ |
| $\tan v$ | $0$ | $\frac{\sqrt{3}}{3}$ | $1$ | $\sqrt{3}$ | — |

Disse kommer fra to «halve» trekanter: et halvt kvadrat (45°-45°-90°) og en halv likesidet trekant (30°-60°-90°).

## Enhetssirkelen (vinkler over 90°)

Tegn en sirkel med radius 1 og sentrum i origo. Et punkt på sirkelen som danner vinkelen $v$ med den positive $x$-aksen, har koordinatene

$$(\cos v,\ \sin v)$$

Slik definerer vi sinus og cosinus også for stumpe vinkler. To viktige regler:

$$\sin(180° - v) = \sin v \qquad\qquad \cos(180° - v) = -\cos v$$

> ⚠️ Likningen $\sin v = k$ (med $0 < k < 1$) har **to** løsninger mellom $0°$ og $180°$: $v$ og $180° - v$. Kalkulatoren viser bare den spisse.

## Arealsetningen

$$A = \frac{1}{2} \cdot a \cdot b \cdot \sin C$$

To sider og **vinkelen mellom dem**.

## Sinussetningen

$$\frac{a}{\sin A} = \frac{b}{\sin B} = \frac{c}{\sin C}$$

Brukes når du kjenner en side og vinkelen **rett overfor**, pluss én side eller vinkel til.

## Cosinussetningen

$$a^2 = b^2 + c^2 - 2bc \cdot \cos A$$

Brukes når du kjenner **tre sider**, eller **to sider og vinkelen mellom dem**.

## Hvilken setning skal jeg bruke?

| Du kjenner … | Bruk |
|---|---|
| tre sider | cosinussetningen |
| to sider og vinkelen mellom dem | cosinussetningen (eller arealsetningen for areal) |
| to vinkler og en side | sinussetningen (finn først den tredje vinkelen: summen er 180°) |
| to sider og en vinkel som *ikke* er mellom dem | sinussetningen (pass på at det kan finnes to trekanter!) |

## Bevisene (kompetansemål: «begrunne»)

**Arealsetningen:** Tegn høyden $h$ fra $B$ ned på siden $b$. I den rettvinklede trekanten med hypotenus $a$ er $\sin C = \dfrac{h}{a}$, så $h = a \sin C$. Arealet er $\dfrac{1}{2} \cdot \text{grunnlinje} \cdot \text{høyde} = \dfrac{1}{2} \cdot b \cdot a \sin C$.

**Sinussetningen:** Arealet kan skrives på tre måter med arealsetningen:

$$\frac{1}{2}bc\sin A = \frac{1}{2}ac\sin B = \frac{1}{2}ab\sin C$$

Gang med 2 og del på $abc$: $\dfrac{\sin A}{a} = \dfrac{\sin B}{b} = \dfrac{\sin C}{c}$. Snu brøkene, så er du ferdig.

**Cosinussetningen** (for spiss vinkel $A$): Tegn høyden $h$ fra $C$ ned på $c$. Den deler $c$ i to deler: $x = b\cos A$ og $c - x$. Pytagoras i de to rettvinklede trekantene gir $h^2 = b^2 - x^2$ og $a^2 = h^2 + (c - x)^2$. Sett inn:

$$a^2 = b^2 - x^2 + c^2 - 2cx + x^2 = b^2 + c^2 - 2c \cdot b\cos A$$

## Oppgaver

#### Oppgave 6.1 (lett)
I en rettvinklet trekant er hypotenusen 10 cm og en av vinklene 30°. Finn lengden av katetene.

<details markdown="1"><summary>Vis fasit</summary>

Motstående katet: $10 \cdot \sin 30° = 10 \cdot \frac{1}{2} = 5$ cm

Hosliggende katet: $10 \cdot \cos 30° = 10 \cdot \frac{\sqrt{3}}{2} = 5\sqrt{3} \approx 8{,}66$ cm
</details>

#### Oppgave 6.2 (lett)
En rettvinklet trekant har kateter på 6 cm og 8 cm. Finn hypotenusen og den minste vinkelen.

<details markdown="1"><summary>Vis fasit</summary>

Hypotenus: $\sqrt{36 + 64} = 10$ cm

Minste vinkel står overfor den korteste kateten: $\tan v = \dfrac{6}{8}$, så $v \approx 36{,}9°$
</details>

#### Oppgave 6.3 (lett)
Finn eksakt verdi av $\sin 120°$, $\cos 120°$ og $\cos 135°$.

<details markdown="1"><summary>Vis fasit</summary>

$\sin 120° = \sin 60° = \dfrac{\sqrt{3}}{2}$

$\cos 120° = -\cos 60° = -\dfrac{1}{2}$

$\cos 135° = -\cos 45° = -\dfrac{\sqrt{2}}{2}$
</details>

#### Oppgave 6.4 (lett)
I trekant $ABC$ er $a = 7$, $b = 9$ og $C = 40°$. Finn arealet.

<details markdown="1"><summary>Vis fasit</summary>

$A = \dfrac{1}{2} \cdot 7 \cdot 9 \cdot \sin 40° \approx 20{,}2$
</details>

#### Oppgave 6.5 (middels)
I trekant $ABC$ er $A = 50°$, $B = 70°$ og $a = 8$. Finn $b$ og $c$.

<details markdown="1"><summary>Vis fasit</summary>

$C = 180° - 50° - 70° = 60°$

$b = \dfrac{8 \cdot \sin 70°}{\sin 50°} \approx 9{,}81$

$c = \dfrac{8 \cdot \sin 60°}{\sin 50°} \approx 9{,}04$
</details>

#### Oppgave 6.6 (middels)
I trekant $ABC$ er $b = 5$, $c = 7$ og $A = 60°$. Finn $a$.

<details markdown="1"><summary>Vis fasit</summary>

$a^2 = 25 + 49 - 2 \cdot 5 \cdot 7 \cdot \cos 60° = 74 - 35 = 39$

$a = \sqrt{39} \approx 6{,}24$
</details>

#### Oppgave 6.7 (middels)
En trekant har sidene 5, 6 og 7. Finn den største vinkelen.

<details markdown="1"><summary>Vis fasit</summary>

Største vinkel står overfor lengste side (7). Kall den $C$.

$\cos C = \dfrac{5^2 + 6^2 - 7^2}{2 \cdot 5 \cdot 6} = \dfrac{12}{60} = 0{,}2$, så $C \approx 78{,}5°$
</details>

#### Oppgave 6.8 (utfordring)
I trekant $ABC$ er $a = 6$, $b = 8$ og $A = 40°$. Finn vinkel $B$. Hvor mange trekanter finnes det?

<details markdown="1"><summary>Vis fasit</summary>

$\sin B = \dfrac{8 \cdot \sin 40°}{6} \approx 0{,}857$

Kalkulatoren gir $B \approx 59{,}0°$. Men $B = 180° - 59{,}0° = 121{,}0°$ er også en løsning.

Sjekk: $40° + 121{,}0° = 161{,}0° < 180°$, så begge er mulige. Det finnes **to trekanter** (med $C \approx 81{,}0°$ eller $C \approx 19{,}0°$).
</details>

#### Oppgave 6.9 (middels)
Du står 50 m fra foten av et tårn og ser toppen under en vinkel på 35°. Øynene dine er 1,6 m over bakken. Hvor høyt er tårnet?

<details markdown="1"><summary>Vis fasit</summary>

Høyden over øyehøyde: $50 \cdot \tan 35° \approx 35{,}0$ m

Tårnet er $35{,}0 + 1{,}6 \approx 36{,}6$ m høyt.
</details>

#### Oppgave 6.10 (utfordring)
I trekant $ABC$ er $AB = 8$, $AC = 6$ og $\angle A = 60°$. Finn $BC$ og arealet av trekanten. Gi eksakte svar.

<details markdown="1"><summary>Vis fasit</summary>

$BC^2 = 8^2 + 6^2 - 2 \cdot 8 \cdot 6 \cdot \cos 60° = 64 + 36 - 48 = 52$, så $BC = \sqrt{52} = 2\sqrt{13} \approx 7{,}21$

Areal: $\dfrac{1}{2} \cdot 8 \cdot 6 \cdot \sin 60° = 24 \cdot \dfrac{\sqrt{3}}{2} = 12\sqrt{3} \approx 20{,}8$
</details>

#### Oppgave 6.11 (utfordring)
Forklar med egne ord hvorfor arealsetningen er sann. Lag en skisse.

<details markdown="1"><summary>Vis fasit</summary>

Se beviset over: Tegn høyden fra ett hjørne ned på motstående side. Bruk sinus i den rettvinklede trekanten til å uttrykke høyden som $a \sin C$, og sett inn i «grunnlinje ganger høyde delt på 2». Øv på å forklare dette høyt. Det er en typisk muntlig eksamensoppgave!
</details>
