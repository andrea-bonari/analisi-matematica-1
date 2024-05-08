### Sommatoria
>[!note]
>Sia $a_{n}\in\mathbb{N}$ un numero dipendente, la sommatoria $S$ viene definita come: $$S=\sum\limits_{n=n_{0}}^{m}a_{n}:=a_{n0}+a_{n1}+a_{n2}+\cdots+a_{m}$$
>Una sommatoria è detta degenere se $\exists n_{0},n_{1}:\quad n_{0}=n_{1}$

### Produttoria
>[!note]
>Sia $a_{n}\in\mathbb{N}$ un numero dipendente, la produttoria $P$ viene definita come: $$P=\prod_{n=n_{0}}^{m}a_{n}:=a_{n0}\cdot a_{n1}\cdot a_{n2}\cdot\text{ }\cdots\text{ }\cdot a_{m}$$

### Fattoriale
>[!note]
>Il fattoriale di un numero $n$ si definisce come: $$\begin{cases}
n!:=1& n=0 \\
n!:=\prod_{k=1}^{n}k=1\cdot2\cdot\text{ }\cdots\text{ }\cdot n&n\geq1
\end{cases}$$

### Coefficiente binomiale
>[!note]
>Sia $n\geq 1$ e $0\leq k\leq n$, il coefficiente binomiale "$n$ su $k$" è definito come $$\begin{pmatrix}n\\k\end{pmatrix}:= \frac{n!}{k!(n-k)!}$$

Proprietà del coefficiente binomiale:
- Proprietà 1:
$$\begin{pmatrix}n\\0\end{pmatrix}= \frac{n!}{0!(n-0)!}= \frac{n!}{n!}=1$$
- Proprietà 2:
$$\begin{pmatrix}n\\1\end{pmatrix}=\frac{n!}{1!(n-1)!}=\frac{n(n-1)!}{(n-1)!}=n$$
- Proprietà 3:
$$\begin{pmatrix}n\\k\end{pmatrix}=\begin{pmatrix}n\\n-k\end{pmatrix}$$
- Proprietà 4:
$$\begin{pmatrix}n\\k\end{pmatrix}=\begin{pmatrix}n-1\\k-1\end{pmatrix}+\begin{pmatrix}n-1\\k\end{pmatrix}$$

>[!tip]
>Siccome il coefficiente binomiale è solitamente utilizzato per individuare i coefficienti di un binomio elevato a un qualsiasi valore può essere complicato. Fortunatamente esiste il triangolo di tartaglia che può darci una mano:
>![[Pasted image 20240307145751.png]]

