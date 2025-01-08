>[!note]
>Sia $f:(a,b)\to\mathbb{R}\quad x_{0}\in(a,b)\quad,\quad f\text{ derivabile in }(a,b)\smallsetminus\set{x_{0}}$,
>$$l=\lim_{x\to x_{0}^{-}} f'(x)=lim_{x\to x_{0}^{+}} f'(x)\in\mathbb{R}\Longrightarrow\begin{cases}
f\text{ derivabile in } x_{0} \\
f'(x_{0})=l
\end{cases}$$
>La funzione può essere definita derivabile e continua in $x_{0}$

>[!tip] Punti di discontinuità eliminabili
>Considerata $f:(a,x_{0})\cap(x_{0},b)$ continua in $x_{0}$ è definito punto di discontinuità eliminabile se $\exists l:=\lim_{x\to x_{0}}f(x)$, poiché esiste un'estensione continua di $\bar{f}$ in $(a,b):$
>$$\bar{f}(x)=\begin{cases}
f(x)&\text{ se }x\in(a,x_{0})\cap(x_{0},b) \\
l&\text{ se }x=x_{0}
\end{cases}$$

### Punti di non derivabilità
>[!note] Punti angolosi
>Un punto è detto angoloso quando il limite destro e sinistro della derivata esistono ma non coincidono (almeno una finita):
>$$\exists\lim_{x\to x_{0}^{+}}\frac{f(x)-f(x_{0})}{x-x_{0}}\neq\lim_{x\to x_{0}^{-}}\frac{f(x)-f(x_{0})}{x-x_{0}}$$
>![[Pasted image 20240508125616.png]]

>[!note] Flessi verticali
>Un punto è detto flesso verticale quando il limite destro e sinistro della tangente sono entrambi o $+\infty$ o $-\infty$
>$$\lim_{x\to x_{0}^{\pm}}\frac{f(x)-f(x_{0})}{x-x_{0}}=+\infty\quad\vee\quad \lim_{x\to x_{0}^{\pm}}\frac{f(x)-f(x_{0})}{x-x_{0}}=-\infty$$
>![[Pasted image 20240508130110.png]]

>[!note] Cuspide
>Un punto è detto cuspide se i limiti della derivata devono tendere a infinito e essere discordi:
>$$\begin{cases}
\lim_{x\to x_{0}^{\pm}}\frac{f(x)-f(x_{0})}{x-x_{0}}=\pm\infty \\
\lim_{x\to x_{0}^{\mp}}\frac{f(x)-f(x_{0})}{x-x_{0}}=\mp\infty
\end{cases}$$
![[Pasted image 20240508130301.png]]
