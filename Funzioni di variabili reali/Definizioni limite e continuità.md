>[!note] Limite di funzione
>Considerata una funzione $f: D\to\mathbb{R}\quad,\quad D\subseteq\mathbb{R}$, si dice che $f(x)$ ha limite $l\in\mathbb{R}$ in $x_{0}\in D'$ se:
>$$\forall\varepsilon>0,\exists\delta(\varepsilon)>0\quad |\begin{cases}
x\in D \\
|x-x_{0}|<\delta(\varepsilon)\\
x\neq x_{0}
\end{cases}\Longrightarrow |f(x)-l|<\varepsilon$$
>$$\lim_{x\to x_{0}}f(x)=l$$
>Ciò significa che esiste una soglia oltre la quale i punti si accumulano verso un valore reale $l$. ($D'$ è definito come insieme dei punti di accumulazione).
>Inoltre viene posto $x\neq x_{0}$ perché il limite non  comprende il punto.

>[!note] Funzione continua
>Se in più $x_{0}\in(D\cap D')\wedge l=f(x_{0})$ si dice che la funzione è continua nel punto $x_{0}$, in simboli:
>$$\begin{align*}
\forall\varepsilon>0,\exists\delta(\varepsilon)>0\quad &|\quad x\in(D\smallsetminus\set{0})\cap(x_{0}-\delta(\varepsilon),x_{0}+\delta(\varepsilon))\\
&\Longrightarrow f(x)\in(l-\varepsilon,l+\varepsilon)
\end{align*}$$

Si può considerare anche solo un intorno monolaterale di un punto, in questo caso si parla di limite destro o sinistro:
- Limite destro: $$\lim_{x\to x^{+}_{0}}f(x)=l$$$$\forall\varepsilon>0,\exists\delta(\varepsilon)>0\quad|\quad(x_{0})<x<(x_{0}+\delta(\varepsilon))\Longrightarrow|f(x)-l|<\varepsilon$$
- Limite sinistro:$$\lim_{x\to x^{-}_{0}}f(x)=l$$$$\forall\varepsilon>0,\exists\delta(\varepsilon)>0\quad|\quad(x_{0}-\delta(\varepsilon))<x<(x_{0})\Longrightarrow|f(x)-l|<\varepsilon$$

Nel caso una funzione sia continua solo da destra o sinistra possiamo scrivere:
$$\lim_{x\to x^{\pm}_{0}}f(x)=l=f(x_{0})$$
