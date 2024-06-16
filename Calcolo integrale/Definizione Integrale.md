>[!note]
>L'integrale rappresenta il valore dell'area sottesa dal grafico della funzione in un dato intervallo.

### Partizione di intervallo
>[!note]
>Sia $I=[a,b]\subset\mathbb{R}$, una partizione $P:=\set{I_{k}}^{n}_{k=1}$ è una famiglia finita di intervalli $I_{k}$ tutti contenuti ($I_{k}\subset I$) tali che $I=\bigcup_{k=1}^{n}$ con $n\neq j$ contiene al più un punto.

Ciò significa che $I_{k}$ e $I_{j}$ o sono disgiunti o si "toccano" solo in un punto.

### Integrale inferiore e superiore
>[!note] Somme inferiori
>Sia $[a,b]\to\mathbb{R}$ limitata, sia $P=\set{I_{k}}_{k=1}^{n}\in\mathcal{P}(I)$, la somma inferiore è definita come l'area del più piccolo rettangolo sotto a $G(f)$ su $I_{k}$: $$s(f,P):=\sum\limits_{k=1}^{n}|I_{k}|\cdot\begin{pmatrix}\inf(f)\\ I_{k}\end{pmatrix}$$

>[!note] Somme superiori
>Sia $[a,b]\to\mathbb{R}$ limitata, sia $P=\set{I_{k}}^{n}_{k=1}\in\mathcal{P}(I)$, la somma superiore è: $$S(f,P):=\sum\limits_{k=1}^{n}|I_{k}|\cdot\begin{pmatrix}\sup(f)\\I_{k}\end{pmatrix}$$

Si deduce che: $$-\infty<s(f,P)\leq S(f,P)<+\infty$$
Di conseguenza:
>[!note] Integrale inferiore e superiore di $f$ in $I$
>L'integrale inferiore è la migliore approssimazione per difetto dall'alto: $$\underline{I}(f):=\sup(\set{s(f,P)\quad|\quad P\in\mathcal{P}(I)})$$
>Viceversa, l'integrale superiore è la migliore approssimazione per eccesso dal basso: $$\overline{I}(f):=\inf(\set{S(f,P)\quad|\quad P\in\mathcal{P}(I)})$$
### Integrale di Riemann
>[!note]
>Se l'integrale inferiore coincide con quello superiore, ovvero $\underline{I}(f)= \overline{I}(f)$, allora si dice che $f$ è integrabile (secondo Riemann) su $I$ e il valore è detto integrale di $f$ su $I$. Si scrive come: $$\int_{I}f(x)\text{ d}x=\int_{I}f=\int^{b}_{a}f(x)\text{ d}x$$
>Ed è l'area $|A_{f}|$ del sottografico $A_{f}$ di $f$ su $I=[a,b]$.

>[!example]
>Non è integrabile la funzione di Dirichlet che assume valore $0$ se l'argomento è razionale, altrimenti se è irrazionale $1$: $$f(x)=\begin{cases}
0\qquad x\in[0,1]\cap\mathbb{Q} \\
1\qquad x\in[0,1]\cap\mathbb{Q}^{C}
\end{cases}$$
>Si ha che $\underline{I}(f)=0\neq\overline{I}(f)=1$, e quindi la funzione non è integrabile.


