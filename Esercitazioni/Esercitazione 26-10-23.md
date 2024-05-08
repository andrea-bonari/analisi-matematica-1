## Studio di funzione

1)
$$f(x)=x+ \frac{1}{\log x}$$
Dominio:
$$\begin{cases}\log x\neq 0\\x > 0\end{cases}=\begin{cases}x\neq1\\x>0\end{cases}$$
$$D: (0,1)\cap(1,+\infty)\quad;\quad f\in C(D)$$
Segno:

$$x+ \frac{1}{\log x}>0$$
$f(x)> 0 \quad\forall x>1$ perché $\frac{1}{\log x} > 0$

Se $x\in(0,1)$ abbiamo somma di 2 termini discordi $(x>0, \frac{1}{\log x}<0)$.

Limiti e eventuali asintoti:
$$\lim_{x\to0} x + \frac{1}{\log x}=0$$
=> $f$ è prolungabile per continuità in $x=0$; $\stackrel{\sim}{f}(x)=\begin{cases}f(x)&x\in D\\0&x=0\end{cases}$

$$f(x)\stackrel{x\to1}{\sim} \frac{1}{\log x}\Rightarrow\lim_{x\to1} \frac{1}{\log x}=\pm\infty$$
=> $x=1$ asintoto verticale


$$\lim_{x\to+\infty}1 + \frac{1}{\log x}= +\infty$$
$$f(x)-x= \frac{1}{\log x}\stackrel{x\to+\infty}{\to}0$$
=> $y=x$ è un asintoto obliquo

Il grafico di $f$ è sopra l'asintoto definitivamente per $x\to+\infty$

Traccio grafico probabile:
```functionplot
---
title: 
xLabel: 
yLabel: 
bounds: [-10,10,-10,10]
disableZoom: false
grid: true
---
y=x+ 1/log(x)
```

Dal grafico probabile si sa che esiste almeno un punto di minimo in $(1,+\infty)$

Derivata e studio monotonia:

$f$ sarà derivabile $\forall x\in D;\quad f\in C^{1}(D)$

$$f'(x)=Dx+ D(\log x)^{-1}=1+ (-\log x)^{-2}\cdot \frac{1}{x}=$$
$$1- \frac{1}{x(\log x)^{2}}=\frac{x(\log x)^{2}-1}{x(\log x)^{2}}$$
Denominatore sempre $>0$

$$x(\log x)^{2}-1\geq0 <=> x(\log x)^{2}\geq1$$
$$\stackrel{x>0}{<=>} (\log x)^{2}\geq \frac{1}{x}$$
$$g(x)=(\log x)^{2}$$
$$g'(x)=\frac{2\log x}{x}\geq 0\stackrel{x\geq0}{<=>} x\geq1$$

Per $(0,1)$ decrescente e per $(1,+\infty)$ crescente

```functionplot
---
title: 
xLabel: 
yLabel: 
bounds: [-10,10,-10,10]
disableZoom: false
grid: true
---
y=1/x
y=(log(x))^2
```

$$\exists\alpha\in(1,+\infty):\quad(\log\alpha)^{2}= \frac{1}{\alpha} <=> f'(\alpha)=0$$
$$f'(x)>0\quad \forall x>\alpha$$
$$f'(x)<0\quad\forall x<\alpha$$

Per stabilire il segno di $f'$ in $(0, 1)$, possiamo derivare $h(x):=x(\log x)^{2}-1$
$$h'(x)=(\log x)^{2} +2\log x \cdot \frac{1}{x}=$$
$$(\log x)(\log x+2)\geq0$$
$$<=>\log x\leq -2= x\leq e^{-2}= \frac{1}{e^{2}} \qquad x\geq1$$

$h(x)$ crescente per $(0, \frac{1}{e^{2}})$, crescente per $(\frac{1}{e^{2}},1)$ e decrescente per $(1,+\infty)$.

=> $f'(x)<0\quad\forall x\in(0,1)$


$f(x)$ è decrescente per $(0,1)$, decrescente per $(1,\alpha)$ e crescent e $(\alpha,+\infty)$

Nota: non è decrescente su $(0,1)\cap(1,\alpha)$

Grafico probabile:

$f(x)<0\quad\forall x\in(0,1)$

$$f'(e)=\frac{e\cdot1-1}{e\cdot1}=\frac{e-1}{e}>0$$
=> $\alpha\in(1,e)$

---

Definizione. $y=mx+q$ è asintoto di $f(x)$ per $x\to+\infty$ se e solo se $f(x)-(mx+q)\stackrel{x\to+\infty}{\to}0$. Se $m\neq0$ l'asintoto è detto obliquo, se $x=0$ è detto orizzontale.

Oss. $f(x)$ ammette asintoto obliquo $y=mx+q$ se e solo se: $f(x)\sim mx$ e $f(x)-mq\to q$ per $x\to+\infty$

N.B
$$f(x)\sim mx <=> \frac{f(x)}{x}\stackrel{x\to+\infty}\to m$$

2)

$$f(x)=\sqrt[3]{(x-1)^{2}(x+1)}$$
Dominio:
$$\mathbb{R}, f(x)\in C(\mathbb{R})$$

Segno/zeri:

$$f(x)=0 <=> x\pm 1$$
$$f(x)<0 <=> x< -1$$
$$f(x)>0 <=> x\in(-1,1)\cap(1,+\infty)$$

Limiti e eventuali asintoti
$$f(x)\sim \sqrt[3]{x^{2}x}\sim x$$
$$\lim_{x\to\pm\infty} \sqrt[3]{(x-1)^{2}(x+1)}=\pm\infty$$

Potrebbe esserci asintoto obliquo di coefficiente angolare $m=1$.

$$f(x)-mx=\sqrt[3]{(x^{2}-2x+1)(x+1)}-x=$$
$$=\sqrt[3]{x^{3}-x^{2}-x+1}-x=$$
$$x[(1- \frac{1}{x}- \frac{1}{x^{2}}+ \frac{1}{x^{3}})^{\frac{1}{3}}-1]\sim x \frac{1}{3}\left(-\frac{1}{x} - \frac{1}{x^{2}}+ \frac{1}{x^{3}}\right)$$
$$\sim \frac{-1}{3}$$
=> $y=x- \frac{1}{3}$ è asintoto obliquo per $f$.

Cerchiamo intersezioni con il grafico con l'asintoto

$$f(x)=x - \frac{1}{3}$$
$$x^{3}-x^{2}-x+1= x^{3}- x^{2}+ \frac{x}{3}- \frac{1}{27}$$
$$\frac{4x}{3}= \frac{28}{27}$$
$$x= \frac{7}{9}$$

In modo analogo:
$$f(x)> x- \frac{1}{3} <=> x< \frac{7}{9}$$


Derivata e studio monotonia:

Ricordiamo $g(t)=\sqrt[k]t$ non è derivabile per $t=0 (\forall k\geq2)$


