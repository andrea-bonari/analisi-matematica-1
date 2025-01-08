### Criterio di integrabilità per confronto
>[!note]
>Siano $f,g:(a,b)\to\mathbb{R}$ con $-\infty\leq a<b\leq+\infty$ tali che: $$|f(x)|\leq|g(x)|\quad\forall x\in(a,b)$$
>Allora se $g\in\mathcal{R}((a,b))$ anche $f\in\mathcal{R}((a,b))$ e: $$\bigg|\int_{a}^{b}f \bigg|\leq\int_{a}^{b}|f|\leq\int_{a}^{b}|g|$$
>Inoltre se $f$ non è integrabile neanche $g$ lo è.

>[!example] Dimostrazione
>Sia $|f|\leq|g|$ su $(a,b)$. Per monotonia, se $g$ è integrabile: $$\int_{a}^{b}|f|\leq\int_{a}^{b}|g|<+\infty$$
>Viceversa, se $f$ non è integrabile: $$+\infty\leq\int_{a}^{b}|f|\leq\int_{a}^{b}|g|$$

### Criterio di integrabilità per confronto asintotico
>[!note]
>Siano $f,g:[a,+\infty)\to\mathbb{R}$ tali che: $$f(x)\sim g(x)\quad\text{ per }x\to+\infty$$
>Allora $f$ è integrabile se e solo se $g$ è integrabile.

>[!example] Dimostrazione
>Sappiamo che: $$f(x)\sim g(x)\quad\text{per }x\to+\infty \iff \lim_{x\to+\infty} \frac{f(x)}{g(x)}=1$$
>Di conseguenza: $$\forall \varepsilon>0\quad\exists N(\varepsilon)\geq a\quad |\quad x> N(\varepsilon)\Longrightarrow \bigg|\frac{f(x)}{g(x)}-1 \bigg|<\varepsilon$$
>Sappiamo quindi che: $$\begin{matrix}-\varepsilon< \frac{f(x)}{g(x)}-1<+\varepsilon \\ 1-\varepsilon< \frac{f(x)}{g(x)}<1+\varepsilon \end{matrix}$$
>Limitandoci a considerare $0<\varepsilon<1$, abbiamo che $1-\varepsilon>0$, e di conseguenza: $$0<1-\varepsilon< \frac{f(x)}{g(x)}\Longrightarrow \frac{f(x)}{g(x)}=\frac{|f(x)|}{|g(x)|}$$
>Da cui: $$\begin{align*}
>&1-\varepsilon< \frac{|f(x)|}{|g(x)|}<1+\varepsilon\\
>&(1-\varepsilon)|g(x)|<|f(x)|<(1+\varepsilon)|g(x)|
>\end{align*}$$
>Da qui se $g$ è integrabile anche $(1-\varepsilon)g$ lo è, e per il teorema del confronto anche $f$ è integrabile.
