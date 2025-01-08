### Integrabilità funzioni con salto
>[!note]
>Se $f:[a,b]\to\mathbb{R}$ è una funzione continua solo al più un numero finito di salti, allora è integrabile: $$f\in\mathcal{R}([a,b])$$
>È necessario spezzare l'integrale utilizzando la sua proprietà di addittività quando si integra su intervallo con salto.

### Integrale di funzioni per insiemi non limitati
>[!note]
>Sia data una funzione $f:[a,+\infty)\to\mathbb{R}$, allora $f$ è integrabile su $[a,+\infty)$ se: $$\begin{cases}
|f|\in\mathcal{R}([a,b])\quad\forall b>a \\
\exists\lim_{b\to+\infty}\int_{a}^{b}|f|\in[0,+\infty)
\end{cases}\Longrightarrow\exists\lim_{b\to+\infty}\int_{a}^{b}f=:\int_{a}^{+\infty}f$$

### Integrali di funzioni non limitate
>[!note]
>Sia $f:(a,b]\to\mathbb{R}$ integrabile su $(a,b]$, se:
>$$\begin{cases}
>\forall\varepsilon>0:\quad |f|\in\mathcal{R}([a+\varepsilon,b]) \\
>\exists\lim_{\varepsilon\to0}\int^{b}_{a+\varepsilon}|f|
>\end{cases}\Longrightarrow\exists \lim_{\varepsilon\to0^{+}}\int_{a+\varepsilon}^{b}f=:\int_{a^b}f$$


