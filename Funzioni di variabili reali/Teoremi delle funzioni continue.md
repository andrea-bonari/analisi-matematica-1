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
>[!example] Dimostrazione
>Dimostrazione per induzione e seconda proprietà (prodotto)

7. Continuità dei polinomi: $$P_{n}(x)=\sum\limits_{i=0}^{n}c_{n}x^{n}=(c_{0}+c_{1}x^{1}+c_{2}x^{2}+\cdots+ c_{n}x^{n})\in C$$
>[!example] Dimostrazione
>Dimostrazione per induzione e prima proprietà (somma)

8. Continuità di funzioni razionali: $$R(x)= \frac{P(x)}{Q(x)}\quad D(R):=\set{x\in\mathbb{R}\text{ }|\space Q(x)\neq0}$$$$P,Q\in C(R)\Longrightarrow R= \frac{p}{q}$$
>[!example] Dimostrazione
>Dimostrazione per induzione e terza proprietà (quoziente)

9. Continuità del seno e del coseno:
$$\sin,\cos\in C(\mathbb{R})$$

### Teorema di Weierstrass
>[!note]
>Sia $f\in C([a,b])$ una funzione continua sull'intervallo chiuso e limitato $[a,b]\subset\mathbb{R}$. Esistono allora il massimo e minimo globali di $f$ su $[a,b]$:
>$$\exists x_{m},x_{M}\in[a,b]\quad |\quad x\in[a,b]\Longrightarrow f(x_{m})\leq f(x)\leq f(x_{M})$$
>In altre parole, $M:=f(x_{M})$ è il valore massimo e $m:=f(x_{m})$ è il valore minimo di $f$ su $[a,b].$

>[!example] Dimostrazione
>Ci limiteremo a provare l'esistenza del massimo. Sia $M:=\sup\text{Im}(f)\in\mathbb{R}\cup\set{+\infty}$ l'estremo superiore dell'immagine della funzione. Per le proprietà dell'estremo superiore, esiste una successione $\set{y_{n}}\subset\text{Im}(f)$ tale che $\lim_{n}y_{n}=M$. Sia quindi $\set{x_{n}}\subset[a,b]$ una successione tale che $f(x_{n})=y_{n}$ per la quale evidentemente si ha $$\lim_{n}f(x_{n})=\lim_{n}y_{n}=M$$
>Se per un certo $n$ si ha $y_{n}=M$, allora $M\in\text{Im}(f)$ è un valore massimo per la funzione e $x_{n}\in[a,b]$ è il punto di massimo. Se invece $y_{n}\neq M$ per ogni $n$, allora la successione $\set{x_{n}}$ è un insieme limitato e infinito e, per il teorema di Bolzano-Weierstrass, ammette almeno un punto di accumulazione che denotiamo con $x_{M}\in[a,b]$. Esisterà quindi almeno una sotto-successione $\set{x_{n_{k}}}\subseteq\set{x_{n}}$ convergente a $x_{M}$. Poiché $f$ è continua$$M=\lim_{n\to\infty}y_{n}=\lim_{n\to\infty}f(x_{n})=\lim_{k\to\infty}f(x_{n_{k}})=f(x_{M})\in\mathbb{R}$$
>Questo dimostra che $M:=\sup\text{Im}(f)\in\mathbb{R}$ è finito e che appartiene all'immagine $\text{Im}(f)$. $M$ è quindi un valore massimo di $\text{Im}(f)$, assunto da $f$ nel punto $x_{M}\in[a,b]$
### Teorema degli zeri
>[!note]
>Sia data una funzione continua $f\in C([a,b])$ sull'intervallo chiuso e limitato $[a,b]\subset\mathbb{R}$. Se $$f(a)\cdot f(b)<0\quad\text{cioè}\quad\text{sgn}(f(a))\neq\text{sgn}(f(b))$$
allora $$\exists x_{0}\in(a,b)\quad |\quad f(x_{0})=0$$

>[!example] Dimostrazione
>Dividiamo l'intervallo $(a,b)$ per dicotomia tale che ogni sotto intervallo ha condizione $f(a_{n})\cdot f(b_{n})<0$. Conoscendo la costruzione delle successioni $\set{a_{n}}$ e $\set{b_{n}}$, sapendo che $$\lim_{n\to+\infty}b_{n}-a_{n}=\lim_{n\to+\infty}\frac{b_{0}-a_{0}}{2^{n}}=0$$
>e per il teorema delle successioni monotone limitate $$\exists x_{0}=\lim_{n\to+\infty}a_{n}=\lim_{n\to+\infty}b_{n}\in\mathbb{R}$$
>Per il teorema della permanenza del segno e poiché $f$ è continua in $x_{0}$ si ha $$[f(x_{0})]^{2}=\left(\lim_{n\to+\infty}f(a_{n})\right)\cdot\left(\lim_{n\to+\infty} f(b_{n})\right)=\lim_{n\to+\infty}f(a_{n})\cdot f(b_{n})\leq0$$
>E quindi $f(x_{0})=0$
### Proprietà dei valori intermedi
>[!note]
>Sia data una funzione continua $f\in C([a,b])$ sull'intervallo chiuso e limitato $[a,b]\subset\mathbb{R}$ e siano $$M:=\underbrace{\max f}_{[a,b]}\quad m:=\underbrace{\min f}_{[a,b]}$$
>i suoi valori massimo e minimo su $[a,b]$. Allora: $$\forall\lambda\in (m,M)\quad\exists x_{\lambda}\in[a,b]\quad |\quad f(x_{\lambda})=\lambda$$
>
>In particolare l'immagine di una funzione continua $f$ su di un intervallo chiuso $[a,b]$ è l'intervallo chiuso $[m,M]$: $$\text{Im}(f):= f([a,b]):=\set{f(x)\in\mathbb{R}:\quad x\in[a,b]}=[m,M]$$

>[!example] Dimostrazione
>Siano $x_{m}$ un punto di minimo e $x_{M}$ un punto di massimo di $f$ su $[a,b]$. Possiamo limitarci al caso $x_{m}<x_{M}$. La conclusione del teorema discerne allora applicando il teorema degli zeri alla funzione continua $g\in C([x_{m},x_{M}])$ definita da $g(x):=f(x)-\lambda$ sull'intervallo chiuso $[x_{m},x_{M}]$.



