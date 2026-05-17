# Eksempelsett vår 2026

## Del 1 – 3 timer – Uten hjelpemidler


:::::::::::::::{exercise} Oppgave 1
Deriver funksjonene.

:::::::::::::{part} a
$$
f(x) = x^4 - 2e^{3x} + \ln x
$$

::::{answer}
$$
f'(x) = 4x^3 - 6e^{3x} + \frac{1}{x}
$$
::::

:::::::::::::


:::::::::::::{part} b
$$
g(x) = x^7 e^x
$$


::::{answer}
$$
g'(x) = e^x x^6 (x + 7)
$$
::::

::::{solution}
Vi bruker produktregelen for derivasjon:

$$
\begin{align*}
g'(x) &= (x^7)' \cdot e^x + x^7 \cdot (e^x)'  \\
\\
&= 7x^6 \cdot e^x + x^7 \cdot e^x \\
\\
&= e^x (x^7 + 7x^6) \\
\\
&= e^x x^6 (x + 7)
\end{align*}
$$
::::

:::::::::::::


:::::::::::::{part} c
$$
h(x) = \dfrac{\ln (2x)}{x^2}
$$


::::{answer}
$$
h'(x) = \dfrac{2 \ln (2x) - 1}{x^3}
$$
::::

::::{solution}
Vi bruker kvotientregelen for derivasjon:

$$
\begin{align*}
h'(x) &= \dfrac{(x^2)' \cdot \ln (2x) - x^2 \cdot \left[\ln (2x)\right]'}{(x^2)^2} \\
\\
&= \dfrac{2x \cdot \ln (2x) - x^2 \cdot \dfrac{1}{2x} \cdot 2}{x^4} \\
\\
&= \dfrac{2x \cdot \ln (2x) - x}{x^4} \\
\\
&= \dfrac{2 \ln (2x) - 1}{x^3}
\end{align*}
$$
::::
:::::::::::::

:::::::::::::::




---



:::::::::::::::{exercise} Oppgave 2


:::::::::::::{part} a
Løs likningen

$$
4^x - 2 \cdot 2^x = 8
$$


::::{answer}
$$
x = 2
$$
::::


::::{solution}
Vi kan først skrive om likningen til

$$
2^{2x} - 2 \cdot 2^x - 8 = 0
$$

Deretter setter vi $u = 2^x$ som gir oss andregradslikningen

$$
u^2 - 2u - 8 = 0
$$

Vi løser denne med $abc$-formelen som gir

$$
u = \dfrac{2 \pm \sqrt{4 + 32}}{2} = \dfrac{2 \pm \sqrt{36}}{2} = \dfrac{2 \pm 6}{2} = 1 \pm 3    
$$

Altså får vi at

$$
2^x = -2 \or 2^x = 4
$$

Den første av de to er en ugyldig likning. Dermed blir den eneste løsningen av likningen

$$
2^x = 4 \liff x = 2. 
$$
::::
:::::::::::::


:::::::::::::{part} b
Løs likningen

$$
\log_2 (x) + \log_2 (x - 3) = 2
$$



::::{answer}
$$
x = 4
$$
::::

::::{solution}
Vi kan bruke logaritmeregler for å skrive om venstresiden av likningen:

$$
\log_2[x(x - 3)] = 2
$$

Det betyr at

$$
x(x - 3) = 2^2 \liff x^2 - 3x - 4 = 0
$$

Vi løser denne andregradslikningen med $abc$-formelen som gir

$$
x = \dfrac{3 \pm \sqrt{9 + 16}}{2} = \dfrac{3 \pm 5}{2} 
$$

som betyr at

$$
x = 4 \or x = -1
$$

Løsningen kan ikke være negativ fordi da ville $\log_2 (x)$ være udefinert. Dermed er den eneste løsningen av likningen

$$
x = 4.
$$
::::
:::::::::::::

:::::::::::::::



---


:::::::::::::::{exercise} Oppgave 3
Gitt punktene $A(-2, 1)$, $B(2, -1)$, $C(4, 2)$ og $D(t, 3)$ der $t \in \real$.

:::::::::::::{part} a
Avgjør om $\lvec{AB} \perp \lvec{BC}$.


::::{answer}
$\lvec{AB} \not\perp \lvec{BC}$
::::

::::{solution}
Vi finner først vektorene $\lvec{AB}$ og $\lvec{BC}$:

$$
\lvec{AB} = [2 - (-2), -1 - 1] = [4, -2]
$$

$$
\lvec{BC} = [4 - 2, 2 - (-1)] = [2, 3]
$$

Deretter finner vi skalarproduktet av de to vektorene:

$$
\lvec{AB} \cdot \lvec{BC} = 4 \cdot 2 + (-2) \cdot 3 = 8 - 6 = 2
$$

Siden skalarproduktet ikke er lik $0$, så er $\lvec{AB} \not\perp \lvec{BC}$.
::::
:::::::::::::


:::::::::::::{part} b
Bruk vektorregning til å bestemme $t$ slik at $\lvec{AB} \perp \lvec{AD}$.



::::{answer}
$$
t = -1.
$$
::::

::::{solution}
Vi har vektoren $\lvec{AB} = [4, -2]$ fra oppgave **a**. Vi må også finne vektoren $\lvec{AD}$:

$$
\lvec{AD} = [t - (-2), 3 - 1] = [t + 2, 2]
$$

For at $\lvec{AB} \perp \lvec{AD}$, så må skalarproduktet av de to vektorene være lik $0$:

$$
\lvec{AB} \cdot \lvec{AD} = 4(t + 2) + (-2) \cdot 2 = 4t + 8 - 4 = 4t + 4
$$

Altså må 

$$
4t + 4 = 0 \liff t = -1.
$$
::::
:::::::::::::


:::::::::::::{part} c
Bestem $t$ slik at $\vec{AB} \parallel \vec{CD}$.



::::{answer}
$$
t = 2
$$
::::

::::{solution}
Fra oppgave **a** har vi at

$$
\lvec{AB} = [4, -2]
$$

Vi finner også vektoren $\lvec{CD}$:

$$
\lvec{CD} = [t - 4, 3 - 2] = [t - 4, 1]
$$

For at de to vektorene skal være parallelle, må forholdstallet mellom vektorkomponentene være like. Det vil si

$$
\dfrac{4}{t - 4} = \dfrac{-2}{1} \liff 4 = -2(t - 4) \liff 4 = -2t + 8 \liff -2t = -4 \liff t = 2.
$$

Altså må $t = 2$ for at $\lvec{AB} \parallel \lvec{CD}$.
::::

:::::::::::::

:::::::::::::::




---


:::::::::::::::{exercise} Oppgave 4
:::{plot}
axis: equal
fontsize: 28
width: 100%
align: right
xmin: -1
ymin: -1
xmax: 3
ymax: 3
function: sqrt(4 - x**2), (0, 2)
def: f(x) = sqrt(4 - x**2)
let: a = 1.4
let: Ox = 0
let: Oy = 0
let: Ax = a
let: Ay = 0
let: Bx = a
let: By = f(a)
let: Cx = 0
let: Cy = f(a)
polygon: (Ox, Oy), (Ax, Ay), (Bx, By), (Cx, Cy)
ticks: off
text: Ox, Oy, "$O$", bottom-left
text: Ax, Ay, "$A(x, 0)$", bottom-center
text: Bx, By, "$B$", top-right
text: Cx, Cy, "$C$", center-left
fill-between: f(x), f(a), (0, a), blue, 0.2, where=above
fill-between: f(x), 0, (a, 2), blue, 0.2, where=above
nocache:
:::

Figuren til høyre viser en kvartsirkel med radius $2$. Funksjonen for kvartsirkelen er gitt ved

$$
f(x) = \sqrt{4 - x^2} \qfor 0 \leq x \leq 2.
$$

Firkanten $OABC$ er et rektangel, der $O$ er origo, $A$ ligger på $x$-aksen, $B$ ligger på kvartsirkelen og $C$ ligger på $y$-aksen.


:::{clear}
:::


:::::::::::::{part} a
Bestem en eksakt verdi for arealet når $x = 1$.


::::{answer}
$$
T_\mathrm{fargelagt} = \pi - \sqrt{3}
$$
::::

::::{solution}
Arealet av det fargelagte området blir 

$$
T_\mathrm{fargelagt} = T_\mathrm{kvartsirkel} - T_\mathrm{rektangel}
$$

Arealet av kvartsirkelen er gitt ved 

$$
T_\mathrm{kvartsirkel} = \dfrac{1}{4} \pi \cdot 2^2 = \pi
$$

Arealet av rektangelet er gitt ved

$$
T_\mathrm{rektangel} = 1 \cdot f(1) = 1 \cdot \sqrt{4 - 1^2} = 1 \cdot \sqrt{3} = \sqrt{3}
$$

Altså er arealet av det fargelagte området lik

$$
T_\mathrm{fargelagt} = \pi - \sqrt{3}
$$

::::
:::::::::::::


:::::::::::::{part} b
Bestem det minste arealet det fargelagte området kan ha.



::::{answer}
$$
T_\mathrm{minst} = \pi - 2
$$
::::


::::{solution}
Arealet $T(x)$ av det fargelagte området vil være gitt ved

$$
T(x) = \pi - xf(x) = \pi - x\sqrt{4 - x^2}
$$

Vi deriverer $T(x)$ for å finne kritiske punkter:

$$
\begin{align*}
T'(x) &= -\sqrt{4 - x^2} - x \cdot \dfrac{-2x}{2\sqrt{4 - x^2}} \\
\\
&= -\sqrt{4 - x^2} + \dfrac{x^2}{\sqrt{4 - x^2}} \\
\end{align*}
$$

Så løser vi $T'(x) = 0$ som gir

$$
T'(x) = 0 \liff -\sqrt{4 - x^2} + \dfrac{x^2}{\sqrt{4 - x^2}} = 0
$$

som vi kan skrive om til

$$
\sqrt{4 - x^2} = \dfrac{x^2}{\sqrt{4 - x^2}}
$$

Vi ganger med $\sqrt{4 - x^2}$ på begge sider av likningen som gir oss

$$
4 - x^2 = x^2 \liff 4 = 2x^2 \liff x^2 = 2 \liff x = \sqrt{2}.
$$

Arealet i dette punktet vil være

$$
T(\sqrt{2}) = \pi - \sqrt{2} \cdot \sqrt{4 - 2} = \pi - \sqrt{2} \cdot \sqrt{2} = \pi - 2.
$$

Vi sjekker at arealet er større i endepunktene for å være sikre på at dette er det minste arealet:

$$
T(0) = \pi - 0 \cdot \sqrt{4 - 0^2} = \pi
$$

$$
T(2) = \pi - 2 \cdot \sqrt{4 - 2^2} = \pi
$$

Altså er det minste arealet det fargelagte området kan ha gitt ved

$$
T_\mathrm{minst} = \pi - 2.
$$
::::
:::::::::::::


:::::::::::::::





---




:::::::::::::::{exercise} Oppgave 5
Funksjonen $f$ er gitt ved

$$
f(x) = \begin{cases}
    x^2 + bx & \qhvis x \lt 1 \\
    \\
    e^{a(x - 1)} + 3 & \qhvis x \geq 1
\end{cases}
$$

Bestem $a$ og $b$ slik at $f$ er kontinuerlig og deriverbar i $x = 1$.


::::{answer}
$$
a = 5 \and b = 3.
$$
::::

::::{solution}
Vi lar 

$$
p(x) = x^2 + bx \qog q(x) = e^{a(x - 1)} + 3.
$$


For at $f$ skal være kontinuerlig i $x = 1$, så må vi kreve at

$$
p(1) = q(1) \liff 1 + b = 4 \liff b = 3.
$$

For at $f$ skal være deriverbar i $x = 1$, så må også kreve at

$$
p'(1) = q'(1).
$$

Vi finner først $p'(x)$ og $q'(x)$:

$$
p'(x) = 2x + b
$$

$$
q'(x) = ae^{a(x - 1)}
$$

Altså må vi ha at

$$
p'(1) = q'(1) \liff 2 + b = ae^{0} \liff 2 + 3 = a \liff a = 5.
$$

Altså er $f$ kontinuerlig og deriverbar i $x = 1$ dersom

$$
a = 5 \and b = 3.
$$
::::

:::::::::::::::


---


:::::::::::::::{exercise} Oppgave 6
:::::::::::::{part} a
Bestem grenseverdien

$$
\lim_{x\to 4} \dfrac{x - 4}{2 - \sqrt{x}}
$$


::::{answer}
$$
\lim_{x\to 4} \dfrac{x - 4}{2 - \sqrt{x}} = -4
$$
::::


::::{solution}
Vi prøver å sette inn $x = 4$ direkte i uttrykket:

$$
\lim_{x\to 4} \dfrac{x - 4}{2 - \sqrt{x}} = \dfrac{4 - 4}{2 - \sqrt{4}} = \dfrac{0}{2 - 2} = \dfrac{0}{0}
$$

Vi får et ubestemt uttrykk på formen $0/0$ så da kan vi bruke L'Hôpitals regel: 

$$
\lim_{x\to 4} \dfrac{x - 4}{2 - \sqrt{x}} \overset{[\frac{0}{0}]}{=} \lim_{x\to 4} \dfrac{1}{-\dfrac{1}{2\sqrt{x}}} = \lim_{x\to 4} -2\sqrt{x} = -4.
$$
::::
:::::::::::::


:::::::::::::{part} b
Bestem $a$ slik at grenseverdien nedenfor eksisterer.

$$
\lim_{x\to a} \dfrac{8 - \sqrt{ax}}{x - a}
$$


Bestem grenseverdien for denne verdien av $a$.


::::{answer}
$$
a = 8 \and \lim_{x\to a} \dfrac{8 - \sqrt{ax}}{x - a} = -\dfrac{1}{2}.
$$
::::


::::{solution}
Setter vi inn $x = a$ i uttrykket, så får vi $0$ i nevneren. Den eneste måten grenseverdien kan eksistere er dersom vi også får $0$ i telleren: 

$$
8 - \sqrt{a^2} = 8 - \abs{a} = 0 \liff \abs{a} = 8
$$

Vi må forutsette at $a > 0$, så den eneste muligheten er

$$
a = 8.
$$

Grenseverdien blir da

$$
\lim_{x\to 8} \dfrac{8 - \sqrt{8x}}{x - 8} \overset{[\frac{0}{0}]}{=} \lim_{x\to 8} \dfrac{-\dfrac{1}{2\sqrt{8x}} \cdot 8}{1} = \lim_{x\to 8} -\dfrac{4}{\sqrt{8x}} = -\dfrac{4}{\sqrt{64}} = -\dfrac{4}{8} = -\dfrac{1}{2}.
$$
::::
:::::::::::::


:::::::::::::::





---



:::::::::::::::{exercise} Oppgave 7
For to vektorer $\vec{a}$ og $\vec{b}$ er

* $\abs{\vec{a}} = 4$
* $\abs{\vec{b}} = 5$
* $\cos \varphi = \dfrac{1}{2}$ der $\varphi$ er vinkelen mellom $\vec{a}$ og $\vec{b}$.


:::::::::::::{part} a
Bestem $\vec{a} \cdot \vec{b}$.


::::{answer}
$$
\vec{a} \cdot \vec{b} = 10.
$$
::::


::::{solution}
Den geometriske formelen for skalarproduktet av to vektorer er gitt ved

$$
\vec{a} \cdot \vec{b} = \abs{\vec{a}} \cdot \abs{\vec{b}} \cdot \cos \varphi
$$

Ergo får vi at 

$$
\vec{a} \cdot \vec{b} = 4 \cdot 5 \cdot \dfrac{1}{2} = 10.
$$
::::
:::::::::::::

En vektor $\vec{p}$ er gitt ved

$$
\vec{p} = 2\vec{a} + t \cdot \vec{b}
$$


:::::::::::::{part} b
Bestem $t$ slik at $\abs{\vec{p}}$ er minst mulig.


::::{answer}
$$
t = -\dfrac{4}{5}.
$$
::::

::::{solution}
Vi ønsker å gjøre $\abs{\vec{p}}$ minst mulig. Det kan vi gjøre ved å gjøre $\abs{\vec{p}}^2$ minst mulig. Vi har at

$$
\begin{align*}
\abs{\vec{p}}^2 &= \vec{p} \cdot \vec{p} \\
\\
&= (2\vec{a} + t \cdot \vec{b}) \cdot (2\vec{a} + t \cdot \vec{b}) \\
\\
&= 4\vec{a} \cdot \vec{a} + 4t \cdot \vec{a} \cdot \vec{b} + t^2 \cdot \vec{b} \cdot \vec{b} \\
\\
&= 4 \cdot 16 + 4t \cdot 10 + t^2 \cdot 25 \\
\\
&= 64 + 40t + 25t^2 \\
\\
&= 25t^2 + 40t + 64
\end{align*}
$$

Vi deriverer og setter lik $0$ for å finne kritiske punkter:

$$
(25t^2 + 40t + 64)' = 0 \liff 50t + 40 = 0 \liff t = -\dfrac{4}{5}.
$$

Altså blir $\abs{\vec{p}}$ minst mulig når $t = -\dfrac{4}{5}$.
::::
:::::::::::::


:::::::::::::::


## Del 2 – 2 timer – Med hjelpemidler


:::::::::::::::{exercise} Oppgave 1
---
aids: true
---

Tabellen nedenfor viser hvor mange prosent strøm en telefon som opprinnelig var tom for strøm har $t$ minutter etter at den blir koblet til laderen.

:::{table}
---
transpose: true
---
labels: Tid (minutter), Batteristrøm (prosent)
$5$, $7$
$10$, $11$
$15$, $17$
$20$, $25$
$40$, $72$
$60$, $94$
:::


:::::::::::::{part} a
Lag en modell for batteristrømmen $B(t)$ (prosent), $t$ minutter etter at telefonen blir koblet i laderen på formen

$$
B(t) = \dfrac{c}{1 + a\cdot e^{-b\cdot t}}
$$


::::{answer}
$$
B(t) = \dfrac{98.5}{1 + 22.5 e^{-0.1 \cdot t}}
$$
::::

::::{solution}
Vi legger inn datapunktene i et regneark:

:::{figure} ./figurer/1/a/regneark.png
---
class: no-click, adaptive-figure
width: 40%
---
:::

Deretter bruker vi {ggb-icon}`mode_regression` til å lage en *logistisk* regresjonsmodell for datapunktene:

:::{figure} ./figurer/1/a/regresjonsmodell.png
---
class: no-click, adaptive-figure
width: 70%
---
:::

Altså er en god logistisk modell for batteristrømmen til telefonen gitt ved

$$
B(t) = \dfrac{98.5}{1 + 22.5 e^{-0.1 \cdot t}}
$$


::::


:::::::::::::


I resten av oppgaven skal du bruke modellen

$$
B(t) = \dfrac{100}{1 + 22 \cdot e^{-0.1 \cdot t}}
$$

:::::::::::::{part} b
Ved hvilket tidspunkt lades telefonen raskest ifølge modellen? 

Hvor raskt øker batteriprosenten på dette tidspunktet?


::::{answer}
ca. $2.5~\%$ per minutt etter $30.9$ minutter.
::::


::::{solution}
Siden modellen er en logistisk modell, vil $B(t) = 100/2 = 50$ gi oss tidspunktet hvor telefonen lades raskest. Vi kan deretter finne hvor raskt batteriprosenten øker ved å regne ut $B'(t)$ i dette tidspunktet:

:::{figure} ./figurer/1/b/sol.png
---
class: no-click, adaptive-figure
width: 70%
---
:::

Altså øker batteriprosenten raskest med ca. $2.5~\%$ per minutt etter $30.9$ minutter.

::::
:::::::::::::



:::::::::::::::




---


:::::::::::::::{exercise} Oppgave 2
---
aids: true
---

Funksjonen $f$ er gitt ved

$$
f(x) = \dfrac{1}{3}x^3 - 2x^2 + 3x + 1
$$

:::::::::::::{part} a
Bestem det største intervallet $I = [a, b]$ der $f$ har en omvendt funksjon og $2 \in I$


::::{answer}
$$
I = [1, 3].
$$
::::


::::{solution}
For at $f$ skal ha en omvendt funksjon på intervallet $I$, må vi sørge for at det ikke finnes noen ekstremalpunkter på innsiden av intervallet. Vi løser derfor $f'(x) = 0$:


:::{figure} ./figurer/2/a/sol.png
---
class: no-click, adaptive-figure
width: 70%
---
:::

som gir $x = 1$ og $x = 3$. Vi må sjekke at dette er ekstremalpunkter som vi kan gjøre med andrederiverttesten:

:::{figure} ./figurer/2/a/sol2.png
---
class: no-click, adaptive-figure
width: 70%
---
:::

I begge tilfeller er $f''(x) \neq 0$ som betyr at begge punkter er ekstremalpunkter. Vi skal også sørge for at $2 \in I$ som betyr at det største intervallet som sørger for at $f$ har en omvendt funksjon og $2 \in I$ er gitt ved

$$
I = [1, 3].
$$

::::

:::::::::::::

La $g$ være den omvendte funksjonen til $f$. Det finnes to punkter på grafen til $g$ der $g'(x) = -\dfrac{4}{3}$.

:::::::::::::{part} b
Finn koordinatene til disse punktene.



::::{answer}
$\left(\dfrac{17}{8}, \dfrac{3}{2}\right)$ og $\left(\dfrac{29}{24}, \dfrac{5}{2}\right)$
::::

::::{solution}
I punktet $(y, x)$ på grafen til $g$ vil tilsvare et punkt $(x, y)$ på grafen til $f$ siden de er omvendte funksjoner. Da har vi også at

$$
f'(x) = \dfrac{1}{g'(y)} = \dfrac{1}{-\dfrac{4}{3}} = -\dfrac{3}{4}.
$$

Vi løser derfor $f'(x) = -\dfrac{3}{4}$ som gir oss

:::{figure} ./figurer/2/b/sol.png
---
class: no-click, adaptive-figure
width: 70%
---
:::

Altså er punktene $\left(\dfrac{3}{2}, \dfrac{17}{8}\right)$ og $\left(\dfrac{5}{2}, \dfrac{29}{24}\right)$ punkter på grafen til $f$ der $f'(x) = -\dfrac{3}{4}$. Det betyr at punktene $\left(\dfrac{17}{8}, \dfrac{3}{2}\right)$ og $\left(\dfrac{29}{24}, \dfrac{5}{2}\right)$ er punkter på grafen til $g$ der $g'(x) = -\dfrac{4}{3}$.
::::
:::::::::::::

:::::::::::::::


---

:::::::::::::::{exercise} Oppgave 3
---
aids: true
---

En golfball blir slått ut fra et tak som er 20 meter over bakkenivå.

Posisjonen til golfballen er gitt ved vektorfunksjonen

$$
\vec{r}(t) = [17t, -5t^2 + 29t + 20]
$$


Her er $t$ tiden (målt i sekunder) etter at ballen blir slått ut fra taket, og koordinatene er gitt i meter. Førstekoordinaten er posisjon i horisontal retning, og andrekoordinaten er høyden til ballen over bakkenivå.


:::::::::::::{part} a
Hvor lang tid tar det før golfballen treffer bakken?


::::{answer}
Ca. $6.42$ sekunder.
::::

::::{solution}
Golfballen treffer bakken når $y$-komponenten er lik $0$ så vi løser $y(t) = 0$ med CAS:

:::{figure} ./figurer/3/a/sol.png
---
class: no-click, adaptive-figure
width: 70%
---
:::

Altså treffer golfballen bakken etter ca. $6.42$ sekunder.
::::
:::::::::::::

:::::::::::::{part} b
Bestem banefarten til golfballen i det øyeblikket den blir slått ut fra taket.


::::{answer}
ca. $33.6~\mathrm{m/s}$
::::

::::{solution}
Banefarten til golfballen idet den blir slått ut er gitt ved $\abs{\vec{r}'(0)}$. Vi regner ut med CAS:

:::{figure} ./figurer/3/b/sol.png
---
class: no-click, adaptive-figure
width: 70%
---
:::

Altså er banefarten til golfballen idet den blir slått ut ca. $33.6~\mathrm{m/s}$

::::

:::::::::::::

Ved $t = 0$ befinner en fugl seg i punktet $(20, 10)$. Fuglen flyr langs en rett linje med konstant banefart og fanger ballen når den er i sitt høyeste punkt over bakken.

:::::::::::::{part} c
Bestem banefarten til fuglen.



::::{answer}
Ca. $20.6~\mathrm{m/s}$.
::::

::::{solution}
Golfballen er i sitt høyest punkt når $y'(t) = 0$. Vi løser likningen med CAS som gir:

:::{figure} ./figurer/3/c/sol1.png
---
class: no-click, adaptive-figure
width: 70%
---
:::

Altså er golfballen i sitt høyeste punkt når $t = \dfrac{29}{10}$. Koordinatene til punktet er $\vec{r}\left(\dfrac{29}{10}\right)$. Fuglen må flytte seg fra $(20, 10)$ til dette punktet på $\dfrac{29}{10}$ sekunder. Banefarten til fuglen er da gitt ved

$$
v = \dfrac{s}{t} = \dfrac{\abs{\vec{r}\left(\dfrac{29}{10}\right) - [20, 10]}}{\dfrac{29}{10}}
$$

Vi regner ut dette med CAS:

:::{figure} ./figurer/3/c/sol2.png
---
class: no-click, adaptive-figure
width: 70%
---
:::

Altså var banefarten til fuglen omtrent $20.6~\mathrm{m/s}$.
::::

:::::::::::::


:::::::::::::::




---



:::::::::::::::{exercise} Oppgave 4
---
aids: true
---

En sirkel har sentrum i $S(3, 4)$. Et punkt $A(0, 8)$ ligger på sirkelen. En linje $\ell$ tangerer sirkelen i et punkt $P$ og har stigningstall $-\dfrac{3}{4}$. 

Ved å plassere et tredje punkt $Q$ på sirkelen kan vi lage ulike trekanter.

Finn koordinatene til $P$ og $Q$ som gir trekanten med størst mulig areal.


::::{answer}
$$
P(0, 0) \qog Q(8, 4).
$$
::::

::::{solution}
:::{plot}
align: right
width: 100%
axis: equal
axis: off
let: Sx = 3
let: Sy = 4
let: r = 5
circle: (Sx, Sy), r, blue, solid
let: Ax = 0
let: Ay = 8
point: (Ax, Ay)
text: Ax, Ay, "$A(0, 8)$", top-left
point: (Sx, Sy)
text: Sx, Sy, "$S(3, 4)$", bottom-right
let: P1x = 6
let: P1y = 8
point: (P1x, P1y)
text: P1x, P1y, "$P_1$", top-right
let: vx = 4
let: vy = -3
line-segment: (P1x - vx, P1y - vy), (P1x + vx, P1y + vy), red, solid
let: P2x = 0
let: P2y = 0
point: (P2x, P2y)
text: P2x, P2y, "$P_2$", bottom-left
line-segment: (P2x - vx, P2y - vy), (P2x + vx, P2y + vy), red, solid
fontsize: 32
:::

Tangenten kan gå gjennom to forskjellige punkter $P_1$ og $P_2$ som vist i figuren til høyre.

Tangenten har stigningstall $-\dfrac{3}{4}$, så en retningsvektor for tangenten er gitt ved

$$
\vec{v} = \left[1, -\dfrac{3}{4}\right] \cdot 4 = [4, -3].
$$

Vektoren $\lvec{SP}_1$ må være ortogonal med $\vec{v}$, som betyr at den er parallell med en tverrvektor til $\vec{v}$. En tverrvektor til $\vec{v}$ er gitt ved

$$
\vec{v}_\perp = [3, 4].
$$

Vektoren $\lvec{SP}_1$ må ha samme lengde som radiusen til sirkelen. Radiusen kan vi finne ved

$$
r = \abs{\lvec{SA}} = \abs{[0 - 3, 8 - 4]} = \abs{[-3, 4]} = 5.
$$

Altså har $\vec{v}_\perp$ riktig lengde allerede som betyr at $\lvec{SP}_1 = \vec{v}_\perp$. Koordinatene til $P_1$ får vi ved å følge tverrvektoren fra sentrum:

$$
\lvec{OP}_1 = \lvec{OS} + \vec{v}_\perp = [3, 4] + [3, 4] = [6, 8].
$$

Koordinatene til $P_2$ får vi ved å følge tverrvektoren fra sentrum i motsatt retning:

$$
\lvec{OP}_2 = \lvec{OS} - \vec{v}_\perp = [3, 4] - [3, 4] = [0, 0].
$$



:::{plot}
align: right
width: 100%
axis: equal
axis: off
let: Sx = 3
let: Sy = 4
let: r = 5
circle: (Sx, Sy), r, blue, solid
let: Ax = 0
let: Ay = 8
point: (Ax, Ay)
text: Ax, Ay, "$A(0, 8)$", top-left
point: (Sx, Sy)
text: Sx, Sy, "$S(3, 4)$", bottom-right
let: P1x = 6
let: P1y = 8
point: (P1x, P1y)
text: P1x, P1y, "$P_1(6, 8)$", top-right
let: vx = 4
let: vy = -3
let: Mx = 0.5 * (P1x + Ax)
let: My = 0.5 * (P1y + Ay)
point: (Mx, My)
text: Mx, My, "$M_1$", bottom-left
line-segment: (Ax, Ay), (P1x, P1y), solid, red
let: Q1x = 3
let: Q1y = -1
point: (Q1x, Q1y)
text: Q1x, Q1y, "$Q_1$", bottom-right
line-segment: (Mx, My), (Q1x, Q1y), dashed, gray
line-segment: (Ax, Ay), (Q1x, Q1y), solid, red
line-segment: (P1x, P1y), (Q1x, Q1y), solid, red
fontsize: 32
:::

Vi tenker oss nå at $P_1$ er tangeringspunktet. Da vil punktet $Q_1$ som gir en trekant med størst mulig areal, være plassert på sirkelen slik at det har størst mulig avstand fra linjestykke $AP_1$. Hvis vi lar $M_1$ være midtpunktet på linjestykke $AP_1$, så vil linjestykke fra $M_1$ til $Q_1$ være det som gir størst mulig avstand. Vi finner først koordinatene til $M_1$:

$$
\begin{align*}
\lvec{OM}_1 &= \dfrac{\lvec{OA} + \lvec{OP}_1}{2} \\
\\
&= \dfrac{[0, 8] + [6, 8]}{2} \\
\\
&= [3, 8].
\end{align*}
$$

Vektoren $\lvec{M_1Q_1}$ vil være parallell med $\lvec{M_1S}$. Vi kan dele opp vektoren som

$$
\lvec{M_1Q_1} = \lvec{M_1S} + \dfrac{\lvec{M_1S}}{\abs{\lvec{M_1S}}} \cdot r
$$

siden vi først må flytte oss fra $M_1$ til sentrum og deretter flytter vi oss i samme retning med en lengde lik radiusen til sirkelen. Da får vi at

$$
\lvec{M_1Q_1} = [0, -4] + \dfrac{[0, -4]}{\abs{[0, -4]}} \cdot 5 = [0, -4] + [0, -5] = [0, -9].
$$

Ergo blir koordinatene til $Q_1$:

$$
\lvec{OQ}_1 = \lvec{OM}_1 + \lvec{M_1Q_1} = [3, 8] + [0, -9] = [3, -1].
$$

Arealet av trekanten $AP_1Q_1$ blir 

$$
T_1 = \dfrac{1}{2} \cdot \abs{\lvec{AP}_1} \cdot \abs{\lvec{M_1Q}_1} = \dfrac{1}{2} \cdot 6 \cdot 9 = 27.
$$


:::{plot}
align: right
width: 100%
axis: equal
axis: off
let: Sx = 3
let: Sy = 4
let: r = 5
circle: (Sx, Sy), r, blue, solid
let: Ax = 0
let: Ay = 8
point: (Ax, Ay)
text: Ax, Ay, "$A(0, 8)$", top-left
point: (Sx, Sy)
text: Sx, Sy, "$S(3, 4)$", bottom-right
let: P1x = 0
let: P1y = 0
point: (P1x, P1y)
text: P1x, P1y, "$P_2(0, 0)$", bottom-left
let: vx = 4
let: vy = -3
let: Mx = 0.5 * (P1x + Ax)
let: My = 0.5 * (P1y + Ay)
point: (Mx, My)
text: Mx, My, "$M_2$", bottom-left
line-segment: (Ax, Ay), (P1x, P1y), solid, red
let: Q1x = 8
let: Q1y = 4
point: (Q1x, Q1y)
text: Q1x, Q1y, "$Q_2$", bottom-right
line-segment: (Mx, My), (Q1x, Q1y), dashed, gray
line-segment: (Ax, Ay), (Q1x, Q1y), solid, red
line-segment: (P1x, P1y), (Q1x, Q1y), solid, red
fontsize: 32
:::


Vi gjentar de samme utregningene for $P_2$. Vi har da at midtpunktet $M_2$ på linjestykke $AP_2$ har koordinatene

$$
\begin{align*}
\lvec{OM}_2 &= \dfrac{\lvec{OA} + \lvec{OP}_2}{2} \\
\\
&= \dfrac{[0, 8] + [0, 0]}{2} \\
\\
&= [0, 4].
\end{align*}
$$

Vektoren $\lvec{M_2Q_2}$ vil være parallell med $\lvec{M_2S}$. Vi kan dele opp vektoren som

$$
\lvec{M_2Q_2} = \lvec{M_2S} + \dfrac{\lvec{M_2S}}{\abs{\lvec{M_2S}}} \cdot r
$$

Da får vi 

$$
\lvec{M_2Q_2} = [3, 0] + \dfrac{[3, 0]}{\abs{[3, 0]}} \cdot 5 = [3, 0] + [5, 0] = [8, 0].
$$

Ergo blir koordinatene til $Q_2$:

$$
\lvec{OQ}_2 = \lvec{OM}_2 + \lvec{M_2Q_2} = [0, 4] + [8, 0] = [8, 4].
$$

Arealet av trekanten $AP_2Q_2$ blir

$$
T_2 = \dfrac{1}{2} \cdot \abs{\lvec{AP}_2} \cdot \abs{\lvec{M_2Q}_2} = \dfrac{1}{2} \cdot 8 \cdot 8 = 32.
$$

Dette blir den trekanten som har det største arealet, så koordinatene til $P$ og $Q$ må være 

$$
P(0, 0) \qog Q(8, 4).
$$





::::

:::::::::::::::

