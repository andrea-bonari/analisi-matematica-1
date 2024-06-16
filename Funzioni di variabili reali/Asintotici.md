>[!note]
>Siano $f, g$ due funzioni definite e non nulle in un intorno $I(x_{0})\smallsetminus\set{x_{0}}$ con $x_{0}\in\mathbb{R}\cup{\pm\infty}$, allora si dice che $f$ è asintotica a $g$ se e solo se: $$f(x)\sim g(x)\iff \lim_{x\to x_{0}}\frac{f(x)}{g(x)}=1$$

Proprietà degli asintotici:
1. $\sim$ non è una relazione di equivalenza.
2. $f(x)\sim g(x)\Longrightarrow \lim_{x\to x_{0}} f(x)\cdot g(x)=\lim_{x\to x_{0}} f(x)$, oppure non esistono entrambi i limiti.

3. Esistono funzioni con lo stesso limite non asintotiche.
4. Se $f(x)\sim f_{1}(x)$ e $g(x)\sim g_{1}(x)$, allora anche il loro prodotto, quoziente ed elevamento ad un finito sono asintotici. NON valgono proprietà come la somma, elevamento a funzione o priorità distributiva a meno di ipotesi più stringenti.

### Asintotici notevoli
>[!tip]
>$$\begin{align*}
&\sin(ax)\sim ax&\text{per }x\to0\\
&\tan(ax)\sim ax&\text{per }x\to0\\
&1-\cos x\sim \frac{1}{2}x^{2}&\text{per }x\to0\\
&\ln(1+x)\sim x&\text{per }x\to0\\
&e^{x}-1\sim x&\text{per }x\to0\\
&\arcsin(x)\sim x&\text{per }x\to0\\
&\arctan(x)\sim x&\text{per }x\to0
\end{align*}$$

### o piccolo e gerarchia degli infiniti
>[!note] o-piccolo
>Data $f,g : (a,b)\to\mathbb{R}$, si dice che $f$ è o-piccolo di $g$ per $x\to x_{0}$ se:
>$$\lim_{x\to x_{0}} \frac{f(x)}{g(x)}=0\Longrightarrow f(x)=o(g(x))$$

>[!note] Gerarchia degli infiniti
>1. Con $x\to x_{0}$, se $f(x),g(x)\to 0\quad,\quad \frac{f(x)}{g(x)}\to 0$, si dice che $g$ è infinitesimo di ordine superiore rispetto a $f$.
>2. Con $x\to x_{0}$, se $|f(x)|,|g(x)|\to+\infty\quad,\quad \frac{g(x)}{f(x)}\to0\iff \frac{f(x)}{g(x)}\to+\infty$, si dice che $f$ è infinitesimo di ordine superiore rispetto a $g$.

