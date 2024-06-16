>[!note]
>Considero una funzione $f:(a,b)\to \mathbb{R}\quad,\quad x_{0}\in(a,b)$, diremo che $f$ è derivabile in $x_{0}$ se:$$\exists\lim_{x\to x_{0}} \left(\frac{f(x)-f(x_{0})}{x-x_{0}}\right)\in\mathbb{R}$$
>Questo limite del rapporto incrementale prende il nome di derivata prima nel punto $x_{0}$ e si indica con $f'(x_{0})$.

Nel caso limite dove $x=x_{0}$, il rapporto incrementale assume il valore della tangente dell'angolo formato dalla retta tangente alla curva in $x_{0}$ e l'asse $x$.
$$f'(x)=\tan(\theta_{x})\in\mathbb{R}$$

La retta tangente è esprimibile come:
$$y-y_{0}=m(x-x_{0})\iff f(x)-f(x_{0})=f'(x_{0})\cdot(x-x_{0})$$

>[!tip]
>Se $f:(a,b)\to\mathbb{R}$ è derivabile in $x_{0}\in(a,b)$, allora esiste $R:(a,b)\to\mathbb{R}$, detta funzione resto o errore, tale che:
>$$f(x)=f(x_{0})+f'(x_{0})\cdot(x-x_{0})+R(x)\quad\forall x\in(a,b)$$
>$$\lim_{x\to x_{0}} \frac{R(x)}{x-x_{0}}=0$$

>[!example] Dimostrazione
>Definiamo $R(x):= f(x)-[f(x_{0})+f'(x_{0})\cdot(x-x_{0})]$:
>$$\begin{align*}
\lim_{x\to x_{0}}\frac{f(x)}{x-x_{0}}&=\lim_{x\to x_{0}}\frac{f(x)-f(x_{0})-f'(x_{0})(x-x_{0})}{x-x_{0}}\\
&=\left(\lim_{x\to x_{0}}\frac{f(x)-f(x_{0})}{x-x_{0}}\right)-f'(x_{0})\\
&=f'(x_{0})-f'(x_{0})=0
\end{align*}$$

### Continuità delle funzioni derivabili
>[!note]
>Se una funzione è derivabile, allora sicuramente è anche continua: $$\begin{cases}
f:(a,b)\to\mathbb{R}\quad,\quad x_{0}\in(a,b) \\
f\text{ derivabile in }x_{0}
\end{cases}\Longrightarrow f\text{ continua in }x_{0}$$

>[!example] Dimostrazione
>$$\begin{align*}
\lim_{x\to x_{0}}\bigg(f(x)-f(x_{0})\bigg)&= \lim_{x\to x_{0}}\bigg(\frac{f(x)-f(x_{0})}{x-x_{0}} \bigg)\cdot (x-x_{0})= f'(x)\cdot 0=0
\end{align*}$$
### Calcolo derivate con proprietà

Considero $f:\mathbb{R}\to\mathbb{R}\quad,\quad f(x),x\in\mathbb{R}\quad,\quad f'(x),x_{0}\in\mathbb{R}$:

1. Costante: $f(x)=c$ $$f'(x_{0})=\lim_{x\to x_{0}}0=0$$
2. Identità: $f(x)=x$ $$f'(x_{0})=\lim_{x\to x_{0}}\frac{f(x)-f(x_{0})}{x-x_{0}}=\lim_{x\to x_{0}}\frac{x-x_{0}}{x-x_{0}}=1$$
3. Parabola: $f(x)=x^{2}$ $$\lim_{x\to x_{0}}\frac{x^{2}-x_{0}^{2}}{x-x_{0}}=\lim_{x\to x_{0}}x+x_{0}=2x_{0}$$
4. Seno: $f(x)=\sin(x)$ $$f'(x)=\cos(x)$$
5. Coseno: $f(x)=\cos(x)$ $$f'(x)=-\sin(x)$$
### Regole di calcolo delle derivate
>[!note] Linearità
>La combinazione lineare di funzioni derivabili è una funzione derivabile: $$(a\cdot f+b\cdot g)'(x)=af'(x)+bg'(x)\quad a,b\in\mathbb{R}$$

>[!note] Regola di Leibniz
>$$(f\cdot g)'(x)= f'(x)\cdot g(x)+f(x)\cdot g'(x)$$

>[!note] Quoziente
>$$\left(\frac{f}{g}\right)'(x)=\frac{f'(x)\cdot g(x)-f(x)\cdot g'(x)}{[g(x)]^{2}}\quad g(x)\neq0$$

>[!note] Derivata della funzione composta
>$$(g\circ f)'(x)=g'(f(x))\cdot f'(x)$$

>[!note] Derivata della funzione inversa
>$$D[f^{-1}(y)]= \frac{1}{f'(f^{-1}(y))}$$

>[!note] Derivata di potenze
>$$f_{n}(x)=x^{n}\Longrightarrow f'_{n}(x)=n\cdot x^{n-1}\qquad\forall n\geq0\quad\forall x\in\mathbb{R}$$

### Derivate fondamentali

$$\begin{align*}
&D\space k=0&& D\space\sin x=\cos x&\\
&D\space x^{n}=nx^{n-1}&&D \space \cos x=-\sin x&\\
&D\space \frac{1}{x^{n}}=D\space x^{-n}=-nx^{-n-1}=- \frac{n}{x^{n+1}}&& D\space\tan x=1+\tan^{2}x&\\
&D\space\sqrt[n]{x} = \frac{1}{n\sqrt[n]{x^{n-1}}}&&D\space \cot x=-1-\cot^{2}x \\
&D\space\sqrt{x}=\frac{1}{2\sqrt{x}}&&D\space\arcsin x= \frac{1}{\sqrt{1-x^{2}}}\\
&D\space\log_{a}x = \frac{1}{x}\cdot \frac{1}{\ln a}&&D\space\arccos x= -\frac{1}{\sqrt{1-x^{2}}} \\
&D\space\ln x= \frac{1}{x}&&D\space\arctan x= \frac{1}{1+x^{2}}\\
&D\space a^{x}=a^{x}\ln a&& D\space\text{ arccot }x=-\frac{1}{1+x^{2}}\\
&D\space e^{x}=e^{x}&&D\space|x|= \frac{x}{|x|}= \frac{|x|}{x}
\end{align*}$$
