>[!note]
>Il limite di successione $n\in\mathbb{Q}$ è una successione $\{x_{n}\}_{n\in\mathbb{N}}\subseteq\mathbb{Q}$ che converge al numero $l\in\mathbb{Q}$ e in simboli si scrive: $$\lim_{x\to+\infty}x_{n}=l$$
>
>Le definizioni formali di limite sono: $$\begin{align*}&\forall\varepsilon>0\quad,\quad N(\varepsilon)\in\mathbb{N}\quad|\quad n\geq N(\varepsilon)\Longrightarrow|x_{n}-l|<\varepsilon\\&\forall\varepsilon>0\quad,\quad N(\varepsilon)\in\mathbb{N}\quad |\quad n\geq N(\varepsilon)\Longrightarrow l-\varepsilon<x_{0}<l+\varepsilon\\
&\forall\varepsilon>0\quad,\quad N(\varepsilon)\in\mathbb{N}\quad |\quad n\geq N(\varepsilon)\Longrightarrow x_{n}\in(l-\varepsilon,l+\varepsilon)\\
&\forall\varepsilon>0\quad,\quad N(\varepsilon)\in\mathbb{N}\quad |\quad n\geq N(\varepsilon)\Longrightarrow\{x_{n}\}_{n\geq N(\varepsilon)}\subseteq(l-\varepsilon,l+\varepsilon) \end{align*}$$
>Dove $\varepsilon$ è l'errore (o tolleranza) e $N(\varepsilon)$ è la soglia, cioè il valore oltre il quale la successione è racchiusa nell'intervallo $(l-\varepsilon,l+\varepsilon)$.
>
>Possiamo quindi dire che se $n<N(\varepsilon)$ la successione si troverà in punti casuali, altrimenti per $n>N(\varepsilon)$ si accumulerà verso il valore del limite $l$.

### Proprietà dei limiti

>[!tip] Unicità di un limite
>$$\exists\lim_{n\to+\infty}a_{n}\in\mathbb{Q}\Longrightarrow\exists!\lim_{n\to+\infty}a_{n}$$

>[!tip] Limitatezza di una successione
>$$\exists\lim_{n\to+\infty}a_{n}\in\mathbb{Q}\Longrightarrow \{a_{n}\}_{n}\text{ limitata}$$

>[!tip] Somma di limiti
>$$\lim_{n\to+\infty}(a_{n}+b_{n})= \left(\lim_{n\to+\infty}a_{n}\right)+\left(\lim_{n\to+\infty}b_{n}\right)=l_{1}+l_{2}$$

>[!tip] Prodotto di limiti
>$$\lim_{n\to+\infty}(a_{n}\cdot b_{n})= \left(\lim_{n\to+\infty}a_{n}\right)\cdot\left(\lim_{n\to+\infty}b_{n}\right)=l_{1}\cdot l_{2}$$

>[!tip] Quoziente di limiti
>$$\lim_{n\to+\infty} \frac{a_{n}}{b_{n}}= \frac{\lim_{n\to+\infty}(a_{n})}{\lim_{n\to+\infty}(b_{n})}= \frac{l_{1}}{l_{2}}$$

### Teoremi delle successioni

>[!note] Teorema della permanenza del segno
>$$\begin{cases}
a_{n}\geq0
 \\
\exists l:=\lim_{n\to+\infty}(a_{n})\end{cases}\Longrightarrow l\geq 0$$

>[!note] Teorema della monotonia
>$$\begin{cases}
a_{n}\geq b_{n} \\
\exists l_{1}:=\lim_{n\to+\infty}(a_{n}) \\
\exists l_{2}:=\lim_{n\to+\infty}(b_{n})
\end{cases}\Longrightarrow l_{1}\geq l_{2}$$

>[!note] Prodotto di successione convergente e successione limitata
>$$\begin{cases}
\lim_{n\to+\infty}(a_{n})=0 \\
\{b_{n}\}_{n\geq0}\text{ limitata}
\end{cases}\Longrightarrow \exists \lim_{n\to+\infty}(a_{n}\cdot b_{n})=0$$

>[!note] Teorema di Cauchy
>Se la successione è convergente (esiste limite finito), allora i punti della successione oltre ad una certa soglia sono vicini tra di loro (si accumulano i punti fra loro stessi).
>$$\begin{align*}
\exists\lim_{n}(a_{n})\in\mathbb{Q}&\Longrightarrow\\
&\forall\varepsilon>0\quad\exists N(\varepsilon)\geq0|\quad n,m\geq N(\varepsilon)\Rightarrow |a_{n}-a_{m}|<\varepsilon
\end{align*}$$

>[!example] Dimostrazione teorema di Cauchy
>Sia $l:=\lim_{n}a_{n}$ al valore limite $\forall\varepsilon>0\quad\exists N(\varepsilon)\geq0|\quad n,m\geq N(\varepsilon)\Rightarrow |a_{n}-a_{m}|<\varepsilon$
>Quindi se $n,m\geq N(\varepsilon)$ si ha: $$|a_{n}-a_{m}|=|(a_{n}-l)+(l-a_{m})|\leq|a_{n}-l|+|a_{m}-l|\leq\varepsilon+\varepsilon=2\varepsilon$$
>
>Di conseguenza il teorema di Cauchy è condizione necessaria affinché una successione converga verso un valore definito e limitato nell'insieme $\mathbb{Q}$, ma non nell'insieme $\mathbb{R}$.
