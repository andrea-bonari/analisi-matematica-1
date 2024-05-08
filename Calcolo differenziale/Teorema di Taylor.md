>[!note] Teorema di Taylor con resto di Peano
>Sia $f:(a,b)\to\mathbb{R}$ derivabile $n-\text{volte}$ in $x_{0}\in(a,b)$. Definiamo il suo polinomio di Taylor di ordine $n$ in $x_{0}$ (con $x\in\mathbb{R}$) come:
>$$\begin{align*}
>&T^{f}_{n,x_{0}}(x):=\sum\limits_{k=0}^{n}\frac{f^{(k)}(x_{0})}{k!}\cdot(x-x_{0})^{k}\\
>&=f(x_{0})+f'(x_{0})(x-x_{0})+ \frac{1}{2}f^{(2)}(x_{0})(x-x_{0})^{2}+\cdots+\frac{f^{(n)}(x_{0})}{n!}(x->x_{0})^{n}
>\end{align*}$$
>Allora esiste una funzione resto $R^{f}_{n,x_{0}}(x):(a,b)\to\mathbb{R}$di ordine $n$ in $x_{0}$ tale che: >$$f(x)=T^{f}_{n,x_{0}}(x)+R^{f}_{n,x_{0}}(x)\qquad >x\in(a,b)$$
>Il resto è di infinitesimo di ordine maggiore di $n$ per $x\geq x_{0}$:
>$$\lim_{x\to x_{0}}\frac{T^{f}_{n,x_{0}}(x)-R^{f}_{n,x_{0}}(x)}{(x-x_{0})^{n}}=0$$
>Quindi:
>$$R^{f}_{n,x_{0}}(x)=o((x-x_{0})^{n})\quad\text{per }
>x\to x_{0}$$

### Teorema di Taylor con resto di Lagrange
>[!bug] DA FARE

### Formula di Stirling
>[!note]
>$$n!\sim\sqrt{2\pi\cdot n}\cdot\left(\frac{n}{e}\right)^{n}\quad\text{ con }n\to+\infty$$

### Sviluppi di Mc Laurin
$$\begin{align*}
e^{x}&= 1+x+ \frac{x^{2}}{2}+ \frac{x^{3}}{6}+\cdots+ \frac{x^{n}}{n!}+o(x^{n})\\
\sin x&= x- \frac{x^{3}}{6}+ \frac{x^{5}}{5!}+\cdots+(-1)^{n}\frac{x^{2n+1}}{(2n+1)!}+o(x^{2n+2})\\
\cos x&= 1- \frac{x^{2}}{2}+ \frac{x^{4}}{4}+\cdots+(-1)^{n}\frac{x^{2n}}{(2n)!}+o(x^{2n+1})\\
\tan x&= x+ \frac{x^{3}}{3}+ \frac{2}{15}x^{5}+ \frac{17}{315}x^{7}+ \frac{62}{2835}x^{9}+o(x^{10})\\
\sinh x&= x+ \frac{x^{3}}{6}+ \frac{x^{5}}{5!}+\cdots+\frac{x^{2n+1}}{(2n+1)!}+o(x^{2n+2})\\
\cosh x&= 1+ \frac{x^{2}}{2}+ \frac{x^{4}}{4}+\cdots+\frac{x^{2n}}{(2n)!}+o(x^{2n+1})\\
\tanh x&= x- \frac{x^{3}}{3}+ \frac{2}{15}x^{5}- \frac{17}{315}x^{7}+ \frac{62}{2835}x^{9}+o(x^{10})\\
\frac{1}{1-x}&= 1+x+x^{2}+x^{3}+\cdots+x^{n}+o(x^{n})\\
\log(1+x)&= x- \frac{x^{2}}{2}+ \frac{x^{3}}{3}+\cdots+(-1)^{n+1}\frac{x^{n}}{n}+o(x^{n})\\
\arctan x&= x- \frac{x^{3}}{3}+ \frac{x^{5}}{5}+\cdots+ (-1)^{n}\frac{x^{2n+1}}{2n+1}+o(x^{2n+2})\\
\text{arctanh} x&= x+ \frac{x^{3}}{3}+ \frac{x^{5}}{5}+\cdots+ \frac{x^{2n+1}}{2n+1}+o(x^{2n+2})\\
(1+x)^{a}&= 1+ax+\frac{a(a-1)}{2}x^{2}+\frac{a(a-1)(a-2)}{6}x^{3}+\cdots\\
&\space+\begin{pmatrix}a\\n\end{pmatrix}x^{n}+o(x^{n})\\
&\quad\text{con }\begin{pmatrix}a\\n\end{pmatrix}=\frac{a(a-1)(a-2)(\cdots(a-n+1))}{n!}
\end{align*}$$
