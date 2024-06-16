### Lemma di Fermat
>[!note]
>Considero una funzione $f:(a,b)\to\mathbb{R}$ e un punto di estremo per una funzione (massimo o minimo) $x_{0}\in(a,b)$. se la funzione è derivabile in $x_{0}$, allora la sua derivata vale $0$.

>[!tip] Corollario del teorema di fermat
>Se $f:(a,b)\to\mathbb{R}$, i suoi punti estremi sono da cercarsi nell'insieme $A\cap B$, dove $A,B$ sono insiemi finiti:
>$$A=\set{x\in(a,b)\space|\space\exists f'(x)=0}$$$$B=\set{x\in(a,b)\space|\space\nexists f'(x)}$$

>[!example] Dimostrazione
>Consideriamo il solo caso del massimo. 
>Sia $x_{M}\in(a,b)$ il massimo di $f$ nell'intervallo $(a,b)$ tale che per ogni punto nell'intervallo generico vale: $$f(x_{M})\geq f(x)$$
>Consideriamo il caso in cui $x>x_{M}$, si ha che $$\frac{f(x)-f(x_{M})}{x-x_{M}}\leq0\Longrightarrow\lim_{x\to x_{0}}\frac{f(x)-f(x_{M})}{x-x_{M}}=f'(x)\leq0$$
>Consideriamo, analogamente, il caso $x<x_{M}$:
>$$\frac{f(x)-f(x_{M})}{x-x_{M}}\geq0\Longrightarrow\lim_{x\to x_{0}}\frac{f(x)-f(x_{M})}{x-x_{M}}=f'(x)\geq0$$
>Dalle disequazioni ottenute si ha che: $$\begin{cases}
f'(x)\leq0 \\
f'(x)\geq0
\end{cases}\quad\Longrightarrow\quad f'(x)=0\quad\text{ punto stazionario}$$

### Teorema di Lagrange
>[!note]
>Se $f\in C([a,b])$ è derivabile in $(a,b)$ allora:
>$$\exists c\in(a,b)\quad |\quad \frac{f(b)-f(a)}{b-a}=f'(c)$$
>![[Pasted image 20240508124214.png]]

>[!example] Dimostrazione
>Consideriamo una funzione $g:[a,b]\to\mathbb{R}$ tale che:
>$$g(x):=f(a)+ \left(\frac{f(b)-f(a)}{b-a}\right)(x-a)$$
>Osserviamo che $g$ è un polinomio di grado $\leq 1$, di conseguenza il suo grafico è una retta.
>Definiamo $g$ come la retta passante per $(a, f(a))$ e $(b, f(b))$, la retta ha quindi come coefficiente angolare: $$m=\frac{f(b)-f(a)}{b-a}$$
>Derivando $g(x)$ otteniamo $$g'(x)=\frac{f(b)-f(a)}{b-a}$$
>Consideriamo la funzione $h:=f-g$ sull'intervallo $[a,b]$. La funzione $h$ è continua in tutto l'intervallo, estremi inclusi e derivabile nell'intervallo estremi esclusi in quanto differenza di funzioni continue.
>
>Per il teorema di Weierstrass esiste un punto $x_{m},x_{M}\in[a,b]$ che è estremo globale.
>
>###### Caso 1
>Nel caso in cui gli estremi $[a,b]$ coincidono con $x_{m}, x_{M}$, poiché $$h(a)=f(a)-g(a)=0\qquad\text{ e }\qquad h(b)=f(b)-g(b)=0$$
>È definizione di retta, Si ha quindi che $$h(x)=0\quad\forall x\in[a,b]\Longrightarrow f(x)=g(x)$$
>E quindi che $f'(x)=g'(x)\Longrightarrow \text{ Teorema verificato}$
>
>###### Caso 2
>
>Nel caso in cui almeno uno tra $x_{m},x_{M}$ sia strettamente incluso tra $[a,b]$, quindi $$(x_{m}\vee x_{M})\in(a,b)$$Applicando il teorema di Fermat ottengo che $$0=h'(x_{M})=f'(x_{M})-g'(x_{M})$$
>e quindi $$f'(x_{M})=g'(x_{M})$$
>E quindi il teorema è verificato $\forall x\in(a,b)$

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

>[!tip] Corollario della caratterizzazione delle funzioni costanti
>Considero $f:(a,b)\to\mathbb{R}$ costante, allora la sua derivata prima $f'(x)=0\quad\forall x\in(a,b)$.

>[!tip] Corollario
>Se $f:D\to\mathbb{R}$ con $D$ unione di intervalli e $f$ derivabile in $D$, allora $f'(x)=0\quad\forall x\in D$ se e solo se $f$ è localmente costante (constante nell'intervallo o nel caso limite in un punto).

>[!example] Dimostrazione
>Solo nel caso di funzione crescente.
>Considero: $$\frac{f(y)-f(x)}{y-x}\geq0\quad\text{ se } a<x<y<b$$
>Per il teorema della permanenza del segno $$f'(x)\geq0\quad\forall x\in(a,b)$$
>
>Viceversa, supponiamo che $f'(x)\geq0\quad\forall x\in(a,b)$
>Consideriamo i punti $a<x<y<b$. per il teorema di Lagrange applicato a $f$ sull'intervallo $[a,b]$ segue che $$\exists c\in(x,y)\quad |\quad 0\leq f'(x) \Longrightarrow  f(x)\leq f(y)\qquad\forall x,y\in(a,b)\quad,\quad x<y$$
>Analogamente si dimostra la decrescenza.

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

