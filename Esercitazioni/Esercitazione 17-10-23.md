### Calcolo dei limiti

1)
$$\lim_{x\to-1} \frac{x^{3}+1}{x^{2}+1}= \frac{-1+1}{+1+1}=0$$
2)
$$\lim_{x\to1} \frac{x^{3}-3x+2}{x^{4}-4x+3}=\frac{0}{0}\quad FI$$
$$x^{3}-3x+2=(x+1)(x^{2}+x-2)$$
$$x^{4}-4x+3=(x+1)(x^{3}+x^{2}+x-3)$$
$$\lim_{x\to1} \frac{x^{2}+x-2}{x^{3}+x^{2}+x-3}= \frac{0}{0}\quad FI$$
$$\lim_{x\to1} \frac{x+2}{x^{2}+2x+3}= \frac{3}{6}= \frac{1}{2}$$

3)
$$\lim_{x\to0} \frac{\sqrt{1+x}-\sqrt{1-x}}{x}= \frac{1-1}{0} = \frac{0}{0}\quad FI$$
$$\frac{\sqrt{1+x}-\sqrt{1-x}}{x}\cdot \frac{\sqrt{1+x}+\sqrt{1-x}}{\sqrt{1+x}+\sqrt{1-x}}= \frac{1+x-(1-x)}{x\sqrt{1+x}+\sqrt{1-x}}=$$
$$\frac{2x}{x\sqrt{1+x}+\sqrt{1-x}}= \frac{2}{\sqrt{1+x}+\sqrt{1-x}}$$
$$\lim_{x\to0}\frac{2}{\sqrt{1+x}+\sqrt{1-x}}=\frac{2}{2}=1$$
4)
$$\lim_{x\to-\infty} xe^{\sin x}=$$
> $\sin x$ non avrà limite per $x\to-\infty$; però $\sin x$ è limitata : $-1\leq \sin x\leq+1$
> e quindi $e^{-1}\leq e^{\sin x}\leq e^{+1}$
> Possiamo supporre che $x<0$ (visto che $x\to-\infty$)
> $$\frac{x}{e} \leq xe^{\sin x}\leq xe\quad\quad(\forall x<0)$$ Ci interessa $xe^{\sin x}\leq \frac{x}{e}\to-\infty$
> Per confronto ricaviamo che:

$$\lim_{x\to-\infty}xe^{\sin x}=-\infty$$
#### Limiti notevoli legali alla gerarchia degli infiniti

Teorema.

$$\lim_{x\to+\infty} \frac{\log x}{x^{a}}=0\qquad\forall a>0$$


1)
$$\lim_{x\to+\infty} \frac{(\log x)^{b}}{x^{a}}\qquad\forall a,b>0$$

$$\frac{(\log x)^{b}}{x^{a}}= (\frac{\log x}{x^{\frac{a}{b}}})^{b}\rightarrow 0^{b}=0$$
2)
$$\lim_{x\to+\infty} \frac{x^{b}}{(e^{x})^{a}}=0\qquad\forall a,b>0$$
$$\lim_{x\to+\infty} \frac{x^{b}}{(e^{x})^{a}}\underbrace{=}_{[b=e^{x}]}\lim_{t\to+\infty} \frac{(\log t)^{b}}{t^{a}}=0\qquad\text{per 1)}$$
3)
$$\lim_{x\to+\infty} \frac{x^{b}}{(\gamma^{x})^{a}}=0\qquad\forall a,b>0,\forall\gamma>1$$
$$\frac{x^{b}}{(\gamma^{x})^{a}}= \frac{x^{b}}{(e^{\log \gamma})^{ax}}=0\qquad\text{per 2)}$$

###### Conseguenze

4)
$$\lim_{x\to0^{+}} x^{a}(\pm \log x)^{b}=0\qquad\forall a,b>0$$
Per ogni scelta del segno per cui sia ben definita $(\pm\log x)^{b}$

$$\lim_{x\to0^{+}} x^{a}(\pm\log x)^{b}\underbrace{=}_{[t= \frac{1}{x}]}\lim_{t\to+ \infty} \frac{(\pm\log t^{-1})^{b}}{t^{a}}=\lim_{t\to+ \infty} \frac{(\mp\log t)^{b}}{t^{a}}=0$$

#### Limiti notevoli legati al numero di Neplero

Ricordiamo:

$$a_{n}=(1+ \frac{1}{n})^{n}$$ è strettamente crescente con $2= a_{1}\leq a_{n}<3\qquad\forall n\geq 1$
allora segue che $a_{n}$ è convergente, con limite in $(2,3]$.

Si potrebbe poi dimostrare che il limite è $<3$ o meglio in $(2.71,2.72)$

Si pone $$e:=\lim_{n\to+\infty} (1+ \frac{1}{n})^{n}$$
Teorema
$$\lim_{x\to+\infty} (1+ \frac{1}{x})^{x}=e$$
Dimostrazione

Sia $\lfloor x\rfloor :=\max\{n\in\mathbb{Z}: n\leq x\}$
("Parte intera di $x$")

$\lfloor x\rfloor\leq x<\lfloor x\rfloor + 1\qquad \forall x\in\mathbb{Z}$

