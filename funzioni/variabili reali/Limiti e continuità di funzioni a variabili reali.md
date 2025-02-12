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

Si può considerare anche solo un intorno monolaterale di un punto, in questo caso si parla di limite destro o sinistro:
- Limite destro: $$\begin{align*}
&\lim_{x\to x^{+}_{0}}f(x)=l\\
&\forall\varepsilon>0,\exists\delta(\varepsilon)>0\quad|\quad(x_{0})<x<(x_{0}+\delta(\varepsilon))\Longrightarrow|f(x)-l|<\varepsilon
\end{align*}$$
- Limite sinistro: $$\begin{align*}
&\lim_{x\to x^{-}_{0}}f(x)=l\\
&\forall\varepsilon>0,\exists\delta(\varepsilon)>0\quad|\quad(x_{0}-\delta(\varepsilon))<x<(x_{0})\Longrightarrow|f(x)-l|<\varepsilon
\end{align*}$$
Nel caso una funzione sia continua solo da destra o sinistra possiamo scrivere:
$$\lim_{x\to x^{\pm}_{0}}f(x)=l=f(x_{0})$$
### Proprietà dei limiti
1. Unicità limite: $$\text{se }\exists\lim_{x\to x_{0}}f(x)=l\text{ allora è unico}$$
2. Intorno: $$\text{se }\exists\lim_{x\to x_{0}}f(x)\in\mathbb{R}\Longrightarrow x\in((x_{0}-\delta(\varepsilon),x_{0}+\delta(\varepsilon))\cap D\smallsetminus\set{x_{0}})$$
3. Somma: $$\lim_{x\to x_{0}}(f(x)+g(x))=\lim_{x\to x_{0}}f(x)+\lim_{x\to x_{0}}g(x)$$
4. Prodotto: $$\lim_{x\to x_{0}}(f(x)\cdot g(x))=\lim_{x\to x_{0}}f(x)\cdot \lim_{x\to x_{0}}g(x)$$
5. Quoziente: $$\lim_{x\to x_{0}} \frac{f(x)}{g(x)}= \frac{\lim_{x\to x_{0}} f(x)}{\lim_{x\to x_{0}} g(x)}$$
6. Permanenza del segno: $$\begin{cases}
0\leq f(x)\forall x\in D \\
l:=\lim_{x\to x_{0}}f(x)
\end{cases}\Longrightarrow l\geq0$$
Se una funzione è positiva in tutto il suo dominio, allora il limite della funzione in qualsiasi punto sarà positiva, e viceversa.
7. Monotonia
$$\begin{align*}&\text{se }f(x)\leq g(x)\leq h(x)\quad,\quad x\in((x_{0}-\delta(\varepsilon),(x_{0}+\delta(\varepsilon))\\&\text{allora } \lim_{x\to x_{0}}f(x)\leq \lim_{x\to x_{0}}g(x)\leq \lim_{x\to x_{0}}h(x)
\end{align*}$$

### Continuità della funzione composta
>[!note]
>Considero $f: D(f)\to\mathbb{R}$ e $g: D(g)\to\mathbb{R}$. Siam $\text{Im}(f)\subseteq D(g)$, allora: 
>$$g\circ f:D(f)\to\mathbb{R}\quad,\quad g\circ f:=g(f(x))$$
>Supponendo che $x_{0}\in D(f)$ sia punto di accumulazione, allora:
>$$\exists y_{0}:=f(x)\quad\exists l:=\begin{cases}
\lim_{x\to x_{0}} g(y) \\
y=y_{0}
\end{cases}\Longrightarrow \exists\lim_{x\to x_{0}} g(f(x))=l$$

>[!example] Dimostrazione
>$$\begin{cases}
>\lim_{y\to y_{0}}g(y)&= g(y_{0})\\
>\lim_{x\to x_{0}}f(x)&= f(x_{0})=y_{0}
>\end{cases}\Longrightarrow \exists\lim_{x\to x_{0}} g(f(x))=g(y_{0})$$
>Passando alla definizione formale dei due limiti: $$\begin{align*}
>\forall \varepsilon>0\quad\exists\delta(\varepsilon)>0\quad&|\quad|y-y_{0}|<\delta(\varepsilon)\Longrightarrow |g(y)-g(y_{0})|<\varepsilon\\
>\forall \varepsilon'>0\quad\exists\delta'(\varepsilon')>0\quad&|\quad|y-y_{0}|<\delta'(\varepsilon')\Longrightarrow |g(y)-g(y_{0})|<\varepsilon'\\
>\end{align*}$$
>Scegliendo $\varepsilon':=\delta(\varepsilon)$, otterremo: $$\begin{align*}
|x-x_{0}|<\delta'(\varepsilon)&\Longrightarrow |f(x)-f(x_{0})|<\varepsilon'=\delta(\varepsilon)\\
&\Longrightarrow\varepsilon>|g(f(x))-g(f(x_{0}))|=|(g\circ f)(x)-g(y_{0})|
\end{align*}$$

### Continuità della funzione inversa
>[!note]
>Considero una funzione $f:(a,b)\to\mathbb{R}$ iniettiva e continua in $x_{0}\subset(a,b)$, possiamo considerare la funzione inversa $f^{-1}: \text{Im}(f)\to D(f)$:
>$$\begin{cases}
f^{-1}(f(x))=x \\
f(f^{-1}(y))=y
\end{cases}\Longrightarrow f^{-1}\text{ continua in } y_{0}:= f(x_{0})$$
>Considerata una funzione continua $f(x)$, se esiste la sua funzione inversa $f^{-1}(x)$, allora anch'essa è una funzione continua.
### Limiti notevoli
>[!tip] Funzioni goniometriche
>$$\begin{align*}
&\lim_{x\to0}\frac{\sin x}{x}=1&&
\lim_{x\to0}\frac{1-\cos x}{x}=0\\
&\lim_{x\to0}\frac{1-\cos x}{x^{2}}= \frac{1}{2}&&
\lim_{x\to0} \frac{\sin mx}{\sin nx}= \frac{m}{n}\\
&\lim_{x\to0}\frac{\tan x}{x}=1&&
\lim_{x\to0}\frac{\arcsin x}{x}=1\\
&\lim_{x\to0}\frac{\arctan x}{x}=1&&
\lim_{x\to0}\frac{(\arccos x)^{2}}{1-x}=2
\end{align*}$$

>[!tip] Funzioni esponenziali e logaritmiche
>$$\begin{align*}
&\lim_{x\to\infty} \left(1+ \frac{1}{x}\right)^{x}=e&&\lim_{x\to0} (1+x)^{\frac{1}{x}}=e\\
&\lim_{x\to0}\frac{\log_{a}(1+x)}{x}=\log_{a}e&&\lim_{x\to0}\frac{\ln(1+x)}{x}=1\\
&\lim_{x\to0}\frac{a^{x}-1}{x}=\ln a&&\lim_{x\to0}\frac{e^{x}-1}{x}=1\\
&\lim_{x\to0}\frac{(1+x)^{k}-1}{x}=k&&\lim_{x\to\infty} \frac{x^{n}}{a^{x}}=0\quad (a>1)\\
&\lim_{x\to\infty}\frac{a^{n}}{n!}=0&&\lim_{x\to\infty}\frac{1}{1+a^{x}}=\begin{cases}
1\text{ se } a<1\\
\frac{1}{2}\text{ se } a=1\\
0\text{ se } a>1
\end{cases}
\end{align*}$$
