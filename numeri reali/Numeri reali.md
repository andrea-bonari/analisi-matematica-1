>[!note]
>Sia $X:\set{\text{successioni di Cauchy dei numeri razionali}}$, $\set{a_{n}},\set{b_{n}}\in \mathbb{Q}$ sono relazioni se $\lim_{n\to+\infty}(a_{n}\cdot b_{n})=0$.
>L'insieme dei numeri Reali è l'insieme quoziente fra l'insieme $X$ delle relazioni di Cauchy e $R$ che è una relazione di equivalenza, quindi devono valere riflessività, simmetricità e transitiva:
>$$\mathbb{R}=X\mathbin{ / }R$$

### Operazioni algebriche in $\mathbb{R}$

Considero $\mathbb{R}=[\set{a_{n}}_\mathbb{R}],[\set{b_{n}}_\mathbb{R}]\in X\mathbin{/}R$:
- Somma: $$[\set{a_{n}}]_\mathbb{R}+[\set{b_{n}}]_\mathbb{R}=[\set{a_{n} + b_{n}}]_\mathbb{R}$$
- Prodotto: $$[\set{a_{n}}]_\mathbb{R}\cdot [\set{b_{n}}]_\mathbb{R}=[\set{a_{n} \cdot b_{n}}]_\mathbb{R}$$

Queste operazioni in $\mathbb{R}$ hanno le stesse proprietà di quando si opera in $\mathbb{Q}$. Inoltre i numeri razionali sono ordinati (non ci sono discontinuità nella linea dei numeri, ad esempio $\sqrt2\notin\mathbb{Q},\sqrt2\in\mathbb{R}$)

### Immersione di $\mathbb{Q}$ in $\mathbb{R}$
>[!note]
>Consideriamo la funzione $j: \mathbb{Q}\to\mathbb{R}$:$$j(a)=[\set{a}_{n}]_\mathbb{R}\in \mathbb{R}$$
>È una successione costante di Cauchy. La funzione $j$ è iniettiva e biunivoca, questo significa che ad ogni $x\in\mathbb{Q}$ corrisponde un $x_{1}\in\mathbb{R}$.

### Intervalli di insiemi in $\mathbb{R}$
>[!note]
>Considerati due numeri reali $r_{1},r_{2}\in\mathbb{R}$:
>$$(r_{1},r_{2}):=\set{x\in\mathbb{R}\space|\space r_{1}<x<r_{2}}\subset\mathbb{R}$$

### Limiti in $\mathbb{R}$
>[!note]
>Considero $r_{n}\in\mathbb{R}\quad,\quad l\in\mathbb{R}$, si dirà che $r_{n}$ converge a $l$ se:
>$$\forall\varepsilon>0,\exists N(\varepsilon)\quad|\quad n\geq N(\varepsilon)\Longrightarrow r_{n}\in(l-\varepsilon,l+\varepsilon)$$
>Si mantengono le stesse proprietà dei limiti di successioni razionali.

La condizione di Cauchy per successioni di numeri reali è necessaria e sufficiente per la convergenza.