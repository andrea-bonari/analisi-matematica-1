### Teorema di derivabilità con asintotico
>[!note]
>Siano $f,g:(a,b)\to\mathbb{R}$ e $x_{0}\in(a,b)$ tali che: $$f(x)-f(x_{0})\sim g(x)-g(x_{0})\quad \text{per }x\to x_{0}$$
>Allora $f$ è derivabile in $x_{0}$ se e solo se $g$ è derivabile nello stesso punto, e in tal caso si ha che: $$f'(x_{0})=g'(x_{0})$$

>[!example] Dimostrazione
>Sappiamo che: $$f(x)-f(x_{0})\sim g(x)-g(x_{0})\quad \text{per }x\to x_{0}$$
>Significa anche: $$\lim_{x\to x_{0}} \frac{f(x)-f(x_{0})}{g(x)-g(x_{0})}=1$$
>Riscriviamo quindi il rapporto incrementale di $f$ e lo trasformiamo nel rapporto incrementale di $g$: $$\begin{align*}
&\lim_{x\to x_{0}}\frac{f(x)-f(x_{0})}{x-x_{0}}=\lim_{x\to x_{0}}\frac{f(x)-f(x_{0})}{g(x)-g(x_{0})}\cdot \frac{g(x)-g(x_{0})}{x-x_{0}}\\
=&\left(\lim_{x\to x_{0}} \frac{f(x)-f(x_{0})}{g(x)-g(x_{0})}\right)\cdot\left(\lim_{x\to x_{0}} \frac{g(x)-g(x_{0})}{x-x_{0}}\right)\\
=&\lim_{x\to x_{0}} \frac{g(x)-g(x_{0})}{x-x_{0}} 
\end{align*}$$

### Lemma di Fermat
>[!note]
>Considero una funzione $f:(a,b)\to\mathbb{R}$ e un punto di estremo per una funzione (massimo o minimo) $x_{0}\in(a,b)$. se la funzione è derivabile in $x_{0}$, allora la sua derivata vale $0$.

>[!tip] Corollario del teorema di fermat
>Se $f:(a,b)\to\mathbb{R}$, i suoi punti estremi sono da cercarsi nell'insieme $A\cap B$, dove $A,B$ sono insiemi finiti:
>$$A=\set{x\in(a,b)\space|\space\exists f'(x)=0}$$$$B=\set{x\in(a,b)\space|\space\nexists f'(x)}$$

>[!example] Dimostrazione
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

### Criterio di convessità/concavità
>[!note]
>Sia $f:(a,b)\to\mathbb{R}$ $2$ volte derivabile in $(a,b)$, allora se: $$\begin{align*}
>f''(x)&\geq 0\quad\forall x\in (a,b)\Longrightarrow f\text{ è convessa}\\
>f''(x)&\leq 0\quad\forall x\in (a,b)\Longrightarrow f\text{ è concava}
>\end{align*}$$
>I punti $x_{0}\in(a,b)$ attorno a cui $f$ cambia concavità si chiamano punti di flesso.

>[!example] Dimostrazione
>Consideriamo solo il primo caso.
>Per l'ipotesi, sfruttando il teorema di Taylor con resto di Lagrange: $$f(y)=f(x)+f'(x)\cdot(y-x)+ \frac{f''(c)}{2}\cdot(y-x)^{2}$$
>Dove $c$ è compreso tra $x$ e $y$: $$|c-x|\leq|y-x|$$
>Siccome per ipotesi $f''(z)\geq0\quad \forall z\in(a,b)$ si ha: $$f''(c)\geq 0\Longrightarrow \frac{f''(c)}{2}(y-x)^{2}\geq0$$
>E di conseguenza: $$\begin{align*}
>f(y)&= f(x)+f'(x)\cdot(y-x)+ \frac{f''(c)}{2}\cdot (y->x)^{2}\geq\\
>&\geq f(x) + f'(x)\cdot (y-x)\qquad\forall x,y\in(a,b)
>\end{align*}$$
