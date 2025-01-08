### Primo teorema fondamentale del calcolo
>[!note]
>Sia $f:[a,b]\to\mathbb{R}$ integrabile ($f\in\mathcal{R}([a,b])$), e sia $$F:[a,b]\to\mathbb{R}$$
>Una primitiva tale che $F'(x)=f(x)\quad x\in(a,b)$. Allora: $$\int_{a}^{b}f(x)\text{ d}x=F(b)-F(a)$$

>[!tip]
>$$\mathcal{R}([a,b]):=\set{\text{Insieme delle funzioni integrabili su }[a,b]}$$

>[!example] Dimostrazione
>Sia $P=\set{x_{k}}_{k=0}^{n}\in\mathcal{R}([a,b])$ una partizione di $[a,b]$. Abbiamo che: $$\begin{align*}
>F(b)-F(a)=F(x_{n})-F(x_{0})=\sum\limits_{k=1}^{n} F(x_{k})-F(x_{k-1})
>\end{align*}$$
>Applicando il teorema di Lagrange alla funzione $F$ su ogni intervallo $I_{k}=[x_{k-1},x_{k}]\quad k=1,\cdots,n$. Avremo che: $$\sum\limits_{k=1}^{n} F(x_{k})-F(x_{k-1})=\sum\limits_{k=1}^{n}(x_{k}-x_{k-1})\cdot F'(y_{k})\qquad y_{k}\in(x_{k-1},x_{k})$$
>Siccome $F$ è primitiva di $f$, abbiamo che $F'(x)=f$: $$\sum\limits_{k=1}^{n}(x_{k}-x_{k-1})\cdot F'(y_{k})=\sum\limits_{k=1}^{n}|I_{k}|\cdot f(y_{k})\qquad y_{k}\in(x_{k-1},x_{k})$$
>Notiamo che: $$\left(\inf_{I_{k}}f\right)\leq f(y_{k})\leq\left(\sup_{I_{k}}f\right)\qquad k=1,\cdots,n$$
>E quindi: $$\underbrace{\sum\limits_{k=1}^{n}|I_{k}|\left(\inf_{I_{k}}f\right)}_{s(f,P)}\leq F(b)-F(a)\leq\underbrace{\sum\limits_{k=1}^{n}|I_{k}|\left(\sup_{I_{k}}f\right)}_{S(f,P)}$$
>E quindi per definizione dell'integrale superiore e inferiore: $$\underline{I}(f)\leq F(b)-F(a)\leq \overline{I}(f)$$
>Poiché per ipotesi $f$ è integrabile, si ha: $$\underline{I}(f)=\overline{I}(f)$$
>Abbiamo quindi: $$I(f)=F(b)-F(a)=\int_{a}^{b}f(x)\text{ d}x$$

### Teorema della media integrale
>[!note]
>Sia $f\in C([a,b])$ allora $\exists x_{0}\in [a,b]$ tale che: $$ \frac{1}{b-a}\int_{a}^{b}f(x)\text{ d}x= f(x_{0})$$
>Cioè: $$\int_{a}^{b}f(x)\text{ d}x=(b-a)\cdot f(x_{0})$$

>[!example] Dimostrazione
>Per il teorema di Weierstrass $\exists m,M\in\mathbb{R}$ valori minimo e di massimo assoluti: $$m\leq f(x)\leq M\qquad\forall x\in[a,b]$$
>Di conseguenza: $$(b-a)\cdot m=\int_{a}^{b}m\leq \int_{a}^{b}f\leq\int^{b}_{a}=M(b-a)\cdot M=$$

### Secondo teorema fondamentale del calcolo
>[!note]
>Sia $f\in\mathcal{R}([a,b])$ e definiamo la funzione integrale di $f$: $$F:[a,b]\to\mathbb{R}\qquad F(x)=\int_{a}^{x}f(t)\text{ d}t\quad x\in[a,b]$$
>Allora:
>1. Se $f$ è limitata allora $F$ è continua
>2. Se $f$ è continua su $[a,b]$ allora $F$ è derivabile in $(a,b)$ e $F'(x)=f(x)\quad\forall x\in(a,b)$ cioè $F$ è primitiva di $f$

>[!example] Dimostrazione
>##### Prima clausola
>Sia $f$ è limitata, allora $\exists M\geq0$ tale che: $$|f(t)|\leq M\qquad\forall t\in[a,b]$$
>Fissiamo $x\in[a,b]$. Sia quindi $h\in\mathbb{R}$: $$\begin{align*}
>0&\leq\bigg|F(x+h) - F(x) \bigg|=\bigg|\int_{a}^{x+h}f-\int_{a}^{x}f \bigg|\\
>&= \bigg|\int_{x}^{x+h}f(t)\text{ d}t \bigg|\leq\int_{x}^{x+h}|f(t)|\text{ d}t\leq\int^{x+h}_{x}M\text{ d}t=M\cdot |h|
>\end{align*}$$
>Sapendo che: $$\lim_{h\to0} |F(x+h)-F(x)|=0$$
>Abbiamo che: $$\lim_{h\to0}F(x+h)=F(x)\qquad\forall x\in[a,b]$$
>##### Seconda clausola
>Siano $f\in C([a,b])$, $x\in(a,b)$ fissato e $h\in\mathbb{R}$: $$\begin{align*}
>\frac{F(x+h)-F(x)}{h}&=  \frac{1}{h}\left[\int_{a}^{x+h}f-\int_{a}^{x}f\right]= \frac{1}{h}\int_{x}^{x+h}f
>\end{align*}$$
>Per il teorema della media integrale abbiamo che:
>$$\int_{x}^{x+h}f=f(c(h))$$
>Per un opportuno punto $c(h)$ tra $x$ e $x+h$: $$|c(h)-x|\leq|(x+h)-x|=|h|$$
>E quindi: $$\lim_{h\to0} c(h)=x$$Per la continuità di $f$: $$\lim_{h\to0}f(c(h))=\lim_{t\to x}f(t)=f(x)$$
>E quindi: $$\lim_{h\to0}\frac{F(x+h)-F(x)}{h}=\lim_{h\to0}f(c(h))=f(x)\quad\forall x\in(a,b)$$
>E di conseguenza: $$\exists F'(x)=f(x)\quad\forall x\in(a,b)$$


