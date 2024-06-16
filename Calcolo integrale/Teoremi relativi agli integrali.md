### Primo teorema fondamentale del calcolo integrale
>[!note]
>Se $f\in C([a,b])$ è continua, allora è integrabile su $[a,b]$. La notazione per le funzioni integrabili è $$\mathcal{R}([a,b]):=\set{\text{ tutte le }f\text{ integrabili su }[a,b]}$$

>[!note] Primitiva di una funzione
>Sia $f:(a,b)\to\mathbb{R}$. Una funzione $F:(a,b)\to\mathbb{R}$ è detta primitiva di $f$ se:
>- $F$ è derivabile
>- $F'(x)=f(x)\quad\forall x\in(a,b)$

>[!example] Dimostrazione
>Per ogni partizione $$P=\set{I_{k}}^{n}_{k=1}\quad I_{k}=[x_{k},x_{k+1}]\qquad,\quad x_{0}=a\space,\space x_{n}=b$$
>Abbiamo $$F(b)-F(a)=F(x_{n})-F(x_{0})=\sum\limits^{n}_{k=0}[F(x_{k})-F(x_{k-1})]$$
>Questa sommatoria è detta telescopica.
>Applicando il teorema di Lagrange a $F$ su $[x_{k},x_{k+1}]$:
>$$\exists y_{k}\in(x_{k-1},x_{k})\quad |\quad \frac{F(x_{k})-F(x_{k-1})}{x_{k}-x_{k-1}}=F'(y_{k})-f(y_{k})=0$$
>Cioè: $$F(x_{k})-F(x_{k-1})=f(y_{k})\cdot (x_{k}-x_{k-1})=|I_{k}|\cdot f(y_{k})$$
>Quindi possiamo affermare, dalla precedente sommatoria:
>$$\sum\limits^{n}_{k=1}[F(x_{k})-F(x_{k-1})]=\sum\limits_{k=1}^{n}|I_{k}|f(y_{k})$$
>Poiché: $$y_{k}\in(x_{k-1},x_{k})\Longrightarrow \inf(f)\leq f(y_{k})\leq\sup(f)$$
>Passiamo quindi alla sommatoria:
>$$\sum\limits_{k=1}^{n}|I_{k}|\begin{pmatrix}\inf(f)\\I_{k}\end{pmatrix}\leq\sum\limits_{k=1}^{n}|I_{k}|f(y_{k})\leq\sum\limits_{k=1}^{n}|I_{k}|\begin{pmatrix}\sup(f)\\I_{k}\end{pmatrix}$$
>Che corrisponde a dire che $$s(f,P)\leq F(b)-F(a)\leq S(f,P)\qquad \forall P\in \mathcal{P}(I)$$
>Passando a Inf e Sup: $$\inf\set{s(f,P)\quad |\quad \forall P\in \mathcal{P}(I)}\leq F(b)-F(a)\leq \sup\set{S(f,P)\quad |\quad \forall P\in \mathcal{P}(I)}$$
>Quindi: $$\underline{I}(f)\leq F(b)-F(a)\leq\overline{I}(f)$$
>E siccome per ipotesi $f$ è integrabile: $$F(b)-F(a)=\underline{I}(f)=\overline{I}(f)=\int^{b}_{a}f(x)\text{ d}x$$

Due funzioni primitive $F,G$ di $f$, differiscono di una costante su $[a,b]$. Se $F-G$ è costante su $[a,b]$ si dice che le curve sono parallele (o coincidenti se la distanza è $0$). Per indicare una famiglia di primitive si usa la notazione: $$\int f(x)\text{ d}x=g(x)+c$$
### Proprietà e interpretazione dell'integrale
1. Linearità:
Sia $a,b\in\mathbb{R}\quad,\quad I\subset\mathbb{R}$ e: $$\int_{I}(a\cdot f+ b\cdot g)\text{ d}x=a\cdot \int_{i} f\text{ d}x+b\cdot \int_{I} g\text{ d}x\Longrightarrow f,g\in\mathcal{R}(I)$$
2. Positività: $$\begin{cases}
f\in\mathcal{R}(I) \\
f\geq0
\end{cases}\Longrightarrow \int_{I}f\text{ dx}\geq0$$
3. Monotonia: $$\begin{cases}
f,g\in\mathcal{R}(I) \\
f\leq g
\end{cases}\Longrightarrow\int_{I}f\text{ d}x\leq\int_{I}g\text{ d}x$$
4. Annullamento: $$\begin{cases}
f\in C(I)\subset\mathcal{R}(I) \\
f\geq0 \\
\int_{I}f=0
\end{cases}\Longrightarrow \int_{I}f\geq0\text{ su }[a,b]$$
5. Additività: $$\begin{cases}
a<b<c \\
f\in(\mathcal{R}([a,b])\cap\mathcal{R}([b,c]))
\end{cases}\Longrightarrow f\in\mathcal{R}([a,c])\iff \int_{a}^{c}f=\int_{a}^{b}f+\int_{b}^{c}f$$
6. Orientamento:
$$\int^{b}_{a}f=-\int^{a}_{b}f\quad\forall a,b$$
### Integrazione per parti
>[!note]
>Sia $f,g\in C([a,b])$ e $f',g'\in C([a,b])$, allora: $$\int_{a}^{b} f'\cdot g= [f\cdot g]^{b}_{a}-\int_{a}^{b}f\cdot g'$$

>[!tip] Scelta di integrazione e derivazione:
>Si usa il metodo LINATE, dando priorità a:
>1. L: Logaritmi
>2. I: Trigonometriche inverse
>3. N: Numeriche
>4. A: Polinomio algebrico
>5. T: Trigonometriche
>6. E: Esponenziali

>[!tip] Metodo DI
>Un ottima risorsa per integrare per parti è il metodo DI, è possibile approfondirlo [qui](https://www.youtube.com/watch?v=2I-_SV8cwsw)

>[!example] Dimostrazione
>Partendo dalla regola di Leibniz di derivazione: $$(f\cdot g)'= f'\cdot g+f\cdot g'$$
>Si integrano entrambi i membri dell'equazione di Leibniz: $$\int^{b}_{a}(f\cdot g)'=\int^{b}_{a}(f'\cdot g+f\cdot g')=\int^{b}_{a}f'\cdot g+\int^{b}_{a}f\cdot g'$$
### Integrazione per sostituzione
>[!note]
>Sia $f\in C([a,b])\subset\mathcal{R}\quad,\quad \varphi:[c,b]\to[a,b]$ derivabile e $\varphi'\in C([a,b])$ strettamente monotona e crescente. Fissato $\varphi(c)=a$ e $\varphi(d)=b$, allora vale la seguente proprietà:
>$$\int_{a}^{b}f(y)\text{ d}y=\int_{c}^{d}f(\varphi(x))\cdot \varphi'(x)\text{ d}x$$

>[!example] Dimostrazione
>Sia $F: [a,b]\to\mathbb{R}$ primitiva di $f$, così per il primo teorema del calcolo integrale: $$\int^{b}_{a}f(y)\text{ d}y=F(b)-F(a)$$
>Sia $G:=F\circ \varphi:[c,d]\to\mathbb{R}$, per il teorema di derivazione della funzione composta:
>$$G'=(F'\circ\varphi)\cdot \varphi'=f(\varphi(x))\cdot\varphi'(x)$$
>Quindi $G'$ è una primitiva di $(f\circ g)\cdot\varphi'$, di conseguenza per primo teorema fondamentale del calcolo integrale: $$\begin{align*}
\int^{d}_{c}f(\varphi(x))\cdot \varphi'(x)\text{ d}x &=G(d)-G(c)\\
&=F(\varphi(d))-F(\varphi(c))\\
&=F(b)-F(a)\\
&=\int^{b}_{a}f(y)\text{ d}y
\end{align*}$$
### Integrali di funzioni razionali fratte
Si elencano i vari metodi di risoluzione di funzioni razionali fratte:

##### Grado del numeratore maggiore o uguale al denominatore
1. Si esegue la divisione polinomiale
2. Si riscrive la frazione come $$\int \underbrace{P(x)}_\text{risultato della divisione}+\underbrace{ \frac{R(x)}{D(x)}}_\text{resto fratto divisore}\text{ d}x$$
3. Si risolve l'integrale scomponendolo in più integrali

##### Grado Numeratore minore del denominatore

>[!example] Esempio delta maggiore di $0$
>1. Considero l'integrale $$\int\frac{x-1}{x^{2}+5x+6}\text{ d}x$$
>2. Riscriviamo la frazione come: $$\frac{x-1}{x^{2}+5x+6}= \frac{A}{x+3}+ \frac{B}{x+2}=\frac{Ax+2A+Bx+3B}{(x+3)(x+2)}$$
>$$x-1=x(A+B)+2A+3B\Longrightarrow\begin{cases}
>A+B=1 \\
>2A+3B=-1
>\end{cases}$$
>3. Risolvendo il sistema, risolvo poi normalmente gli integrali: $$\int \frac{A}{x+3}\text{ d}x+\int\frac{B}{x+2}\text{ d}x$$

>[!example] Esempio delta uguale a $0$
>Come nell'esempio precedente:
>1. Considero l'integrale $$\int\frac{x+5}{(x+3)^{2}}\text{ d}x$$
>2. Riscriviamo la frazione, e risolviamo per $A$ e $B$: $$\frac{x+5}{(x+3)^{2}}=\frac{A}{(x+3)^{2}}+\frac{B}{x+3}=\frac{A+Bx+3B}{(x+3)^{2}}$$
>3. Risolvendo il sistema, risolvo poi normalmente gli integrali: $$\int\frac{A}{(x+3)^{2}}\text{ d}x+\int \frac{B}{x+3}\text{ d}x$$

>[!example] Esempio delta minore di $0$
>1. Considero l'integrale $$\int\frac{1}{x^{2}-6x+10}\text{ d}x$$
>2. Cerco di ricondurlo alla formula generale dell'arcotangente: $$\int\frac{f'(x)}{[f(x)]^{2}+n^{2}}\text{ d}x= \frac{1}{n}\arctan\left( \frac{x}{n}\right)+c$$$$\int\frac{1}{x^{2}-6x+10}\text{ d}x=\int\frac{1}{(x-3)^{2}+1}=\arctan(x-3)+c$$

### Teorema della media
>[!note]
>Sia $f\in C([a,b])\subset\mathcal{R}([a,b])$, allora: $$\exists x_{0}\in[a,b]\quad|\quad \frac{1}{b-a}\int^{b}_{a}f(x)\text{ d}x=f(x_{0})\iff \int^{b}_{a}f(x)\text{ d}x=f(x_{0})\cdot(b-a)$$
>![[Pasted image 20240514162130.png]]

>[!example] Dimostrazione
>Per il teorema di Weierstrass, $f$ assume estremi assoluti su $[a,b]$. Denotiamo con $m=\min(f)$ e $M=\max(f)$, e quindi $m\leq f(x)\leq M$.
>Per la monotonia: $$m(b-a)=\int^{b}_{a}m\leq\int^{b}_{a}f\leq\int^{b}_{a}M=M(b-a)$$
>E per il teorema dei valori intermedi:
>$$\exists x_{0}\in[a,b]\quad |\quad \frac{1}{b-a}\int^{b}_{a}f=f(x_{0})$$

### Secondo teorema del calcolo integrale
>[!note]
>Sia $f\in\mathcal{R}([a,b])$ e definiamo la funzione integrale $F$ su $[a,b]$:
>$$F:[a,b]\to\mathbb{R}\qquad F(x):=\int^{x}_{a}f(x)\text{ d}x$$
>Allora:
>1. Se $f$ è limitata allora $F$ è continua
>2. Se $f$ è continua allora $F$ è derivabile in $(a,b)$ e: $$F'(x)=f(x)\qquad\forall x\in(a,b)$$
>Quindi la funzione integrale $F$ è primitiva della funzione derivata $f$:
>$$\frac{\text{d}}{\text{d}x}\int^{x}_{a}f=f(x)\qquad\forall x\in(a,b)$$

>[!example] Dimostrazione
>###### Se $f$ è limitata allora $F$ è continua
>$$f\text{ limitata }\Longrightarrow \exists M \quad|\quad |f(x)|\leq M\qquad\forall x\in[a,b]$$
>Quindi:
>$$|F(x+h)-F(x)|=\left|\int^{x+h}_{a}f-\int^{x}_{a}f\right|=\left|\int^{x+h}_{x}f \right|\leq\int^{x+h}_{x}|f|\leq\int^{x+h}_{x}M=M\cdot |h|$$
>Passando al limite di $h\to 0$:
>$$M\cdot |h|\to_{h\to0}0\Longrightarrow \lim_{h\to0}|F(x+h)-F(x)|=0\iff\lim_{h\to0} F(x+h)=F(x)$$
>###### Se $f$ è continua allora $F$ è derivabile in $(a,b)$ e $F'(x)=f(x)\quad x\in(a,b)$
>
>La media dell'integrale di $f$ sull'intervallo di lunghezza $h$ è $$\frac{F(x+h)-F(x)}{h}= \frac{1}{h}\cdot\int^{x+h}_{x}f=f(y(h))$$
>Tra $x$ e $x+h$: $$|y(h)-x|\leq|(x+h)-x|=|h|\Longrightarrow \lim_{h\to0} y(h)=x$$
>E poiché è continua in $x$, allora: $$\lim_{h\to0}\frac{F(x+h)-F(x)}{h}=\lim_{h\to0}f(y(h))= f(\lim_{h\to0}y(h))=f(x)$$
>Quindi in un singolo punto l'incremento dell'area sottesa dal grafico è pari al limite dell'integrale su un intervallo che tende a zero, che è il valore della funzione stessa.
>
>Una conseguenza di questo teorema è che il primo teorema del calcolo integrale può essere espresso come: $$\int^{x}_{a}F'=F(x)-F(a)\iff F(x)=F(a)-\int^{x}_{a}F'$$

### Integrali fondamentali notevoli
$$\begin{align*}
&\int 0\text{ d}x=c&&\int \text{ d}x=x+c\\
&\int k\cdot f(x)\text{ d}x=k\cdot \int f(x)\text{ d}x&&\\\\
&\int x^{n}\text{ d}x=\frac{x^{n+1}}{n+1}+c\quad n\neq-1
&&\int[f(x)]^{n}\cdot f'(x)\text{ d}x = \frac{1}{n+1}[f(x)]^{n+1}+c\\&\int\frac{1}{2\sqrt{x}}\text{ d}x=\sqrt{x} + c&&\int\frac{f'(x)}{2\sqrt{f(x)}}\text{ d}x=\sqrt{f(x)}+c\\
&\int\sin(x)\text{ d}x=-\cos(x)+c&&\int\sin(f(x))\cdot f'(x)\text{ d}x=-\cos(f(x))+c\\
&\int\cos(x)\text{ d}x=\sin(x)+c&&\int\cos(f(x))\cdot f'(x)\text{ d}x=\sin(f(x))+c\\
&\int\frac{1}{\cos^{2}(x)}\text{ d}x=\tan(x)+c&&\int \frac{f'(x)}{\cos^{2}(f(x))}\text{ d}x=\tan(f(x))+c\\
&\int\frac{1}{\sin^{2}(x)}\text{ d}x=-\cot(x)+c&&\int \frac{f'(x)}{\sin^{2}(f(x))}\text{ d}x=-\cot(f(x))+c
\end{align*}$$

