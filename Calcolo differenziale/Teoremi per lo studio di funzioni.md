### Lemma di Fermat
>[!note]
>Considero una funzione $f:(a,b)\to\mathbb{R}$ e un punto di estremo per una funzione (massimo o minimo) $x_{0}\in(a,b)$. se la funzione è derivabile in $x_{0}$, allora la sua derivata vale $0$.

>[!tip] Corollario del teorema di fermat
>Se $f:(a,b)\to\mathbb{R}$, i suoi punti estremi sono da cercarsi nell'insieme $A\cap B$, dove $A,B$ sono insiemi finiti:
>$$A=\set{x\in(a,b)\space|\space\exists f'(x)=0}$$$$B=\set{x\in(a,b)\space|\space\nexists f'(x)}$$

>[!example]
>Per semplicità supponiamo $x_{0}$ punto di massimo assoluto o globale: $$f(x)\leq f(x_{0})\qquad\forall x\in(a,b)$$
>Se $x>x_{0}$ allora: $$\frac{f(x)-f(x_{0})}{x-x_{0}}\leq0\Longrightarrow \lim_{x\to x_{0}^{+}}\frac{f(x)-f(x_{0})}{x-x_{0}}=f'(x)\leq 0$$
>Analogamente, se $x< x_{0}$ allora: $$\frac{f(x)-f(x_{0})}{x-x_{0}}\geq0\Longrightarrow\lim_{x\to x_{0}^{-}}\frac{f(x)-f(x_{0})}{x-x_{0}}=f'(x)\geq 0$$
>Quindi: $$\begin{cases}
f'(x_{0})\geq0 \\
f'(x_{0})\leq0
\end{cases}\Longrightarrow f'(x_{0})=0$$

### Teorema di Lagrange
>[!note]
>Se $f\in C([a,b])$ è derivabile in $(a,b)$ allora:
>$$\exists c\in(a,b)\quad |\quad \frac{f(b)-f(a)}{b-a}=f'(c)$$
>![[Pasted image 20240508124214.png]]

>[!example] Dimostrazione
>Consideriamo una funzione $g:[a,b]\to\mathbb{R}$ tale che:
>$$g(x):=f(a)+ \left(\frac{f(b)-f(a)}{b-a}\right)(x-a)$$
>Osserviamo che $g$ è un polinomio di grado $\leq 1$, di conseguenza il suo grafico è una retta. Il grafico di $g$ è la retta secante a $G(f)$ passante per i suoi estremi $a$ e $b$, infatti: $$\begin{cases}
>g(a)=f(a) \\
>g(b)=f(b)
>\end{cases}$$
>Consideriamo adesso la funzione: $$h:= f-g\quad \forall x\in[a,b]$$
>$h$ è una funzione continua e derivabile su $(a,b)$, inoltre $h(a)=h(b)=0$.
>
>Per il teorema di Weierstrass $\exists x_{m},x_M\in[a,b]$ punti di minimo e massimo globale per $h$: $$h(x_{m})\leq h(x)\leq h(x_{M})\quad\forall x\in[a,b]$$
>
> ##### Caso 1
>Nel caso in cui $x_{m}$ e $x_{M}$ sono gli estremi di $[a,b]$, abbiamo che $h(x)=0\quad\forall x\in[a,b]$ e quindi: $$0=h'(x)=(f-g)'(x)=f'(x)-g'(x)$$
>Siccome $f'(x)=g'(x)=\frac{f(b)-f(a)}{b-a}\quad\forall x\in(a,b)$ ogni punto $c\in(a,b)$ è punto di Lagrange.
>
>##### Caso 2
>Nel caso in cui almeno uno tra $x_{m}$ e $x_{M}$ è in $(a,b)$, sia $c$ tale punto, e per il lemma di Fermat: $$0=h'(c)=f'(c)-g'(c)$$
>E siccome $f'(x)=g'(x)=\frac{f(b)-f(a)}{b-a}\quad\forall x\in(a,b)$ abbiamo che $c$ è punto di lagrange.

### Teorema di Rolle
>[!note]
>Considerata una funzione tale che $f(a)=f(b)$, allora:
>$$\exists c\in(a,b)\quad|\quad f'(c)=\frac{f(b)-f(a)}{b-a}=0$$
>![[Pasted image 20240508124445.png]]

### Test della monotonia
>[!note]
>Sia $f:(a,b)\to\mathbb{R}$ una funzione derivabile in $(a,b)$, allora:
>1. $f\text{ crescente}\iff f'(x)>0\quad\forall x\in(a,b)$
>2. $f\text{ descrescente}\iff f'(x)<0\quad\forall x\in(a,b)$
>3. $f\text{ stazionaria}\iff f'(x)=0\quad\forall x\in(a,b)$ 

>[!example] Dimostrazione
>Consideriamo solo il caso di $f$ crescente in $(a,b)$: $$a<x<y<b\Longrightarrow f(x)\leq f(y)$$
>E di conseguenza: $$\frac{f(y)-f(x)}{y-x}\geq0$$
>E per il teorema di permanenza del segno: $$f'(x)=\lim_{y\to x}\frac{f(y)-f(x)}{y-x}\geq0$$
>
>Se invece $f'(x)\geq\quad\forall x\in(a,b)$, fissiamo $a<x<y<b$ e applichiamo il teorema di Lagrange a $f$ sul $[x,y]$: $$\exists f'(c)=\frac{f(y)-f(x)}{y-x}\geq0$$
>E quindi $f(x)\leq f(y)$.

>[!tip] Corollario della caratterizzazione delle funzioni costanti
>Considero $f:(a,b)\to\mathbb{R}$ costante, allora la sua derivata prima $f'(x)=0\quad\forall x\in(a,b)$.

>[!tip] Corollario
>Se $f:D\to\mathbb{R}$ con $D$ unione di intervalli e $f$ derivabile in $D$, allora $f'(x)=0\quad\forall x\in D$ se e solo se $f$ è localmente costante (constante nell'intervallo o nel caso limite in un punto).

### Punti di non derivabilità

>[!note] Punti angolosi
>Un punto è detto angoloso quando il limite destro e sinistro della derivata esistono ma non coincidono (almeno una finita):
>$$\exists\lim_{x\to x_{0}^{+}}\frac{f(x)-f(x_{0})}{x-x_{0}}\neq\lim_{x\to x_{0}^{-}}\frac{f(x)-f(x_{0})}{x-x_{0}}$$
>![[Pasted image 20240508125616.png]]

>[!note] Flessi verticali
>Un punto è detto flesso verticale quando il limite destro e sinistro della tangente sono entrambi o $+\infty$ o $-\infty$
>$$\lim_{x\to x_{0}^{\pm}}\frac{f(x)-f(x_{0})}{x-x_{0}}=+\infty\quad\vee\quad \lim_{x\to x_{0}^{\pm}}\frac{f(x)-f(x_{0})}{x-x_{0}}=-\infty$$
>![[Pasted image 20240508130110.png]]

>[!note] Cuspide
>Un punto è detto cuspide se i limiti della derivata devono tendere a infinito e essere discordi:
>$$\begin{cases}
\lim_{x\to x_{0}^{\pm}}\frac{f(x)-f(x_{0})}{x-x_{0}}=\pm\infty \\
\lim_{x\to x_{0}^{\mp}}\frac{f(x)-f(x_{0})}{x-x_{0}}=\mp\infty
\end{cases}$$
![[Pasted image 20240508130301.png]]

>[!note] Punti di discontinuità eliminabili
>Considerata $f:(a,x_{0})\cap(x_{0},b)$ continua in $x_{0}$ è definito punto di discontinuità eliminabile se $\exists l:=\lim_{x\to x_{0}}f(x)$, poiché esiste un'estensione continua di $\bar{f}$ in $(a,b):$
>$$\bar{f}(x)=\begin{cases}
f(x)&\text{ se }x\in(a,x_{0})\cap(x_{0},b) \\
l&\text{ se }x=x_{0}
\end{cases}$$

### Criterio di derivabilità
>[!note]
>Sia $f:(a,b)\to\mathbb{R}\quad x_{0}\in(a,b)\quad,\quad f\text{ derivabile in }(a,b)\smallsetminus\set{x_{0}}$,
>$$l=\lim_{x\to x_{0}^{-}} f'(x)=lim_{x\to x_{0}^{+}} f'(x)\in\mathbb{R}\Longrightarrow\begin{cases}
f\text{ derivabile in } x_{0} \\
f'(x_{0})=l
\end{cases}$$
>La funzione può essere definita derivabile e continua in $x_{0}$

### Derivate di ordine $n$
>[!note]
>Se $f:(a,b)\to\mathbb{R}$ è $(n-1)$ volte derivabile in $x_{0}\in(a',b')\subset(a,b)$ e la derivata di ordine $(n-1)$, $f^{n-1}(x)$ è a sua volta derivabile in $x_{0}$, diremo che $f$ è $n-\text{volte}$ derivabile e:
>$$f^{(n)}(x)=(f^{(n-1)})'(x)\qquad\text{ con }n\geq 1$$

### Concavità e convessità
>[!note] Funzione convessa e concava
>Sia $f:(a,b)\to\mathbb{R}$ derivabile in $(a,b)$, essa si definisce convessa se il suo grafico sta al di sopra di tutte le sue rette tangenti.
>Viceversa, si definisce concava se il suo grafico sta al di sotto di tutte le sue rette tangenti.
>![[Pasted image 20240508132142.png]]

>[!note] Derivata seconda e concavità
>Sia $f:(a,b)\to\mathbb{R}$ derivabile $2-\text{volte}$, allora:
>1. $f\text{ è convessa }\iff f^{(2)}(x)\geq0\quad\forall x\in(a,b)$
>2. $f\text{ è concava }\iff f^{(2)}(x)\leq0\quad\forall x\in(a,b)$

I punti dove cambia la concavità di $f$, ovvero dove cambia di segno la derivata seconda $f^{(2)}(x)$ sono detti flessi obliqui.

### Teorema di De L'Hopital
>[!note]
>Siano $f,g:(a,b)\to\mathbb{R}$ derivabili e $g\neq0$ tale che:
>$$\begin{cases}
\exists\lim_{x\to x_{0}} \frac{f'(x)}{g'(x)} \\
\lim_{x\to x_{0}}f(x)=\lim_{x\to x_{0}}g(x)
\end{cases}\Longrightarrow \lim_{x\to x_{0}}\frac{f(x)}{g(x)}=\lim_{x\to x_{0}}\frac{f'(x)}{g'(x)}$$

>[!example] Dimostrazione
>Definiamo $f(a)=g(a)=0$, estendibile in maniera continua all'intervallo $[a,b)$ e fissiamo $x\in[a,b)$, quindi abbiamo $f,g\in C([a,x])$, e in più derivabili in $(a,x)$, poiché derivabili in $[a,b)$ per ipotesi.
>
>Allora $f,g$ sono derivabili in $(a,b)$ e continue in $x=a$.
>Applicando il teorema di Lagrange alla funzione $h:[a,x]\to\mathbb{R}$ definita come: $$h(y):=f(x)\cdot g(y)- f(y)\cdot g(x)\qquad\forall y\in[a,x]$$
>Sappiamo che: $$\exists y(x)\in(a,x)\quad |\quad \frac{h(x)-h(a)}{x-a}= h'(g(x))$$
>Che sta a indicare che il punto di Lagrange dipende da $x$.
>Devo trovare $h'(y)$ dove $x$ è fissato:
>$$0=h'(g(x))=f(x)\cdot g(y)-f(y)\cdot g(x)\Longrightarrow \frac{f(x)}{g(x)}=\frac{f'(y(x))}{g'(y(x))}$$
>Sapendo che $a<y(x)<x$: $$\lim_{x\to a^{+}}y(x)<a^{+}$$
>Si ha quindi che $$\lim_{x\to a^{+}}\frac{f(x)}{g(x)}=\lim_{x\to a^{+}}\frac{f'(y(x))}{g'(y(x))}= \lim_{y\to a^{+}}\frac{f'(y)}{g'(y)}=l$$

