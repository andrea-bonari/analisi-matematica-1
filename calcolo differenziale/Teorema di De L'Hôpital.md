>[!note]
>Siano $f,g:(a,b)\to\mathbb{R}$ derivabili in $(a,b)$ tali che $\lim\limits_{x\to a^{+}}f(x)=\lim\limits_{x\to a^{+}}g(x)=0$ e: $$\exists\lim_{x\to a^{+}}\frac{f'(x)}{g'(x)}:=l\in\mathbb{R}$$
>Allora: $$\exists\lim_{x\to a^{+}} \frac{f(x)}{g(x)}=l$$

>[!example] Dimostrazione
>Estendiamo $f$ e $g$ su tutto $[a,b)$ definendo: $$f(a)=g(a)=0$$
>Poiché: $$\begin{cases}
>\lim_{x\to a^{+}}f(a)=f(a)=0 \\
>\lim_{x\to a^{+}}g(a)=g(a)=0
>\end{cases}\Longrightarrow f,g\in C([a,b))$$
>Fissiamo quindi $a<x<b$ e consideriamo la funzione ausiliaria: $$h: [a,x]\to\mathbb{R}\qquad h(y):=f(x)g(y)-f(y)g(x)\quad\forall y\in[a,x]$$
>Si ha che $h(a)=h(x)=0$. Inoltre si ha che $f$ è derivabile in $(a,x)$ poiché $f$ e $g$ lo erano su $(a,b)$ per ipotesi.
>
>Applicando il teorema di Lagrange a $h$ su $[a,x]$: $$\exists \space y(x)\in(a,x)\quad \mathbin{/}\quad \frac{h(x)-h(a)}{x-a}=h'(y(x))$$
>Derivando $h'(x)$: $$\begin{align*}
>& h'(x)=f(x)\cdot g'(y)-f'(y)\cdot g(x) \\
>\Longrightarrow\space& 0 =f(x)g'(y(x))-f'(y(x))g(x)\\
>\Longrightarrow\space& \frac{f(x)}{g(x)}=\frac{f'(y(x))}{g'(y(x))}
>\end{align*}$$Siccome $a<y(x)<x\Longrightarrow \lim\limits_{x\to a^{+}}y(x)=a$, dalla formula precedente: $$\lim_{x\to a^{+}} \frac{f(x)}{g(x)}\lim_{x\to a^{+}}\frac{f'(y(x))}{g'(y(x))}$$
>Per il teorema del limite per funzione composta: $$\lim_{y\to a^{+}} \frac{f'(y)}{g'(y)}=l\Longrightarrow \exists\lim_{x\to a^{+}} \frac{f(x)}{g(x)}=l$$

>[!tip]
>Grazie al teorema di De L'Hôpital, definiamo i seguenti limiti e o-piccoli: $$\begin{align*}
\gamma>0&\quad\lim_{x\to+\infty} \frac{x}{e^{\gamma x}}=0&\Longrightarrow e^{\gamma x}=o(x)\\
\alpha,\beta>0&\quad\lim_{x\to+\infty} \frac{x^{\alpha}}{e^{\beta x}}=0&\Longrightarrow e^{\beta x}=o(x^\alpha)\\
&\quad\lim_{x\to+\infty} \frac{\log(x)}{x}=0&\Longrightarrow x=o(\log(x))
\end{align*}$$
