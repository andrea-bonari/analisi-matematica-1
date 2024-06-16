### Convergenza di successione monotone e limitate in $\mathbb{R}$
>[!note]
>Sia $\set{x_{n}\in\mathbb{R}:\space n\geq1}\subset\mathbb{R}$ una successione monotona crescente (o decrescente) e superiormente (o inferiormente) limitate. Allora la successione è convergente in $\mathbb{R}$.

>[!example] Dimostrazione
>Per la completezza di $\mathbb{R}$ è sufficiente mostrare che la successione possiede la proprietà di Cauchy seguente: $$\forall\varepsilon>0\quad\exists N\geq1\quad|\quad n,m\geq N: \quad |x_{n}-x_{m}|<\varepsilon$$
>
>Supponiamo per assurdo che la successione non sia di Cauchy, quindi $$\forall\varepsilon>0\quad\forall N\geq 1\quad\exists n_{N},m_{N}\geq N\quad|\quad |x_{n_{N}}-x_{m_{N}}|\geq\varepsilon$$ Possiamo quindi supporre che $m_{N}\leq n_{N}\qquad\forall N\geq1$
>Poiché la successione è crescente abbiamo che $m_{k+1}\geq n_{k}$, e di conseguenza: $$x_{n_{k+1}}\geq\varepsilon+ x_{m_{k+1}}\geq\varepsilon+x_{n_{k}}\geq\cdots\geq k\varepsilon+x_{n_{1}}\geq k\varepsilon+x_{1}\quad\forall k\geq1$$
>Quindi: $$\lim_{k\to+\infty} x_{n_{k+1}}=+\infty$$
>Che però contraddice l'ipotesi di limitatezza superiore, e quindi la successione è necessariamente di Cauchy.
### Insiemi limitati
>[!note]
>Dato un insieme $A\subseteq\mathbb{R}$, un numero $\bar{x}\in\mathbb{R}$ è detto estremo superiore di $A$ se è il minimo dei maggioranti di $A$.
>$$x\in A\Longrightarrow x\leq \bar x$$$$\forall \varepsilon>0:\space \bar{x}-\varepsilon\text{ non è un maggiorante }\iff\exists x\in A\quad |\quad \bar{x}-\varepsilon<x$$
>Analogamente, un numero $\bar{x}\in\mathbb{R}$ è detto estremo inferiore di $A$ se è il massimo dei maggioranti di $A$.
>$$x\in A\Longrightarrow x\geq \bar x$$$$\forall \varepsilon>0:\space \bar{x}+\varepsilon\text{ non è un minorante }\iff\exists x\in A\quad |\quad \bar{x}-\varepsilon>x$$
>
>L'estremo superiore si indica con $\sup A$, mentre l'estremo inferiore si indica con $\inf A$.
>Se gli estremi appartengono all'insieme ($\sup A\in A$ o $\inf A\in A$) allora sono detti massimo o minimo e si indicano con $\max A$ e $\min A$.

Se un insieme non è limitato allora non esistono maggioranti o minoranti, e non esistono quindi $\sup A$ o $\inf A$.

>[!note] Esistenza dell'estremo superiore per insiemi superiormente limitati
>Se $A\subset\mathbb{R}$ è superiormente limitato, allora esiste $\sup(A)\in\mathbb{R}$

>[!example] Dimostrazione
>Poiché $A$ è superiormente limitato, esiste $b_{0}\in\mathbb{R}$ maggiorante di $A$: $$x\in A\Longrightarrow x\leq b_{0}$$
>Sia $a_{0}\in A$ un elemento fissato di $A$ di modo che $$[a_{0},b_{0}]\cap A\neq\emptyset$$Sia $c:=\frac{a_{0}+b_{0}}{2}$ punto medio di $[a_{0},b_{0}]$ e consideriamo i due sub-intervalli $$[a_{0},c]\text{ e } [c,b_{0}]$$
>Evidentemente in almeno uno dei due sub-intervalli vi sono elementi di $A$. Ne scegliamo uno dei due, denotandolo con $[a_{1},b_{2}]$, optando per quello di destra se entrambe le meta contengono elementi di $A$, evidentemente abbiamo che $$[a_{1},b_{1}]\cap A\neq0$$ E che $b_{1}$ è maggiorante di $A$.
>
>Iterando questo processo (detto dicotomia) otteniamo una successione crescente di intervalli $$\cdots\subset[a_{n+1},b_{n+1}]\subset[a_{n},b_{n}]\subset[a_{n},b_{n}]\subset\cdots\subset[a_{1},b_{1}]\subset[a_{0},b_{0}]$$
>Tali che $$\forall n\geq1 \qquad \forall x\in A\quad x\leq b_{n}\Longrightarrow\forall n\geq 1\quad[a_{n},b_{n}]\cap A\neq0$$
>Poiché la successione $\set{a_{n}}$ è crescente e superiormente limitata da $b_{0}$, e la successione $\set{b_{n}}$ è decrescente e inferiormente limitata da $a_{0}$ e $\lim_{n\to+\infty} b_{n}-a_{n}=\lim_{n\to+\infty} \frac{b_{0}-a_{0}}{2^{n}}=0$, e $\exists \bar{x}=\lim_{n\to+\infty}a_{n}=\lim_{n+\infty}b_{n}$, mostriamo che $\sup A=\bar{x}$. $$x\in A\qquad x\leq\bar{x}$$
>Se per assurdo non fosse tale, esisterebbe $\varepsilon>0$ per il quale $\bar{x}-\varepsilon$ sarebbe maggiorante di $A$, strettamente minore di $\bar{x}$: $$x\in A\qquad x\leq \bar{x}-\varepsilon\leq\bar{x}$$
>Tuttavia siccome $\bar{x}$ esisterebbe per $n\geq 1$, per cui $\bar{x}-\varepsilon<a_{n}<\bar{x}$, ciò contraddirebbe $[a_{n},b_{n}]\cap A\neq0$
### Proprietà di Bolzano-Weierstrass
>[!note]
>Sia $E\subset\mathbb{R}$ un insieme limitato e infinito. L'insieme dei punti di accumulazione $E'$ di $E$ è allora non vuoto: $$E'\neq\emptyset$$

>[!tip] Punti di accumulazione
>Dato un insieme $E\subseteq\mathbb{R}$, un punto $\bar{x}\in\mathbb{R}$ è detto di accumulazione per $E$ se: $$\forall\varepsilon>0\quad(E\smallsetminus\set{\bar{x}})\cap(\bar{x}-\varepsilon,\bar{x}+\varepsilon)\neq\emptyset\iff$$$$\forall\varepsilon>0\quad\exists x\in E\smallsetminus\set{\bar{x}}\quad |\quad |x-\bar{x}|<\varepsilon\iff$$$$\forall\varepsilon>0\quad \#(E\cap(\bar{x}-\varepsilon,\bar{x}+\varepsilon))=\infty$$
>L'insieme dei punti di accumulazione di $E\subseteq\mathbb{R}$ è detto insieme derivato di $E$ e si denota con $E'$.

>[!example] Dimostrazione
>Ripetiamo il processo di dicotomia per l'insieme $E$, e avremo che $$\forall n\geq1\qquad \text{\#}([a_{n},b_{n}]\cap E)=\infty$$
>In questo modo si ha che la successione $\set{a_{n}}$ è crescente e superiormente limitata da $b_{0}$, mentre $\set{b_{n}}$ è decrescente e inferiormente limitata da $a_{0}$, $\lim_{n\to+\infty} b_{n}-a_{n}=\lim_{n\to+\infty} \frac{b_{0}-a_{0}}{2^{n}}=0$, e $\exists \bar{x}=\lim_{n\to+\infty}a_{n}=\lim_{n+\infty}b_{n}$.
>Scegliendo $x_{n}\in[a_{n},b_{n}]\cap E$ con $x_{n}\neq \bar{x}$, otteniamo una successione $\set{x_{n}}\subseteq E\smallsetminus\set{\bar{x}}$ tale che $$a_{n}\leq x_{n}\leq b_{n}\qquad n\geq1$$
>Per il teorema del confronto abbiamo che $\bar{x}=\lim_{n\to\infty} x_{n}$, e quindi $\bar{x}\in E'$
