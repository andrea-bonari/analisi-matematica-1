### Convergenza di successione monotone e limitate in $\mathbb{R}$
>[!note]
>Sia $\set{x_{n}\in\mathbb{R}:\space n\geq1}\subset\mathbb{R}$ una successione monotona crescente (o decrescente) e superiormente (o inferiormente) limitate. Allora la successione è convergente in $\mathbb{R}$.

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

### Proprietà di Bolzano-Weierstrass
>[!note]
>Sia $E\subset\mathbb{R}$ un insieme limitato e infinito. L'insieme dei punti di accumulazione $E'$ di $E$ è allora non vuoto: $$E'\neq\emptyset$$

>[!tip] Punti di accumulazione
>Dato un insieme $E\subseteq\mathbb{R}$, un punto $\bar{x}\in\mathbb{R}$ è detto di accumulazione per $E$ se: $$\forall\varepsilon>0\quad(E\setminus\set{\bar{x}})\cap(\bar{x}-\varepsilon,\bar{x}+\varepsilon)\neq0\iff$$$$\forall\varepsilon>0\quad\exists x\in E\setminus\set{\bar{x}}\quad |\quad |x-\bar{x}|<\varepsilon\iff$$$$\forall\varepsilon>0\quad \#(E\cap(\bar{x}-\varepsilon,\bar{x}+\varepsilon))$$
>L'insieme dei punti di accumulazione di $E\subseteq\mathbb{R}$ è detto insieme derivato di $E$ e si denota con $E'$.

