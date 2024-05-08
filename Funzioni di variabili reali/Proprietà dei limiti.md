1. Unicità limite: $$\text{se }\exists\lim_{x\to x_{0}}f(x)=l\text{ allora è unico}$$
2. Intorno: $$\text{se }\exists\lim_{x\to x_{0}}f(x)\in\mathbb{R}\Longrightarrow x\in((x_{0}-\delta(\varepsilon),x_{0}+\delta(\varepsilon))\cap D\setminus\set{x_{0}})$$
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

### Limiti di funzione composta
>[!note]
>Considero $f: D(f)\to\mathbb{R}$ e $g: D(g)\to\mathbb{R}$. Siam $\text{Im}(f)\subseteq D(g)$, allora: 
>$$g\circ f:D(f)\to\mathbb{R}\quad,\quad g\circ f:=g(f(x))$$
>Supponendo che $x_{0}\in D(f)$ sia punto di accumulazione, allora:
>$$\exists y_{0}:=f(x)\quad\exists l:=\begin{cases}
\lim_{x\to x_{0}} g(y) \\
y=y_{0}
\end{cases}\Longrightarrow \exists\lim_{x\to x_{0}} g(f(x))=l$$

>[!example] Dimostrazione
>Considero $|g(f(x))-l|\Longrightarrow \lim_{x\to x_{0}} f(y)=l$:
>$$\forall\varepsilon>0\quad\exists\delta(\varepsilon)>0\quad|\quad(y-y_{0})<\delta(\varepsilon)\Longrightarrow \varepsilon>|g(y)-l|$$
>Scelgo $\varepsilon':=\delta(\varepsilon)\Longrightarrow\exists\delta'(\varepsilon')>0\quad |\quad |x-x_{0}|<\delta'(\varepsilon')$.
>Di conseguenza si ha che $|f(x)-y_{0}|>\varepsilon':=\delta(\varepsilon)$.
>
>Quindi $|f(x)-x_{0}|<\varepsilon'\iff \varepsilon> |g(f(x))|$

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

