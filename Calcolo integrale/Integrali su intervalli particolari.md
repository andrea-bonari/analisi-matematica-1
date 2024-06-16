### Integrabilità funzioni con salto
>[!note]
>Se $f:[a,b]\to\mathbb{R}$ è una funzione continua solo al più un numero finito di salti, allora è integrabile: $$f\in\mathcal{R}([a,b])$$

### Integrale di funzioni su insiemi non limitati
>[!note]
>Sia data una funzione $f:[a,+\infty)\to\mathbb{R}$, allora $f$ è integrabile su $[a,+\infty)$ se:
>- $\forall b>a:\quad |f|\in\mathcal{R}([a,b])$
>- $\exists\lim_{b\to+\infty} \int^{b}_{a}|f|$
>$f$ si dice integrabile su una semiretta e il suo integrale è definito da: $$\int^{+\infty}_{a}f:=\lim_{b\to+\infty}\int^{b}_{a}f$$

### Integrali di funzioni non limitate
>[!note]
>Sia $f:(a,b]\to\mathbb{R}$ integrabile su $(a,b]$, se:
>- $\forall\varepsilon>0:\quad |f|\in\mathcal{R}([a+\varepsilon,b])$
>- $\exists\lim_{\varepsilon\to0}\int^{b}_{a+\varepsilon}|f|$
>Allora l'integrale è definito come: $$\int^{b}_{a}f:=\lim\int^{b}_{a+\varepsilon}f$$

### Area delimitata da funzioni
>[!note]
>Per calcolare l'area delimitata dei grafici di $f(x)$ e $g(x)$ nell'intervallo $[a,b]$ vale:
>$$\int^{b}_{a}[f(x)-g(x)]\text{ d}x\qquad\iff\qquad f(x)\geq g(x)\quad\forall x\in[a,b]$$
>In caso il segno di una funzione rispettivamente all'altra vari, si scompone l'integrale in più integrali, per esempio se la funzione cambia nel punto $B$: $$\int_{a}^{c}|f(x)-g(x)|\text{ d}x=\int_{a}^{b}|f(x)-g(x)|\text{ d}x+\int_{b}^{c}|f(x)-g(x)|\text{ d}x$$
>![[Pasted image 20240520105750.png]]






