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

>[!tip]
>Definisco la forma esponenziale di un numero complesso come $$z:=\rho\cdot e^{i\theta}=\rho(\cos\theta+i\sin\theta)$$
>
>
>È utilizzato principalmente per i prodotti, considerati $z$ e $w=r(\cos\alpha+i\sin\alpha)=r\cdot e^{i\alpha}$, il prodotto è definito come:
>$$w\cdot z=(\rho\cdot r)e^{i(\theta+\alpha)}$$
### Formule di De Moivre
>[!note] Prodotto tra numeri complessi nella notazione goniometrica (1a formula)
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

>[!tip] Elevamento a potenza di numero complesso nella notazione goniometrica
>Considero $z=\rho(\cos\theta+i\sin\theta)\in\mathbb{C}$ e $k\in\mathbb{Z}$, possiamo affermare che:
>$$z^{k}=\rho^{k}(\cos(k\theta)+i\sin(k\theta))$$E quindi possiamo dire che $$\begin{cases}
|z^{k}|=\rho^{k}=|z|^{k}\\
\text{Arg}(z^{k})=k\text{Arg}(z)\text{ con } k\neq2k\pi
\end{cases}$$

>[!note] Formula delle radici di numeri complessi (2a formula)
>Dato $w\in\mathbb{C}\smallsetminus\set{0}$ e $n\in\mathbb{N},\quad n\geq1$, allora l'equazione $$z^{n}=w$$
>Ha esattamente $n$ soluzioni distinte: $$z_{0},z_{1},\cdots,z_{n-1}\in\mathbb{C}$$
>Cioè $z_{k}^{n}=w\quad\forall k=0,\cdots, n-1$ date da: $$z_{k}=\rho_{k}\cdot\left(\cos\theta_{k}+i\sin\theta_{k}\right)$$
>Dove: $$\begin{cases}
\rho_{k}=\rho^\frac{1}{k}=\sqrt[k]{\rho} \\
\text{Arg}(z_{k})=\theta_{k}=\frac{\theta+2k\pi}{n}\qquad k=0,\cdots,n-1
\end{cases}$$

>[!example] Dimostrazione seconda formula di De Moivre
>Mostriamo che $z_{0},\cdots,z_{n-1}$ sono soluzione di $z^{n}=w$.
>$$\begin{align*}
>z_{k}^{n}&=\left(\sqrt[n]{\rho}(\cos\theta_{k}+i\sin\theta_{k})\right)^{n}\\
>&=\rho(\cos(n\theta_{k})+i\sin(n\theta_{k}))\\
>&= \rho\left(\cos\left(n\frac{\theta+2k\pi }{n}\right)+i\sin\left(n\frac{\theta+2k\pi}{n}\right)\right)\\
>&=\rho(\cos(\theta+2k\pi)+i\sin(\theta+2k\pi))\\
>&\Longrightarrow \theta+2k\pi=\theta\quad\forall k=0,\cdots,n-1\\
>&\Longrightarrow\rho(\cos\theta+i\sin\theta)=w
>\end{align*}$$
>Ogni $z_{k}$ è radice $n$-esima di $w$.
>
>Viceversa mostriamo che la lista $z_{0},\cdots,z_{n-1}$ esaurisce tutte le radici $n$-esime. Sia $z=r(\cos\alpha+i\sin \alpha)$ una radice di $z^{n}=w$ di modulo $r=|z|$ e $\text{Arg}(z)=\alpha$. Sostituiamo nell'equazione e otteniamo: $$z^{n}=r^{n}(\cos(n \alpha)+i\sin(n \alpha))=\rho(\cos\theta+i\sin\theta)=w$$
>Di conseguenza: $$\begin{cases}
r^{n}=\rho \\
n\alpha=\theta+2k\pi\quad k\in\mathbb{Z}
\end{cases}\Longrightarrow\begin{cases}
r= \rho^\frac{1}{n}=\sqrt[n]{\rho} \\
\alpha= \frac{\theta}{n}+k\cdot \frac{2\pi}{n}\quad k\in\mathbb{Z}
\end{cases}$$
>Quindi tutte le soluzioni sono date dalle formule di De Moivre.

>[!tip]
>Le radici $n$-esime di $w\in\mathbb{C}\smallsetminus\{0\}$ sono vertici di un poligono regolare di $n$ lati inscritto sulla circonferenza centrata in $0\in\mathbb{C}$ di raggio $\rho^\frac{1}{n}=|w|^\frac{1}{n}$
