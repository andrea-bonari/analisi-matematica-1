### Numeri complessi (seguito)

Risolvere in $\mathbb{C}$ le seguenti espressioni

1) $z^{6}+(2-i)z^{3}+i-1=0$

Equazioni di tipo $P(0)=0$ con $P$ polinomio => $\exists$ almeno una soluzione; inoltre si può dire che le soluzioni sono esattamente $6$ (grado di $P$), se contate con la molteplicità.

$$P(z)=\prod_{n=1}^{6}(z-z_{n})$$ dove $z_{1},...,z_{6}$ sono soluzioni di $P(z)=0$
(teorema fondamentale dell'algebra)

Poniamo $w=z^{3}$ e riscriviamo l'equazione come:

$$w^{2}+(2-i)w+1-i=0$$
$$\triangle=(2-i)^{2}-4(1-i)=4-4i-4+4i-1=-1$$
$$w=\frac{-2+i\pm i}{2}=\begin{matrix}w_{1}= \frac{-2+2i}{2}=-1+i\\w_{2}=-1\end{matrix}$$
$$z^{3}=w_{1}=-1+i=\sqrt2(\cos \frac{3}{4}\pi+i\sin \frac{3}{4}\pi)$$
$$z_{k}=\sqrt[3]{\sqrt2}(\cos \frac{\frac{3\pi}{4}+2k\pi}{3}+i\sin \frac{\frac{3\pi}{4}+2k\pi}{3})$$
$$z_{0}=\sqrt[6]{2}(\cos \frac{\pi}{4}+i\sin \frac{\pi}{4})=\sqrt[6]{2}(\frac{1}{\sqrt2}+i \frac{1}{\sqrt2})=$$
$$=2^{\frac{1}{6}}(2^{- \frac{1}{2}}+i2^{- \frac{1}{2}})= 1+i/\sqrt[3]{2 }$$
$$z_{1}=\sqrt[6]{2}(\cos \frac{11\pi}{12}+i \frac{11\pi}{12})=2^{\frac{1}{6}}\cos \frac{11\pi}{12}+i2^{\frac{1}{6}}\sin \frac{11\pi}{12}$$
$$z_{2}=2^{\frac{1}{6}}(\cos \frac{19\pi}{12} +i\sin \frac{19\pi}{12})=$$
Osservazione: Si può dimostrare che $\forall z=x+iy (x,y\in\mathbb{R}): e^{z}=e^{x}(\cos y+i\sin y)$

E quindi se poniamo $x=0: e^{iy}=\cos y+i\sin y$
(identità di eulero).

Quindi invece di scrivere
$$\rho(\cos\theta+i\sin\theta)\Rightarrow \rho e^{iy}$$
Questa è detta notazione esponenziale.

---

$$z=z^{\frac{1}{6}}e^{\frac{19\pi}{12}i}$$
$$z^{3}=w_{"}=-1=1e^{\pi i}$$
$$z=\sqrt[3]{1}e^{\frac{\pi+2k\pi}{3}i}$$
$$z_{3}=e^{\frac{\pi}{3}i}$$
$$z_{4}=e^{\pi i}=-1$$
$$z_{5}=e^{\frac{5\pi}{3}i}=\frac{1}{2}-i \frac{\sqrt3}{2}$$


2) $$z^{2}-(5+3i)z+10+5i=0$$

$$\triangle=(5+3i)^{2}-40-20i=25+30i-9-40-20i=-24+10i$$
Per calcolare le radici $w=x+iy (x,y\in\mathbb{R})$
di $\triangle$ scriviamo: $$w^{2}=-24+10i$$
$x^{2}-y^{2}+2xyi=-24+10i$

$$\begin{cases}x^{2}-y^{2}=-24\\2xy=10\end{cases}$$

Possiamo supporre $y\neq0$ (altrimenti la seconda eq. avrebbe $0=10$)

$$\begin{cases}x= \frac{5}{y}\\ \frac{25}{y^{2}}-y^{2}+24=0\end{cases}$$
$$\begin{cases}x= \frac{5}{y}\\y^{4}-24y^{2}-25=0\end{cases}$$
$$\begin{cases}x= \frac{5}{y}\\(y^{2}-25)(y^{2}+1)=0\end{cases}$$
$$\begin{cases}x= \frac{5}{y}\\y=\pm 5\end{cases}$$
$$[N.B.\quad y^{2}+1\neq0\quad\forall y\in\mathbb{R}]$$
$$\begin{cases}x=\pm 1\\y=\pm 5\end{cases}$$
$$\sqrt\triangle=\pm(1+5i)$$
Le soluzioni dell'equazioni sono:

$$z_{1}= \frac{5+3i+1+5i}{2}= \frac{6+8i}{2}=3+4i$$
$$z_{2}= \frac{4-2i}{2}=2-i$$


Da fare:
$$z^{2}-z\cdot\overline{z}-2z+4=0$$
$$z^{3}=i\overline{z}|z|$$