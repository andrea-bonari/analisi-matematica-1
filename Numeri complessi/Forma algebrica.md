>[!note]
>Considero un numero $z=(a,b)\in\mathbb{C}$:
>Ricaviamo quindi: $$(a,b)=a+ib$$ dove l'unità immaginaria $i$ equivale a $(0,1)$.

>[!example] Dimostrazione
>$$\begin{align*}
(a,b)&=(a,0)+(0,b)=a+(0,b)=a+(0,1)\cdot(b,0)\\
&=a+(0,1)b=a+ib
\end{align*}$$

>[!tip] Proprietà dell'unità immaginaria
>$$\begin{align*}
&i^{1}=i\\
&i^{2}=-1\\
&i^{3}=-i\\
&i^{4}=1
\end{align*}$$
Questi valori si ripetono ciclicamente con un periodo di $2\pi$

Posso distinguere due parti che compongono il numero complesso, consideriamo $z=a+ib$:
- Parte reale: $\text{Re}(z):=a\qquad a\in\mathbb{R}$
- Pare immaginaria: $\text{Im}(z):=b\qquad b\in\mathbb{R}$

Di conseguenza possiamo scrivere $$z=\text{Re}(z)+i\cdot \text{Im}(z)$$

### Operazioni in forma algebrica
##### Somma
$$z+w=(a+c)+i\cdot(b+d)$$
##### Prodotto
$$z\cdot w=(a+i\cdot b)(c+i\cdot d)=(ac-bd)+i(ad+bc)$$

### Opposto, inverso e coniugato

Definiamo $z=(a,b)$
##### Opposto
$$(-a,-b)$$
##### Coniugato
simmetria rispetto l'asse $x$ (reale):
$$\bar{z}=a-ib=\begin{cases}
\text{Re}(\bar{z})=&\text{Re}(z)&=a \\
\text{Im}(\bar{z})=&-\text{Im}(z)&=-b
\end{cases}$$
##### Inverso
$$w:=\left( \frac{a}{a^{2}+b^{2}}, \frac{b}{a^{2}+b^{2}} \right)$$

>[!tip]
>Un numero complesso è uguale al suo coniugato solo quando è reale: $$z=\bar{z}\iff z\in\mathbb{R}$$

>[!tip]
>Vengono definiti numeri immaginari puri quelli che hanno $\text{Re}(z)=0$, l'opposto di un numero immaginario puro è pari al suo coniugato $\bar{z}=-z\iff\text{Re}(z)=0$

### Modulo
>[!note] 
>Considero un numero immaginario $z=a+ib$, il suo modulo è:
$$|z|:=\sqrt{a^{2}+b^{2}}$$
Dal punto di vista geometrico il modulo corrisponde alla distanza fra l'origine degli assi $(0,0)$ e il punto $z=(a,b)$

Dal punto di vista geometrico il modulo di una differenza $|z-w|$ corrisponde alla distanza fra i due punti nel piano di Gauss.

##### Proprietà
- Simmetria rispetto al centro: $|z|=|-z|$
- Simmetria rispetto all'asse reale: $|\bar{z}|=|z|$
- $\bar{z}+\bar{w}=z+w$
- $\bar{z}\cdot\bar{w}=z\cdot w$
- $|z|=\sqrt{z\cdot\bar{z}}\Longrightarrow |z|^{2}=z\cdot\bar{z}$
- Disuguaglianza triangolare: $|z+w|\leq|z|+|w|$
