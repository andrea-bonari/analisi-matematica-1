>[!note]
>Sia data una successione $\set{a_{n}}^{\infty}_{n=0}\subset\mathbb{R}$, definiamo la successione $s_{N}$ delle somme parziali: $$s_{N}:=\sum\limits^{N}_{n=0}a_{n}\iff N\geq 0$$

Notiamo come la somma delle serie coincide con l'integrale se la serie è definitivamente positiva:
$$\sum\limits^\infty_{n=0}a_{n}=\int^{+\infty}_{0}f(x)\text{ d}x$$

### Carattere della serie
- Se la successione $\set{s_{n}}^{\infty}_{n=0}$ ammette limite finito, si dice che la serie definita dai $\set{a_{n}}^{\infty}_{n=0}$ converge.
- Se la successione $\set{s_{n}}^{\infty}_{n=0}$ converge a $\pm\infty$, si dice che la serie definita dai $\set{a_{n}}^{\infty}_{n=0}$ diverge.
- Se la successione $\set{s_{n}}^{\infty}_{n=0}$ non ammette limite, si dice che la serie è indeterminata.

>[!tip] Osservazione sul carattere delle serie
>Il carattere di una serie non viene alterato se si trascurano un numero finito di termini, ovvero la serie $\sum\limits^{\infty}_{n=n_{0}}$ ha lo stesso carattere di $\sum\limits^{\infty}_{n=n_{0}+k}$.

### Proprietà delle serie

1. Linearità $$\sum\limits_{n}(\alpha\cdot a_{n}+\beta \cdot b_{n})=\alpha\sum\limits_{n}a_{n}+\beta\sum\limits_{n}b_{n}\qquad\alpha,\beta\in\mathbb{R}$$
Se anche una delle due serie non converge allora la somma delle due serie non convergerà.

2. Confronto
Se $0\leq a_{n}\leq b_{n}\quad\forall n$ allora:
- Se $\sum\limits_{n}b_{n}$ converge, anche $\sum\limits_{n}a_{n}$ converge: $$\sum\limits_{n}a_{n}\leq\sum\limits_{n}b_{n}$$
- Se $\sum\limits_{n}a_{n}$ diverge a $\pm\infty$, allora anche la serie $\sum\limits_{n}b_{n}$ diverge a $\pm\infty$, poiché le somme parziali sono sempre maggiori.

3. Confronto asintotico
Sia $0\leq a_{n}\quad,\quad0\leq b_{n}\quad,\quad a_{n}\sim b_{n}\text{ per }n\to+\infty$, allora:
- $\sum\limits_{n}a_{n}\text{ converge }\iff\sum\limits_{n}b_{n}\text{ converge }$
- $\sum\limits_{n}a_{n}\text{ diverge }\iff\sum\limits_{n}b_{n}\text{ diverge }$

>[!example] Dimostrazione
>Siccome $a_{n}\sim b_{n}\Longrightarrow\lim_{n} \frac{a_{n}}{b_{n}}=1$:
>$$\forall\varepsilon>0\quad\exists N\space |\space n\geq N\space|\quad \left| \frac{a_{n}}{b_{n}}-1  \right|<\varepsilon \Longrightarrow$$
>$$\Longrightarrow 1-\varepsilon< \frac{a_{n}}{b_{n}}<1+\varepsilon\Longrightarrow (1-\varepsilon)b_{n}<a_{n}<(1+\varepsilon)b_{n}\qquad n\geq N$$
>Si conclude la dimostrazione per il criterio del confronto.

4. Condizione necessaria per la convergenza
La condizione necessaria affinché la serie $\sum\limits_{n}a_{n}$ converga è: $$\lim_{n}a_{n}=0$$
Quindi $$\lim_{n}a_{n}\neq0\iff \sum\limits_{n}a_{n} \text{ non converge }$$
### Serie particolari

>[!note] Serie geometrica
>Sia $q$ un numero reale. Si dice serie geometrica di ragione $q$ la serie $$\sum\limits^{+\infty}_{n=0}q^{n}$$
>Se $|q|<1$, la serie geometrica converge ed ha per somma $\frac{1}{1-q}$
>Se $q\leq-1$, la serie geometrica è irregolare
>Se $q\geq1$, la serie geometrica diverge positivamente

>[!note] Serie armonica generalizzata
>Sia $\alpha$ un numero reale. Si dice serie armonica generalizzata la serie $$\sum\limits^{+\infty}_{n=0} \frac{1}{n^{\alpha}}$$
>Se $\alpha>1$ converge
>Se $\alpha\leq 1$ diverge positivamente

>[!note] Serie armonica a segni alterni
>Sia $\alpha$ un numero reale positivo. Si dice serie armonica a segno alterno la serie $$\sum\limits^{+\infty}_{n=1} (-1)^{n}\frac{1}{n^{\alpha}}$$
>Se $\alpha>1$ converge assolutamente
>Se $0<\alpha\leq1$ converge semplicemente

>[!note] Serie armonica modificata
>Sia $\alpha$ un qualsiasi numero reale. Si dice serie armonica modificata la serie $$\sum\limits^{+\infty}_{n=2}\frac{1}{n^{\alpha}(\log(n))^{\beta}}$$
>Se $\alpha>1$ e $\forall\beta$, converge
>Se $\alpha=1$ e $\beta>1$ converge
>Se $\alpha=1$ e $\beta\leq1$ diverge positivamente
>Se $\alpha<1$ diverge positivamente