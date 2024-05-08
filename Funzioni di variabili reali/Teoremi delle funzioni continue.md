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

### Teorema degli zeri
>[!note]
>Sia data una funzione continua $f\in C([a,b])$ sull'intervallo chiuso e limitato $[a,b]\subset\mathbb{R}$. Se $$f(a)\cdot f(b)<0\quad\text{cioè}\quad\text{sgn}(f(a))\neq\text{sgn}(f(b))$$
allora $$\exists x_{0}\in(a,b)\quad |\quad f(x_{0})=0$$

### Proprietà dei valori intermedi
>[!note]
>Sia data una funzione continua $f\in C([a,b])$ sull'intervallo chiuso e limitato $[a,b]\subset\mathbb{R}$ e siano $$M:=\underbrace{\max f}_{[a,b]}\quad m:=\underbrace{\min f}_{[a,b]}$$
>i suoi valori massimo e minimo su $[a,b]$. Allora: $$\forall\lambda\in (m,M)\quad\exists x_{\lambda}\in[a,b]\quad |\quad f(x_{\lambda})=\lambda$$
>
>In particolare l'immagine di una funzione continua $f$ su di un intervallo chiuso $[a,b]$ è l'intervallo chiuso $[m,M]$: $$\text{Im}(f):= f([a,b]):=\set{f(x)\in\mathbb{R}:\quad x\in[a,b]}=[m,M]$$

