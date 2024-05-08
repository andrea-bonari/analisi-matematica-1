### Somma di Gauss
$$\forall n\geq 1\quad 1+2+3+\cdots+n= \frac{ n\cdot(n+1)}{2}$$
>[!todo] Dimostrazione
>Sia $n_{0}=1$:
>$$P(n_{0})=P(1)= \frac{1\cdot(1+1)}{2}=1\Longrightarrow\text{vera}$$
>Verifichiamo che $P(n)\Longrightarrow P(n+1)$:
>$$\begin{align*}P(n+1)&=1+2+3+\cdots+n+ (n+1)\\&=\frac{n\cdot (n+1)}{2}+(n+1)\\&=(n+1)\cdot\left(\frac{n}{2}+1\right)\\&=\frac{(n+1)(n+2)}{2}=P(n+1)\Longrightarrow \text{vera}\end{align*}$$

### Somme geometriche
Siano $q\in\mathbb{Q}\smallsetminus\{1\}$ e $n\in\mathbb{N}$:
$$P(n)=q^{0}+q^{1}+q^{2}+q^{3}+\cdots+q^{n}= \frac{1-q^{n+1}}{1-q}$$
>[!todo] Dimostrazione
>Sia $n_{0}=1$:
>$$P(1)=\frac{1-q^{2}}{1-q}=\frac{(1+q)(1-q)}{(1-q)}=1+q^{1}\Longrightarrow\text{vera}$$
>Verifichiamo che $P(n)\Longrightarrow P(n+1)$:
>$$\begin{align*}P(n+1)&=q^{0}+q^{1}+q^{2}+\cdots+q^{n}+q^{n+1}\\&= \frac{1-q^{n+1}}{1-q}+ q^{n+1}\\&=\frac{1-q^{n+1}+q^{n+1}-q^{n+2}}{1-q}\\&=\frac{1-q^{(n+1)+1}}{1-q}=p(n+1)\Longrightarrow \text{vera}\end{align*}$$

### Disuguaglianza di Bernoulli
$$(1+x)^{n}\geq 1+nx\qquad n\geq 0\wedge x\in(-1,+\infty)$$

>[!todo] Dimostrazione
>Sia $n_{0}\in\mathbb{N}: n=0$:
>$$(1+x)^{0}=1+0x\Longrightarrow\text{vera}$$
>Verifichiamo che $P(n)\Longrightarrow P(n+1)$:
>$$\begin{align*}P(n+1)&=(1+x)^{n+1}=\underbrace{(1+x)^{n}}_{P(n)}(1+x)\\& \geq(1+nx)(1+x)\\&=1+x+nx+nx^{2}\\&=1+(n+1)x+nx^{2}\\& \Longrightarrow\text{siccome }nx^{2}\text{ è sicuramente positivo o nullo}\\&\Rightarrow (1+x)^{n+1}\geq1+(n+1)x\Longrightarrow\text{vera}
\end{align*}$$

### Binomio di Newton
Siano $a,b\in\mathbb{Q}$ e $n\geq 1$, allora:
$$(a+b)^{n}=\sum\limits_{k=0}^{n}\begin{pmatrix}n\\k\end{pmatrix}\cdot a^{k}\cdot b^{n-k}$$
>[!todo] Dimostrazione
>Sia $n_{0}=1$:
>$$(a+b)^{1}=\begin{pmatrix}1\\0\end{pmatrix}\cdot a^{0}\cdot b^{1}+\begin{pmatrix}1\\1\end{pmatrix}\cdot a^{1}\cdot b^{0}= a+ b\Longrightarrow\text{vera}$$
>Verifichiamo che $P(n)\Longrightarrow P(n+1)$
>$$\begin{align*}P(n+1)&=(a+b)^{n+1}=(a+b)^{n}\cdot(a+b)\\&= \left[\sum\limits^{n}_{k=0}\begin{pmatrix}n\\k\end{pmatrix}\cdot a^{k}\cdot b^{n-k}\right]\cdot(a+b)\\&=a\cdot\sum\limits^{n}_{k=0}\begin{pmatrix}n\\k\end{pmatrix}\cdot a^{k}\cdot b^{n-k}\quad+ b\cdot \sum\limits^{n}_{k=0}\begin{pmatrix}n\\k\end{pmatrix}\cdot a^{k}\cdot b^{n-k}\\&=\sum\limits^{n+1}_{k=0}\begin{pmatrix}n+1\\k\end{pmatrix}\cdot a^{k}\cdot b^{n+1-k}\Longrightarrow\text{vera} \end{align*}$$

### Dimostrazione necessità dei numeri reali

La motivazione che ha portato all'introduzione dei numeri reali è il fatto che ci sono alcune equazioni, come quella per trovare la diagonale del quadrato di lato 1, che non hanno soluzioni tra i numeri razionali. Ad esempio $$\nexists x\in\mathbb{Q}\quad|\quad x^{2}=2$$
>[!todo] Dimostrazione
>Consideriamo per assurdo un numero $x= \frac{m}{n}\quad |\quad x\in\mathbb{Q}$ che è soluzione di $x^{2}=2$. Allora $m^{2}$ deve essere pari perché è un quadrato, e quindi si può scrivere come $m=2\cdot p\quad,\quad p\in\mathbb{N}$, quindi. $$2=\frac{m^{2}}{n^{2}}\Longrightarrow 2\cdot n^{2}=m^{2}=(2\cdot p)^{2}=4\cdot p^{2}$$
>Sappiamo quindi che $n^{2}=2\cdot p^{2}$, per soddisfare questa condizione è necessario che $m$ e $n$ abbiano un fattore in comune, ma se così fosse si potrebbero semplificare e questo è assurdo, di conseguenza è necessario introdurre un nuovo insieme numerico chiamato reali ($\mathbb{R}$)

