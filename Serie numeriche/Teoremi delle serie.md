### Teorema del confronto integrale
>[!note]
>Sia data una serie $\sum\limits_{n}a_{n}$ a termini positivi e una funzione $f:[0,+\infty)\to[0,+\infty)$ integrabile e decrescente. Se $a_{n}\sim f(n)$ per $n\to+\infty$ allora $\sum\limits_{n}a_{n}$ converge.

### Criterio della radice
>[!note]
>Sia $0\leq a_{n}$ e supponiamo che $$\exists l:=\lim_{n}\sqrt[n]{a_{n}}$$Allora:
>1. Se $0\leq l <1$ la serie $\sum\limits_{n}a_{n}$ converge.
>2. Se $l>1$ la serie $\sum\limits_{n} a_{n}$ diverge.
>3. Se $l=1$ bisogna ricondursi a dei casi notevoli.

>[!example] Dimostrazione
>Dall'ipotesi segue che: $$\forall\varepsilon>0\quad\exists N\space|\space n\geq N\Longrightarrow|\sqrt[n]{a_{n}}-l|<\varepsilon\quad\Longrightarrow\quad l-\varepsilon<\sqrt[n]a_{n}<l+\varepsilon$$
>Se $0<\varepsilon<l$ eleviamo alla $n$: 
>$$(l-\varepsilon)^{n}<a_{n}<(l+\varepsilon)^{n}\qquad n\geq N$$
>###### Caso 1
>Se $l < 1$, e scegliendo quindi $\varepsilon\quad |\quad l+\varepsilon<1$: $$\sum\limits_{n\geq N}(l+\varepsilon)^{n}\text{ converge }\iff\sum\limits_{n}a_{n}\text{ converge }$$
>###### Caso 2
>Se $l>1$,  e scegliendo quindi $\varepsilon\quad |\quad l-\varepsilon>1$: $$\sum\limits_{n\geq N}(l-\varepsilon)^{n}\text{ diverge }\iff\sum\limits_{n}a_{n}\text{ diverge}$$
>
### Criterio del rapporto
>[!note]
>Sia $0\leq a_{n}$ e supponiamo che: $$\exists l:=\lim_{n}\frac{a_{n+1}}{a_{n}}\in[0,+\infty)$$
>Allora:
>1. Se $0\leq l <1$ la serie $\sum\limits_{n}a_{n}$ converge
>2. Se $l>1$ la serie $\sum\limits_{n}a_{n}$ diverge
>3. Se $l=0$ ci si deve ricondurre a casi notevoli.

>[!example] Dimostrazione
>Dall'ipotesi segue che:
>$$\forall\varepsilon>0\quad\exists N\space |\space n\geq N\Longrightarrow \left|\frac{a_{n+1}}{a_{n}}-l  \right|<\varepsilon\Longrightarrow l-\varepsilon< \frac{a_{n+1}}{a_{n}}<l+\varepsilon$$
>Se $0<\varepsilon<l$, moltiplichiamo per $a_{n}$: $$(l-\varepsilon)a_{n}<a_{n+1}<(l+\varepsilon)a_{n}\qquad n\geq N$$
>###### Caso 1
>Se $l<1$, scegliendo $0<\varepsilon\space |\space l+\varepsilon<1$:
>$$a_{n+1}<(l+\varepsilon)a_{n}<(l+\varepsilon)(l+\varepsilon)a_{n}<\cdots<(l+\varepsilon)^{n+1}a_{n}$$
>Siccome la serie $\sum\limits_{n\geq N}(l+\varepsilon)^{n}$ è convergente, per il criterio del confronto $\sum\limits_{n}a_{n}$ è convergente.
>###### Caso 2
>Se $l>1$, scegliendo $\varepsilon>0\space |\space l-\varepsilon>1$:
>$$a_{n+1}>(l-\varepsilon)a_{n}>(l-\varepsilon)(l-\varepsilon)a_{n}>\cdots>(l-\varepsilon)^{n+1}a_{n}$$
>Siccome la serie $\sum\limits_{n\geq N}(l+\varepsilon)^{n}$ è divergente, per il criterio del confronto $\sum\limits_{n}a_{n}$ è divergente.
### Teorema della convergenza assoluta
>[!note]
>La serie $\sum\limits_{n}a_{n}$ è assolutamente convergente se la serie $\sum\limits_{n}|a_{n}|$ converge: $$\sum\limits_{n}a_{n}\text{ coverge }\iff\mathbb{R}\ni\sum\limits_{n}|a_{n}|<+\infty$$
>Se $\sum\limits_{n}a_{n}$ converge assolutamente, allora converge semplicemente a: $$\bigg|\sum\limits_{n}a_{n}\bigg|\leq\sum\limits_{n}|a_{n}|$$

### Criterio di Leibniz
>[!note]
>Consideriamo la serie $\sum\limits^\infty_{n=0}(-1)^{n}a_{n}$ dove:
>1. La serie ha termini di segno alterno: $a_{n}\geq0$
>2. Condizione necessaria per la convergenza della serie $\lim_{n\to+\infty}a_{n}=0$
>3. È definitivamente crescente $\set{a_{n}}^{\infty}_{n=0}$, cioè: $$\exists n_{0}\geq0\quad |\quad n\geq n_{0}\Longrightarrow a_{n}\geq a_{n+1}$$
>
>Allora la serie $\sum\limits^{\infty}_{n=0}(-1)^{n}a_{n}$ converge semplicemente.
