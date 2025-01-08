>[!note]
>Considerando la definizione di limite per funzioni continue, se $x_{0}\in(D\cap D')\wedge l=f(x_{0})$ si dice che la funzione è continua nel punto $x_{0}$, in simboli:
>$$\begin{align*}
\forall\varepsilon>0,\exists\delta(\varepsilon)>0\quad &|\quad x\in(D\smallsetminus\set{0})\cap(x_{0}-\delta(\varepsilon),x_{0}+\delta(\varepsilon))\\
&\Longrightarrow f(x)\in(l-\varepsilon,l+\varepsilon)
\end{align*}$$
### Proprietà delle funzione continua
Considero una funzione $f: D\to C\quad,\quad D\subseteq\mathbb{R}\quad,\quad C:=\set{\text{funzioni continue }\forall x\in D}$:

1. Somma: $$f,g\in C(D)\Longrightarrow (f+g)\in C(D)$$
2. Prodotto: $$f,g\in C(D)\Longrightarrow (f\cdot g)\in C(D)$$
3. Quoziente: $$f,g\in C(D)\Longrightarrow \left(\frac{f}{g}\right)\in C(D)\quad g\neq 0$$
4. Inversa: $$\begin{align*}
f:(a,b)\to (c,d)\quad,\quad f\in C(D)&\Longrightarrow f^{-1}\in C(D)\quad,\quad g\neq0\\
&\Longrightarrow f^{-1}\in C)c,d
\end{align*}$$
5. Composta: $$\begin{cases}
f\in C(D(f)) \\
g\in C(D(g)) \\
\text{Im}(f)\subseteq D(g)
\end{cases}\Longrightarrow (f\circ g)\in C(D(f))$$
6. Potenza ennesima: $$f: D\to C\quad,\quad f_{n}(x)=x^{n}\in C(\mathbb{R})\quad\forall x\in D, n\geq 0$$
7. Continuità dei polinomi: $$P_{n}(x)=\sum\limits_{i=0}^{n}c_{n}x^{n}=(c_{0}+c_{1}x^{1}+c_{2}x^{2}+\cdots+ c_{n}x^{n})\in C$$
8. Continuità di funzioni razionali: $$R(x)= \frac{P(x)}{Q(x)}\quad D(R):=\set{x\in\mathbb{R}\text{ }|\space Q(x)\neq0}$$$$P,Q\in C(R)\Longrightarrow R= \frac{p}{q}$$
9. Continuità del seno e del coseno:
$$\sin,\cos\in C(\mathbb{R})$$

### Teorema di Weierstrass
>[!note]
>Sia $f\in C([a,b])$ una funzione continua sull'intervallo chiuso e limitato $[a,b]\subset\mathbb{R}$. Esistono allora il massimo e minimo globali di $f$ su $[a,b]$:
>$$\exists x_{m},x_{M}\in[a,b]\quad |\quad x\in[a,b]\Longrightarrow f(x_{m})\leq f(x)\leq f(x_{M})$$
>In altre parole, $M:=f(x_{M})$ è il valore massimo e $m:=f(x_{m})$ è il valore minimo di $f$ su $[a,b].$

>[!example] Dimostrazione
>Ci limiteremo a provare l'esistenza del massimo.
>
>Sia $M:=\sup(\text{Im}(f))\in\mathbb{R}\cup\set{+\infty}$ l'estremo superiore dell'immagine $\text{Im}(f):=\set{f(x)\in\mathbb{R}:\quad x\in[a,b]}$ della funzione.
>Per le proprietà dell'estremo superiore (sia finito che infinito), esiste una successione $\set{y_{n}}_{n\in\mathbb{N}}\subset\text{Im}(f)$ tale che $\lim\limits_{n}y_{n}=M$. Esiste quindi una corrispondente successione $\set{x_{n}}_{n\in\mathbb{N}}\subset[a,b]$ tale che $f(x_{n})=y_{n}$ e per la quale, evidentemente: $$\lim_{n}f(x_{n})=\lim_{n}y_{n}=M$$
>Se la successione $\set{x_{n}}_{n\in\mathbb{N}}\subset[a,b]$ assumesse solo un numero finito di valori, anche $\set{y_{n}}_{n\in\mathbb{N}}\subset\text{Im}(f)$ assumerebbe solo n numero finito di valori. Ma poiché $\lim\limits_{n}y_{n}=M$, esisterebbe un certo $n\in\mathbb{N}$ per il quale $y_{n}=M$.
>Si avrebbe allora $M=y_{n}\in\text{Im}(f)\subseteq\mathbb{R}$, e quindi $M$ sarebbe infinito ed un valore massimo per $f$ ($x_{n}\in[a,b]$ sarebbe allora un punto di massimo $x_{M}$ cercato)
>
>Se invece $\set{x_{n}}_{n\in\mathbb{N}}$ fosse costituita da un numero infinito di valori, in quanto insieme limitato, per il teorema di Bolzano-Weierstrass sull'esistenza di punti di accumulazione di insiemi limitati ed infiniti, ammetterebbe almeno un punto di accumulazione $x_{M}\in[a,b]$. Esisterebbe quindi almeno una sotto-successione $\set{x_{n_{k}}}_{k\in\mathbb{N}}\subseteq\set{x_{n}}_{n\in\mathbb{N}}$ convergente a $x_{M}$ e $\lim\limits{k}=x_{n_{k}}=x_{M}$, per continuità di $f$ si avrebbe: $$M=\lim_{n\to\infty} y_{n}=\lim_{n\to\infty} f(x_{n})=\lim_{k\to\infty} f(x_{n_{k}})= f(\lim_{k\to\infty} x_{n_{k}})=f(x_{M})\in\text{Im}(f)\subseteq\mathbb{R}$$
>Questo dimostrerebbe che $M:=\sup(\text{Im}(f))\in\mathbb{R}$ è finito e che appartiene a $\text{Im}(f)$. $M$ sarebbe quindi il valore massimo di $\text{Im}(f)$, assunto da $f$ in $x_{M}\in[a,b]$ (punto di massimo).
### Teorema degli zeri
>[!note]
>Sia data una funzione continua $f\in C([a,b])$ sull'intervallo chiuso e limitato $[a,b]\subset\mathbb{R}$. Se $$f(a)\cdot f(b)<0\quad\text{cioè}\quad\text{sgn}(f(a))\neq\text{sgn}(f(b))$$
allora $$\exists x_{0}\in(a,b)\quad |\quad f(x_{0})=0$$

>[!example] Dimostrazione
>Per comodità di notazione poniamo $a_{0}:= a$ e $b_{0}:= b$, per cui: $$f(a_{0})\cdot f(b_{0})<0$$
>Sia $c:=\frac{a_{0}+b_{0}}{2}$ il punto medio di $[a_{0},b_{0}]$. Se $f(c)=0$ abbiamo trovato il punto $x_{0}:= c$ dove $f$ si annulla. Altrimenti, tra $[a_{0},c]$ e $[c,b_{0}]$, denotiamo con $[a_{1},b_{1}]$ quello a cui estremi $f$ assume il segno opposto: $$f(a_{1})\cdot f(b_{1})<0$$
>Iterando questo procedimento, a meno che in uno dei punti medi ottenuti la funzione si annulli, otteniamo una successione decrescente di intervalli: $$\cdots\subset[a_{n+1},b_{n+1}]\subset[a_{n},b_{n}]\subset\cdots\subset[a_{1},b_{1}]\subset[a_{0},b_{0}]$$
>tali che $$f(a_{n})\cdot f(b_{n})<0\qquad\forall n\in\mathbb{N}$$
>Definiamo le successioni $\set{a_{n}}$ crescente e superiormente limitata da $b_{0}$, e la successione $\set{b_{n}}$ decrescente e inferiormente limitata da $a_{0}$: $$\begin{align*}
>\cdots\leq a_{n}\leq a_{n+1}\leq\cdots\leq b_{0}\\
>a_{0}\leq\cdots\leq b_{n+1}\leq b_{n}\leq\cdots
>\end{align*}$$
>Per il teorema della convergenza di successioni monotone limitate in $\mathbb{R}$, entrambe le successioni convergono. Inoltre Poiché: $$\lim_{n\to+\infty} b_{n}-a_{n}=\lim_{n\to+\infty}\frac{b_{0}-a_{0}}{2^{n}}=0$$
>Per le proprietà del limite, esiste un $\overline{x}\in\mathbb{R}$ limite comune delle due successioni: $$\exists!\overline{x}=\lim_{n\to+\infty}a_{n}=\lim_{n\to+\infty}b_{n}\in\mathbb{R}$$
>Passando al limite, per il teorema della permanenza del segno, e poiché $f$ è continua $\overline{x}$ si ha $$f(\overline{x})^{2}=f(\overline{x})\cdot f(\overline{x})=\left(\lim_{n\to\infty}f(a_{n})\right)\left(\lim_{n\to\infty}f(b_{n})\right)=\lim_{n\to\infty}f(a_{n})\cdot f(b_{n})\leq 0$$
>E quindi che $f(\overline{x})=0$.
### Proprietà dei valori intermedi
>[!note]
>Sia data una funzione continua $f\in C([a,b])$ sull'intervallo chiuso e limitato $[a,b]\subset\mathbb{R}$ e siano $$M:=\underbrace{\max f}_{[a,b]}\quad m:=\underbrace{\min f}_{[a,b]}$$
>i suoi valori massimo e minimo su $[a,b]$. Allora: $$\forall\lambda\in (m,M)\quad\exists x_{\lambda}\in[a,b]\quad |\quad f(x_{\lambda})=\lambda$$
>
>In particolare l'immagine di una funzione continua $f$ su di un intervallo chiuso $[a,b]$ è l'intervallo chiuso $[m,M]$: $$\text{Im}(f):= f([a,b]):=\set{f(x)\in\mathbb{R}:\quad x\in[a,b]}=[m,M]$$

>[!example] Dimostrazione
>Siano $x_{m}$ un punto di minimo e $x_{M}$ un punto di massimo di $f$ su $[a,b]$. Possiamo limitarci al caso $x_{m}<x_{M}$. 
>La conclusione del teorema discerne allora applicando il teorema degli zeri alla funzione continua $g\in C([x_{m},x_{M}])$ definita da $g(x):=f(x)-\lambda$ sull'intervallo chiuso $[x_{m},x_{M}]$, in quanto: $$f(x_{m})\cdot g(x_{M})=(m-\lambda)(M-\lambda)<0$$
>Poiché $m<\lambda<M$. Esiste quindi $x_{\lambda}\in(x_{m},x_{M})$ tale che $0=g(x_{\lambda})=f(x_{\lambda})-\lambda$ per cui $f(x_{\lambda})=\lambda$.





