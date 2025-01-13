### Teorema del confronto integrale
>[!note]
>Data $f:[n_{0}+\infty)\to[0,+\infty)$, e la serie $\sum\limits_{n=n_{0}}^{\infty} a_{n}$ dove $a_{n}:=f(n)\quad n\geq n_{0}$, allora: $$\sum\limits_{n=n_{0}}^{\infty} a_{n}\text{ converge se e solo se } f\text{ è integrabile}$$

### Criterio della radice
>[!note]
>Sia $0\leq a_{n}$ e supponiamo che: $$\exists\lim_{n}\sqrt[n]{a_{n}}:=l\in[0,+\infty]$$Allora:
>1. Se $0\leq l <1$ la serie $\sum\limits_{n}a_{n}$ converge.
>2. Se $l>1$ la serie $\sum\limits_{n} a_{n}$ diverge.
>3. Se $l=1$ non si deduce niente.

>[!example] Dimostrazione
>Da $\lim_{n}\sqrt[n]{a_{n}}=l$ segue che: $$\forall \varepsilon>0\quad\exists N(\varepsilon)\geq n_{0}\quad|\quad n\geq n_{0}\Longrightarrow |\sqrt[n]{a_{n}}-l|< \varepsilon$$
>Cioè: $$l-\varepsilon<\sqrt[n]{a_{n}}<l+\varepsilon$$
>Scegliendo $0<\varepsilon<l$ e elevando alla $n$: $$(l-\varepsilon)^{n}<a_{n}<(l+\varepsilon)^{n}$$
>
>##### Caso 1
>Se $l<1$ allora $\exists \varepsilon>0\quad|\quad l+\varepsilon<1$: $$\sum\limits_{n= n_{0}}^{\infty}a_{n}<\underbrace{\sum\limits_{n=n_{0}}^{\infty}(l+\varepsilon)^{n}}_\text{Serie geometrica convergente}$$E quindi per il teorema del confronto anche $\sum\limits_{n=n_{0}}^{\infty}a_{n}$ converge.
>##### Caso 2
>Se $l>1$ allora $\exists \varepsilon>0\quad |\quad l-\varepsilon>1$: $$\underbrace{\sum\limits_{n=n_{0}}^{\infty}(l-\varepsilon)^{n}}_\text{serie geometrica divergente}<\sum\limits_{n=n_{0}}^{\infty}a_{n}$$E quindi per il teorema del confronto anche $\sum\limits_{n=n_{0}}^{\infty}a_{n}$ diverge.

### Criterio del rapporto
>[!note]
>Sia $0\leq a_{n}$ e supponiamo che: $$\exists \lim_{n}\frac{a_{n+1}}{a_{n}}:=l\in[0,+\infty)$$
>Allora:
>1. Se $0\leq l <1$ la serie $\sum\limits_{n}a_{n}$ converge
>2. Se $l>1$ la serie $\sum\limits_{n}a_{n}$ diverge
>3. Se $l=0$ non si deduce niente.

>[!example] Dimostrazione
>Da $\lim_{n} \frac{a_{n+1}}{a_{n}}=l$ segue che: $$\forall \varepsilon>0\quad\exists N(\varepsilon)\geq n_{0}\quad|\quad n\geq n_{0}\Longrightarrow \bigg| \frac{a_{n+1}}{a_{n}}-l\bigg|< \varepsilon$$
>Cioè: $$l-\varepsilon<\frac{a_{n+1}}{a_{n}}<l+\varepsilon$$
>Scegliendo $0<\varepsilon<l$ e moltiplicando per  $a_{n}$: $$0\leq(l-\varepsilon)a_{n}<a_{n+1}<(l+\varepsilon)a_{n}$$
>
>##### Caso 1
>Se $l<1$ allora $\exists \varepsilon>0\quad|\quad l+\varepsilon<1$: $$\begin{align*}\\
>&a_{n+1}<(l+\varepsilon)a_{n}<(l+\varepsilon)^{2}a_{n-1}<\cdots<(l+\varepsilon)^{n+1}a_{0} \\
>&\sum\limits_{n= n_{0}}^{\infty}a_{n}<\underbrace{\sum\limits_{n=n_{0}}^{\infty}(l+\varepsilon)^{n}}_\text{Serie geometrica convergente}
>\end{align*}$$E quindi per il teorema del confronto anche $\sum\limits_{n=n_{0}}^{\infty}a_{n}$ converge.
>##### Caso 2
>Se $l>1$ allora $\exists \varepsilon>0\quad |\quad l-\varepsilon>1$: $$\begin{align*}\\
>& a_{n}>(l-\varepsilon)a_{n-1}>(l-\varepsilon)^{2}a_{n-2}<\cdots<(l-\varepsilon)^{n}a_{n}\\
>&\underbrace{\sum\limits_{n=n_{0}}^{\infty}(l-\varepsilon)^{n}}_\text{serie geometrica divergente}>\sum\limits_{n=n_{0}}^{\infty}a_{n}
>\end{align*}$$E quindi per il teorema del confronto anche $\sum\limits_{n=n_{0}}^{\infty}a_{n}$ diverge.
### Teorema della convergenza assoluta
>[!note]
>La serie $\sum\limits_{n}a_{n}$ è assolutamente convergente se la serie $\sum\limits_{n}|a_{n}|$ converge.
>Se $\sum\limits_{n=0}^{\infty}a_{n}$ converge assolutamente, allora converge semplicemente: $$\sum\limits_{n}|a_{n}|\text{ coverge }\Longrightarrow\sum\limits_{n}a_{n}\text{ coverge }$$

>[!example] Dimostrazione
>Consideriamo le somme parziali: $$\begin{align*}
>s_{N}&:=\sum\limits_{n=0}^{N}a_{n}=\sum\limits_{\begin{matrix}n=0\\a_{n}>0\end{matrix}}^{n} a_{n}+\sum\limits_{\begin{matrix}n=0\\a_{n}<0\end{matrix}}^{n} a_{n}\\
>&= \underbrace{\sum\limits_{\begin{matrix}n=0\\a_{n}>0\end{matrix}}^{N}a_{n}}_{s_{N}^{+}}-\underbrace{\sum\limits_{\begin{matrix}n=0\\a_{n}<0\end{matrix}}^{n} -(a_{n})}_{s_{N}^{-}}=s_{N}^{+}-s_{N}^{-}
>\end{align*}$$
>Sappiamo che $s_{N}^{\pm}\leq\sum\limits_{n=0}^{N}|a_{n}|$. Poiché per ipotesi la serie $\sum\limits_{n=0}^{\infty} a_{n}$ converge assolutamente, ciò vuol dire che la serie dei moduli converge, cioè: $$\exists\lim_{N\to\infty}\sum\limits_{n=0}^{N}|a_{n}|\in[0,+\infty)$$
>Di conseguenza le successioni $\set{s_{N}^{\pm}}_{N=0}^{\infty}$ sono superiormente limitate. Abbiamo quindi che: $$s_{N}^{\pm}\leq s_{N}\leq\lim_{N\to+\infty} s_{N}\in[0,+\infty)$$
>Ma poiché le successioni $\set{s_{N}^{\pm}}_{N=0}^{\infty}$ sono anche monotone crescenti (poiché a termini positivo), per il teorema di convergenza delle successioni monotone crescenti e superiormente limitate: $$\exists s^{\pm}:=\lim_{N\to+\infty}s_{N}^{\pm}\in[0,\infty)$$
>Quindi: $$\lim_{N\to+\infty} s_{N}=\lim_{N\to+\infty}(s_{N}^{+}-s_{N}^{-})=\lim_{N\to+\infty} s^{+}_{N}-\lim_{N\to+\infty} s_{N}^{-}=s^{+}-s^{-}\in\mathbb{R}$$
>E quindi la serie $\sum\limits_{n=0}^{\infty}a_{n}$ converge semplicemente.
### Criterio di Leibniz per la convergenza di serie con termini di segno alterno
>[!note]
>Se la serie $\sum\limits_{n=0}^{\infty}(-1)^{n}a_{n}$ soddisfa le seguenti ipotesi:
>- La serie ha termini di segno alterno: $a_{n}\geq0\quad \forall n\geq0$
>- È soddisfatta la condizione necessaria per la convergenza: $\lim\limits_{n\to+\infty}a_{n}=0$
>- La successione $\set{a_{n}}_{n=0}^{\infty}$ sia monotona decrescente
>
>Allora converge semplicemente. In più il resto della serie: $$R_{N}:=\sum\limits_{n=N}^\infty(-1)^{n}a_{n}$$
>È stimato da $|R_{n}|\leq a_{N+1}\quad\forall N\geq0$.

>[!example] Dimostrazione
>Analizziamo le somme parziali pari: $$\begin{align*}
>s_{0}&= a_{0}\\
>s_{2}&= a_{0}-a_{1}+a_{2}=s_{0}-\underbrace{(a_{1}-a_{2})}_\text{positiva per ipotesi III}\leq s_{0}\\
>s_{4}&= a_{0}-a_{1}+a_{2}-a_{3}+a_{4}=s_{2}-(a_{3}-a_{4})\leq s_{2}\leq s_{0}\\
>\vdots\\\forall& n\geq0\qquad s_{2n}\leq\cdots\leq s_{4}\leq s_{2}\leq s_{0}
>\end{align*}$$
>Analizziamo adesso le somme parziali dispari: $$\begin{align*}
>s_{1}&= a_{0}-a_{1}\\
>s_{3}&= a_{0}-a_{1}+a_{2}-a_{3}=s_{1}+\underbrace{(a_{2}-a_{3})}_\text{positiva per ipotesi III}\geq s_{1}\\
>s_{5}&= a_{0}-a_{1}+a_{2}-a_{3}+a_{4}-a_{5}=s_{3}+(a_{4}-a_{5})\geq s_{3}\geq s_{1}\\
>\vdots\\\forall& n\geq0\qquad s_{1}\leq s_{3}\leq\cdots\leq s_{2n+1}
>\end{align*}$$
>In più abbiamo che: $$s_{2N}-s_{2N+1}=a_{2n+1}\geq0$$
>Che implica: $$s_{1}\leq s_{3}\leq\cdots\leq s_{2n+1}\leq s_{2n}\leq\cdots\leq s_{2}\leq s_{0}$$
>Cioè $\set{s_{2N}}_{N=0}^{\infty}$ è decrescete e inferiormente limitata, mentre $\set{s_{2N+1}}_{N=0}^{\infty}$ è crescente e superiormente limitata.
>Per il teorema della convergenza di successioni monotone limitate: $$\begin{align*}
>&\exists\lim_{N\to+\infty}s_{2N}=:s_{p}\in\mathbb{R}\\
>&\exists\lim_{N\to+\infty}s_{2N+1}=:s_{d}\in\mathbb{R}
>\end{align*}$$
>Ed anche $s_{d}\leq s_{p}$. Ma poiché $s_{2N}-s_{2N+1}=a_{2N+1}\stackrel{N\to+\infty}{\to}0$
>Si ha $s_{d}-s_{p}=:s\in\mathbb{R}$ quindi: $$\begin{align*}
>&\forall \varepsilon>0\quad\exists N_{d}(\varepsilon)>0\quad |\quad N\geq N_{d}(\varepsilon)\Longrightarrow |s_{2N+1}-s|<\varepsilon\\
>&\forall\varepsilon>0\quad\exists N_{p}(\varepsilon)>0 \quad|\quad N\geq N_{p}(\varepsilon)\Longrightarrow|s_{2N}-s|<\varepsilon
>\end{align*}$$
>Definendo $N(\varepsilon):=\max(N_{d}(\varepsilon),N_{p}(\varepsilon))$ si ha: $$N\geq N(\varepsilon)\Longrightarrow|s_{N}-s|<\varepsilon$$
>Cioè: $$\exists\lim_{N\to++\infty}s_{n}=s\in \mathbb{R}$$
>Cioè la serie $\sum\limits_{n=0}^{\infty}(-1)^{n}a_{n}$ converge.
