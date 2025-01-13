### Proprietà
1. Linearità:
Sia $a,b\in\mathbb{R}\quad,\quad I\subset\mathbb{R}$ e: $$\int_{I}(a\cdot f+ b\cdot g)\text{ d}x=a\cdot \int_{I} f\text{ d}x+b\cdot \int_{I} g\text{ d}x\Longrightarrow f,g\in\mathcal{R}(I)$$
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

### Integrazione per parti
>[!note]
>Siano $f,g\in C([a,b])$ e $f',g'\in C([a,b])$, allora: $$\int_{a}^{b} f'\cdot g= [f\cdot g]^{b}_{a}-\int_{a}^{b}f\cdot g'$$

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
>Si integrano entrambi i membri dell'equazione di Leibniz: $$\int^{b}_{a}(f\cdot g)'=\int^{b}_{a}(f'\cdot g+f\cdot g')=\underbrace{\int^{b}_{a}f'\cdot g}_{[f\cdot g]^{b}_{a}}+\int^{b}_{a}f\cdot g'$$
### Integrazione per sostituzione
>[!note]
>Siano $f\in C([a,b])\subset\mathcal{R}$ e $\varphi:[c,b]\to[a,b]$ derivabile e $\varphi'\in C([a,b])$ strettamente monotona e crescente. Fissato $\varphi(c)=a$ e $\varphi(d)=b$, allora vale la seguente proprietà:
>$$\int_{a}^{b}f(y)\text{ d}y=\int_{c}^{d}f(\varphi(x))\cdot \varphi'(x)\text{ d}x$$

>[!example] Dimostrazione
>Sia $F$ primitiva di $f$ e poniamo $G:=F\circ\varphi$, in questo modo: $$G'=(F\circ\varphi)'=F'(\varphi(x))\cdot\varphi'(x)=f(\varphi(x))\cdot\varphi'(x)$$
>Per il primo teorema del calcolo integrale: $$\begin{align*}
\int_{a}^{b}f(y)\text{ d}y&=F(b)-F(a)= F(\varphi(d))-F(\varphi(c))\\
&= G(d)-G(c)\\
&=\int_{d}^{c}G'(x)\text{ d}x=\int_{c}^{d}f(\varphi(x))\cdot \varphi'(x)\text{ d}x
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

### Area delimitata da funzioni
>[!note]
>Per calcolare l'area delimitata dei grafici di $f(x)$ e $g(x)$ nell'intervallo $[a,b]$ vale:
>$$\int^{b}_{a}[f(x)-g(x)]\text{ d}x\qquad\iff\qquad f(x)\geq g(x)\quad\forall x\in[a,b]$$
>In caso il segno di una funzione rispettivamente all'altra vari, si scompone l'integrale in più integrali, per esempio se la funzione cambia nel punto $B$: $$\int_{a}^{c}|f(x)-g(x)|\text{ d}x=\int_{a}^{b}|f(x)-g(x)|\text{ d}x+\int_{b}^{c}|f(x)-g(x)|\text{ d}x$$
>![[Pasted image 20240520105750.png]]
