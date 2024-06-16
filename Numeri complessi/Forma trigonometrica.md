>[!note]
>Considero un numero complesso $z\neq0\Longrightarrow|z|\neq0$
>$$z=|z|\cdot \frac{\bar{z}}{|z|}=\rho\cdot w=\begin{cases}
\rho=|z|&\text{modulo} \\
w= \frac{\bar{z}}{|z|}&\text{angolo}
\end{cases}$$
Il numero complesso completo sarà quindi $$z=\rho(\cos\theta+i\sin\theta)$$

Definisco l'argomento come $\text{Arg}(z)=\theta$

>[!tip]
>Possiamo ricavare le seguenti formule:
>$$\begin{align*}
&\cos\theta=\frac{\text{Re}(z)}{|z|}\\
&\sin\theta=\frac{\text{Im}(z)}{|z|}\\
&\tan\theta=\tan(\text{Arg(z)})=\frac{\text{Im}(z)}{\text{Re}(z)}\\
&\cot\theta=\cot(\text{Arg(z)})=\frac{\text{Re}(z)}{\text{Im}(z)}  
\end{align*}$$

### Formule di De Moivre

>[!note] Prodotto tra numeri complessi nella notazione goniometrica
>Considerati i due numeri $z_{1}=\rho_{1}(\cos\theta_{1}+i\sin\theta_{1})\in\mathbb{C}$ e $z_{2}=\rho_{2}(\cos\theta_{2}+i\sin\theta_{2})\in\mathbb{C}$ possiamo affermare che:
>$$z_{1}\cdot z_{2}=(\rho_{1}\cdot \rho_{2})\cdot\left( \cos(\theta_{1}+\theta_{2})+i\sin(\theta_{1}+\theta_{2}) \right)$$
>
>E quindi possiamo dire che $$\begin{cases}
|z_{1}\cdot z_{2}|=\rho_{1}\cdot\rho_{2}\\
\text{Arg}(z_{1}\cdot z_{2})=\theta_{1}+\theta_{2}=\text{Arg}(z_{1})+\text{Arg}(z_{2})
\end{cases}$$

>[!example] Dimostrazione
>Considerati i due numeri $z_{1}=\rho_{1}(\cos\theta_{1}+i\sin\theta_{1})\in\mathbb{C}$ e $z_{2}=\rho_{2}(\cos\theta_{2}+i\sin\theta_{2})\in\mathbb{C}$
>$$\begin{align*}
z_{1}\cdot z_{2}&=\rho_{1}(\cos\theta_{1}+i\sin\theta_{1})\cdot\rho_{2}(\cos\theta_{2}+i\sin\theta_{2})\\
&=(\rho_{1}\cdot\rho_{2})(\cos\theta_{1}\cdot\cos\theta_{2}+\cos\theta_{1}i\sin\theta_{2}+i\sin\theta_{1}\cos\theta_{2}-\sin\theta_{1}\sin\theta_{2})\\
&=(\rho_{1}\cdot\rho_{2})(\cos(\theta_{1}+\theta_{2})+i\sin(\theta_{1}+\theta_{2}))
\end{align*}$$

>[!note] Elevamento a potenza di numero complesso nella notazione goniometrica
>Considero $z=\rho(\cos\theta+i\sin\theta)\in\mathbb{C}$ e $k\in\mathbb{Z}$, possiamo affermare che:
>$$z^{k}=\rho^{k}(\cos(k\theta)+i\sin(k\theta))$$E quindi possiamo dire che $$\begin{cases}
|z^{k}|=\rho^{k}=|z|^{k}\\
\text{Arg}(z^{k})=k\text{Arg}(z)\text{ con } k\neq2k\pi
\end{cases}$$

>[!example] Dimostrazione seconda formula di De Moivre
>Considero un numero $w\in\mathbb{C}\smallsetminus\{0\}$ e $n\geq 1, n\in\mathbb{N}$, allora l'equazione $$z^{n}=w$$ha esattamente $n$ soluzioni $z_{0},z_{1},\cdots,z_{n-1 }\in\mathbb{C}$, cioè:
>$$w_{k}=\sqrt[n]{z_{k}}= z^{\frac{1}{n}}_{k}$$
>Che sono date da $z_{k}=\rho^{n}(\cos(k\theta)+i\sin(k\theta))$
>Di conseguenza abbiamo che $$\begin{cases}
\text{Arg}(z_{k})=\theta_{k}= \frac{\theta+2k\pi}{n} \\
|z_{k}|=\sqrt[n]{\rho}=\rho^{\frac{1}{n}}
\end{cases}$$
> - Verifichiamo le $z_{k}$ radici:
>   
> $$\begin{align*}
z_{k}^{n}&=\left(\sqrt[n]{\rho}(\cos\theta_{k}+i\sin\theta_{k})\right)^{n}\\
&=\rho(\cos(n\theta_{k})+i\sin(n\theta_{k}))\\
&=\rho(\cos(\theta+2k\pi)+i\sin(\theta+2k\pi))\\
&=\rho(\cos\theta+i\sin\theta)=w\Longrightarrow\forall k=0,1,\cdots,n-1
\end{align*}$$
> - Verifichiamo che non ci siano radici oltre alle $z_{k}$:
>
>Supponiamo che esista $z=v(\cos\alpha+i\sin\alpha)$ e che sia soluzione di $z^{n}=w$, il numero complesso $z$ ha modulo $|z|=v>0$ e angolo $\text{Arg}(z)=\alpha$. Allora: $$(v(\cos\alpha+i\sin\alpha))^{n}=\rho(\cos\theta+i\sin\theta)$$
>Che corrisponde a $$\begin{align*}&v^{n}(\cos(n\alpha)+i\sin(n\alpha))=\rho(\cos\theta+i\sin\theta)\\
&\Longrightarrow v^{n}=\rho\Longrightarrow v= \sqrt[n]{\rho }
\end{align*}$$
Di conseguenza $$n\alpha=\theta+2k\pi\Longrightarrow\alpha=\text{Arg}(z)$$$k$ è sovrabbondante perché per $k>n-1$ si aggiunge un angolo giro, e quindi non si creano nuove soluzioni $$\Longrightarrow 0\leq k\leq n-1$$.
Si raggiunge quindi la formula $$\text{Arg}(z_{k})=\theta_{k}= \frac{\theta+2k\pi}{n}$$

>[!tip]
>Le radici $n$-esime di $w\in\mathbb{C}\smallsetminus\{0\}$ sono vertici di un poligono regolare di $n$ lati inscritto sulla circonferenza centrata in $0\in\mathbb{C}$ di raggio $\rho^\frac{1}{n}=|w|^\frac{1}{n}$
