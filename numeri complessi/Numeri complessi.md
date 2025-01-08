>[!note]
>I numeri complessi costituiscono un insieme che estende l'insieme dei numeri reali ed in cui, a partire dalla definizione di un unità immaginaria, è possibile estrarre le radici ad indice pari di numeri negativi e risolvere le equazioni di secondo grado con discriminante negativo.
>$$\mathbb{N}\subset\mathbb{Z}\subset\mathbb{Q}\subset\mathbb{R}\subset\mathbb{C}$$

>[!example]
>$$\exists z\in\mathbb{C}\quad z\notin\mathbb{R}\quad |\quad z^{2}=-1$$

>[!note]
>Tutte le equazioni hanno soluzione nell'insieme dei numeri complessi.

Il campo complesso $\mathbb{C}$ si ottiene dal prodotto scalare fra $\mathbb{R}$ e se stesso, di conseguenza un numero complesso è rappresentato da una coppia di numeri reali:
$$\mathbb{C}=\mathbb{R}\times\mathbb{R},\qquad z=(a,b)\in\mathbb{R}$$

Possiamo rappresentare il campo complesso nel piano di Gauss, un sistema di assi ortogonali che rappresentano la parte reale $(a)$ sull'asse $x$ e la parte immaginaria ($b$) sull'asse $y$.

### Operazioni
Siano: $$\begin{align*}
z=(a,b)\in\mathbb{C} \\
w=(c,d)\in\mathbb{C}
\end{align*}$$##### Somma
$$z+w:=(a,b)+(c,d)=(a+c,b+d)$$
###### Prodotto
$$z\cdot w:=(a,b)\cdot(c,d)=(ac-bd,ad+bc)$$

### Proprietà
Siano $z,w,v\in\mathbb{C}$:
##### Commutatività
$$\begin{align*}
&z+w=w+z\\
&z\cdot w=w\cdot z
\end{align*}$$
##### Associatività
$$\begin{align*}
&z+(w+v)=(z+w)+v\\
&z\cdot(w\cdot v)=(z\cdot w)\cdot v
\end{align*}$$
##### Distributività
$$z\cdot(w+v)=z\cdot w+z\cdot v$$
##### Elemento neutro:
$$\begin{align*}
&\text{somma}:&(0,0)\\
&\text{prodotto}:&(1,0)
\end{align*}$$

### Immersione di $\mathbb{R}$ in $\mathbb{C}$
>[!note]
>Definisco la funzione di immersione dei numeri reali nell'insieme dei numeri complessi:
>$$f:\mathbb{R}\to\mathbb{C}\qquad f(x)=(x,0)\quad\forall x\in\mathbb{R}$$

Questa funzione è iniettiva.