### Convergenza di successione monotone e limitate in $\mathbb{R}$
>[!note]
>Sia $\set{x_{n}\in\mathbb{R}:\space n\geq1}\subset\mathbb{R}$ una successione monotona crescente, cioè: $$x_{n}\leq x_{n+1}\quad\forall n\in\mathbb{N}$$ superiormente limitate: $$\exists M\in\mathbb{R}\qquad|\quad x_{n}\leq M\quad\forall n\in \mathbb{N}$$Allora la successione è convergente in $\mathbb{R}$: $$\exists \lim_{n\to+\infty} x_{n}\in\mathbb{R}$$

>[!example] Dimostrazione
>Per il teorema di completezza di $\mathbb{R}$ è sufficiente provare che la successione è di Cauchy, cioè: $$\forall\varepsilon>0\quad\exists N(\varepsilon)\in\mathbb{N}\qquad|\quad n,m\in N(\varepsilon)\Longrightarrow|x_{n}-x_{m}|<\varepsilon$$
>Ragionando per assurdo, supponiamo che $\set{x_{n}}$ non sia di Cauchy: $$\exists \varepsilon>0\quad |\quad\forall n\in\mathbb{N}\quad\exists n_{N},m_{N}\leq N\quad |\quad|x_{m_{N}-x_{n_{N}}}|\geq\varepsilon$$
>Possiamo sempre pensare che $m_{N}< n_{N}$ così per la monotonia $x_{m_{N}}\leq x_{n_{N}}$ e $\varepsilon\leq |x_{m_{N}}-x_{n_{N}}|=x_{n_{N}}-x_{m_{N}}$, cioè: $$x_{n_{N}}\geq x_{m_{N}}+\varepsilon$$
>Per $$\begin{align*}
>N_{1}&:=1\quad\exists n_{1}>m_{1}\geq N_{1}=1\quad |\quad x_{n_{1}}\geq >x_{m_{1}}+\varepsilon\\
N_{2}&:=n_{1}\quad\exists n_{2}>m_{2}\geq N_2=n_{1}\quad |\quad x_{n_{2}}> x_{m_{2}}+\varepsilon\geq x_{n_{1}}+\varepsilon>x_{m_{1}}+2\varepsilon\\
\vdots\\
N_{k+1}&:=n_{k}\quad\exists n_{k+1}>m_{k+1}\geq N_{k+1}=n_{k}\quad|\quad x_{n_{k+1}}\geq x_{m_{1}}+k\varepsilon\quad\forall k\in \mathbb{N}
>\end{align*}$$
>Quindi possiamo dire che $$\lim_{k}x_{n_{k+1}}\geq\lim_{k}(x_{m_{1}}+k\varepsilon)=+\infty$$
>Di conseguenza, $\set{x_{n}}_{n\in\mathbb{N}}$ non è superiormente limitata, contraddicendo una delle ipotesi.
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
>Poiché $A$ è superiormente limitato, esiste $b_{0}\in\mathbb{R}$ maggiorante di $A$: $$\forall x\in A\quad\exists b_{0}\in\mathbb{R}\qquad|\quad x\leq b_{0}$$
>Sia $a_{0}\in A$ un elemento fissato di $A$ in modo che: $$[a_{0},b_{0}]\cap A\neq\emptyset$$
>Sia $c:= \frac{a_{0}+b_{0}}{2}$ il punto medio di $[a_{0},b_{0}]$ e consideriamo i due sub-intervalli $[a_{0},c]$ e $[c,b_{0}]$. Evidentemente in almeno uno dei due sub-intervalli vi sono elementi di $A$. Ne scegliamo uno dei due, denotandolo con $[a_{1},b_{1}]$, optando per quello di destra se entrambe le metà contengono elementi di $A$. Evidentemente abbiamo che: $$[a_{1},b_{1}]\cap A\neq\emptyset$$
>Inoltre abbiamo che, $b_{1}$ è maggiorante di $A$: $$\forall x\in A\quad b_{1}\in\mathbb{R}\qquad|\quad x\leq b_{1}$$
>Iterando questo procedimento (detto dicotomia) otteniamo una successione crescente di intervalli: $$\cdots\subset[a_{n+1},b_{n+1}]\subset[a_{n},b_{n}]\subset\cdots\subset[a_{1},b_{1}]\subset[a_{0},b_{0}]$$
>Tali che per ogni $n\geq1$ si ha che $b_{n}$ è maggiorante di $A$:
>$$n\geq 1\quad \forall x\in A\quad b_{n}\in\mathbb{R}\qquad|\quad x\leq b_{n}$$
>E che per ogni $n\geq1$ si ha che: $$[a_{n},b_{n}]\cap A\neq\emptyset$$
>Definiamo le successioni $\set{a_{n}}$ crescente e superiormente limitata da $b_{0}$, e la successione $\set{b_{n}}$ decrescente e inferiormente limitata da $a_{0}$: $$\begin{align*}
>\cdots\leq a_{n}\leq a_{n+1}\leq\cdots\leq b_{0}\\
>a_{0}\leq\cdots\leq b_{n+1}\leq b_{n}\leq\cdots
>\end{align*}$$
>Per il teorema della convergenza di successioni monotone limitate in $\mathbb{R}$, entrambe le successioni convergono. Inoltre Poiché: $$\lim_{n\to+\infty} b_{n}-a_{n}=\lim_{n\to+\infty}\frac{b_{0}-a_{0}}{2^{n}}=0$$
>Per le proprietà del limite, esiste un $\overline{x}\in\mathbb{R}$ limite comune delle due successioni: $$\overline{x}=\lim_{n\to+\infty}a_{n}=\lim_{n\to+\infty}b_{n}$$
>Mostriamo ora che $\overline{x}=\sup(A)$. Infatti, per la proprietà di monotonia del limite, passando al limite: $$\forall x\in A\qquad|\quad x\leq\lim_{n\to+\infty} b_{n}=\overline{x}$$
>E quindi $\overline{x}$ è un maggiorante di $A$.
>
>Se per assurdo, non fosse $\overline{x}=\sup(A)$, esisterebbe $\varepsilon>0$ per il quale $\overline{x}-\varepsilon$ sarebbe un maggiorante di $A$, strettamente minore di $\overline{x}$: $$\forall x\in A\qquad|\quad x\leq \overline{x}-\varepsilon<\overline{x}$$
>Ma poiché $\overline{x}=\lim\limits_{n\to+\infty}a_{n}$, esisterebbe un $n\geq1$ per cui $\overline{x}-\varepsilon<a_{n}<\overline{x}$. Ciò contraddirebbe il fatto che, per costruzione $[a_{n},b_{n}]\cap A\neq\emptyset$.

### Punti di accumulazione
>[!note] Punti di accumulazione
>Dato un insieme $E\subseteq\mathbb{R}$, un punto $\bar{x}\in\mathbb{R}$ è detto di accumulazione per $E$ se: $$\forall\varepsilon>0\quad(E\smallsetminus\set{\bar{x}})\cap(\bar{x}-\varepsilon,\bar{x}+\varepsilon)\neq\emptyset\iff$$$$\forall\varepsilon>0\quad\exists x\in E\smallsetminus\set{\bar{x}}\quad |\quad |x-\bar{x}|<\varepsilon\iff$$$$\forall\varepsilon>0\quad \#(E\cap(\bar{x}-\varepsilon,\bar{x}+\varepsilon))=\infty$$
>L'insieme dei punti di accumulazione di $E\subseteq\mathbb{R}$ è detto insieme derivato di $E$ e si denota con $E'$.
### Proprietà di Bolzano-Weierstrass
>[!note]
>Sia $E\subset\mathbb{R}$ un insieme limitato e infinito. L'insieme dei punti di accumulazione $E'$ di $E$ è allora non vuoto: $$E'\neq\emptyset$$

>[!example] Dimostrazione
>Poiché $E$ è limitato, esiste un intervallo limitato $E\subseteq[a_{0},b_{0}]\subset\mathbb{R}$ che lo contiene. Sia $c:=\frac{a_{0}+b_{0}}{2}$ il punto medio di $[a_{0},b_{0}]$. Evidentemente almeno uno dei due sub-intervalli $[a_{0},c]$ e $[c,b_{0}]$ contiene infiniti punti di $E$.
>Ne scegliamo uno e lo denotiamo con $[a_{1},b_{1}]$. Avremo che: $$\#([a_{1},b_{1}]\cap E)=\infty$$
>Iterando questo procedimento (detto dicotomia) otteniamo una successione decrescente di intervalli: $$\cdots\subset[a_{n+1},b_{n+1}]\subset[a_{n},b_{n}]\subset\cdots\subset[a_{1},b_{1}]\subset[a_{0},b_{0}]$$
>Tale che per ogni $n\geq1$ si ha che: $$n\geq 1\quad \#([a_{n},b_{n}]\cap E)=\infty$$
>Definiamo le successioni $\set{a_{n}}$ crescente e superiormente limitata da $b_{0}$, e la successione $\set{b_{n}}$ decrescente e inferiormente limitata da $a_{0}$: $$\begin{align*}
>\cdots\leq a_{n}\leq a_{n+1}\leq\cdots\leq b_{0}\\
>a_{0}\leq\cdots\leq b_{n+1}\leq b_{n}\leq\cdots
>\end{align*}$$
>Per il teorema della convergenza di successioni monotone limitate in $\mathbb{R}$, entrambe le successioni convergono. Inoltre Poiché: $$\lim_{n\to+\infty} b_{n}-a_{n}=\lim_{n\to+\infty}\frac{b_{0}-a_{0}}{2^{n}}=0$$
>Per le proprietà del limite, esiste un $\overline{x}\in\mathbb{R}$ limite comune delle due successioni: $$\overline{x}=\lim_{n\to+\infty}a_{n}=\lim_{n\to+\infty}b_{n}$$
>Scegliendo $x_{n}\in[a_{n},b_{n}]\cap E$ con $x_{n}\neq\overline{x}$ (ciò si può fare poiché in $[a_{n},b_{n}]\cap E$ vi sono infiniti punti ed al più uno solo di essi può coincidere con $\overline{x}$), otteniamo una successione $\set{x_{n}}\subseteq E\smallsetminus\set{\overline{x}}$ tale che: $$a_{n}\leq x_{n}\leq b_{n}\quad n\geq 1$$
>Per la proprietà di monotonia del limite delle successioni, abbiamo che: $$\overline{x}=\lim_{n}a_{n}\leq \lim_{n}x_{n}\leq\lim_{n}b_{n}=\overline{x}$$
>Così $\overline{x}=\lim\limits_{n\to+\infty}x_{n}\in E'$ e l'insieme derivato risulta non vuoto $E'\neq\emptyset$ .
