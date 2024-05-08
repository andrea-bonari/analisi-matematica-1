## TODO: riguardare prima ora

Esempi di stime asintotiche per $x\to0$:

$$\log(1+x)\sim x$$
$$\sin x \sim x$$
$$\tan x \sim x$$
infatti:
$$\tan x=\frac{\sin x}{x}\cdot \frac{1}{\cos x}\to 1 \cdot \frac{1}{1}= 1$$

$$1-\cos x \sim \frac{x^{2}}{2}$$
Infatti:
$$ \frac{1-\cos x}{x^{2}}= \frac{1-\cos^{2}x}{x^{2}(1+\cos x)}= (\frac{\sin x}{x})^{2}\cdot \frac{1}{1+\cos x}\to 1^{2}\cdot \frac{1}{2}= \frac{1}{2}$$
=> $$\frac{1-\cos x}{\frac{x^{2}}{2}}= 2\cdot \frac{1-\cos x}{x^{2}}?1$$

$$e^{x}-1\sim x$$
Infatti:
Da $\log(1+t)\sim t$ con $t=e^{x}-1$ si ha
$$e^{x}-1\sim \log[1+(e^{x}-1)]=\log e^{x}=x$$
Limite notevole: $$\frac{e^{x}-1}{x}\underbracket{\to}_{x\to0} 1$$


$$(1+x)^{\alpha}-1\sim\alpha x\qquad\forall\alpha\neq0$$
Infatti:
Da $\log(1+t)\sim t$ con $t=e^{x}-1$ si ha
$$(1+x)^{\alpha}-1\sim \log[1+(1+x)^{\alpha}-1]=\alpha\log(1+x)\sim \alpha x$$
Limite notevole:
$$\frac{(1+x)^{\alpha}-1}{x}\to\alpha\qquad\forall\alpha$$
Per $\alpha\neq0$ segue dalla stima asintotica
Per $\alpha=0$:$\frac{(1+x)^{0}-1}{x}= \frac{1-1}{x}=0=\alpha$

Proprietà di asintotiche
Siano $f(x)\sim f_{1}(x)$, $g(x)\sim g_{1}(x)$ per $x\to x_{0}$

a) $$f(x)g(x)\sim f_{1}(x)g_{1}(x)$$
b) $$\frac{f(x)}{g(x)}\sim \frac{f_{1}(x)}{g_{1}(x)}$$
c) $$[f(x)]^{\alpha}\sim[f_{1}(x)]^{\alpha}$$
Se $\alpha\in\mathbb{R}$ è finito e la potenza è ben definita.

d) Se $f(x)\to L\neq 1$ e $f(x)>0$ in $I(x_{0})\backslash\{x_{0}\}$
$$\log f(x)\sim \log f_{1}(x)$$

Dimostrare a),b),c) per esercizio

---
Nota bene: Può essere $L=+\infty$

d) $$\frac{\log f(x)}{\log f_{1}(x)}= \frac{\log f_{1}(x) + \log \frac{f(x)}{f_{1}(x)}}{\log f_{1}(x)}= 1+\frac{\log \frac{f(x)}{f_{1}(x)}}{\log f_{1}(x)}\to 1+ \frac{\log1}{\log L}=1+ \frac{0}{\log L}=1$$


e) Se $h(t)\to x_{0}$ per $t\to t_{0}$ con $h(t)\neq x_{0}$ in $I(t_{0})\backslash\{t_{0}\}$

$$f(h(t))\underbracket{\sim}_{t\to t_{0}} f_{1}(h(t))$$
Infatti:
$$\lim_{t\to t_{0}} \frac{f(h(t))}{f_{1}(h(t))}\underbracket{=}_{t=h(t)}\lim_{x\to x_{0}} \frac{f(x)}{f_{1}(x)}=1$$
Esempio:
$$\log(1+x^{2})\sim x^{2}\text{ per } x\to0$$
Segue da $\log(1+x)\sim x$
$$\sin \frac{1}{x}\sim \frac{1}{x}\text{ per } x\to+\infty$$
Segue da $\sin x\sim x$

Alcune proprietà che **non** valgono in generale:
- $f(x)\pm g(x)\sim f_{1}(x) \pm g_{1}(x)$
- $[f(x)]^{g(x)}\sim [f_{1}(x)]^{g(x)}$
- $h(f(x))\sim h(f_{1}(x))$
- Principio del trasporto
$$f(x)=g(x)+h(x) <=> f(x)-h(x)=g(x)$$
	- Con $\sim$ non vale mentre con $=$ vale

Altre asintotiche notevoli per $x\to 0$
$$\arcsin x\sim x\qquad\arctan x\sim x$$
Infatti: $x= \sin(\arcsin x)$
$x = \tan(\arctan x)$

Applicazioni al calcolo di limite

1) Per $x\to0$: $f(x)= \frac{\sin5x}{\tan2x}$

$$\sin(5x)\sim 5x,\qquad\tan 2x\sim 2x$$
$$f(x)\sim \frac{5x}{2x}= \frac{5}{2}\Rightarrow f(x)\to \frac{5}{2}$$
2) Per $x\to0$: $f(x)= \frac{e^{(\sin x)^{3}}-1}{\log(1-x^{3})}$
$$e^{(\sin x)^{3}}-1\sim (\sin x)^{3}\sim x^{3}$$
$$\log(1x^{3})\sim -x^{3}$$
$$f(x)\sim \frac{x^{3}}{-x^{3}}=-1$$
3) Per $m\to+\infty$: $a_{m}= \frac{m(m^{\frac{1}{m}}-1)}{\log(m^{2})}$
$$m^{\frac{1}{m}=(e^{\log m})^{\frac{1}{m}}\to}e^{0}=1$$
$$m^{\frac{1}{m}}-1\to0\Rightarrow$$
$$m^{\frac{1}{m}}-1=e^{\frac{\log m}{m}}-1\sim \frac{\log m}{m}$$
$$a_{m}\sim \frac{m \frac{\log m}{m}}{\log m^{2}}=\frac{\log m}{2\log m}=\frac{1}{2}$$