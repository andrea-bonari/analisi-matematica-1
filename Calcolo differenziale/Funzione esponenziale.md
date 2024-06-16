>[!note]
>La funzione esponenziale (e la sua inversa logaritmo) è costruita usando la completezza dell'insieme dei numeri reali e le sue conseguenze, quali le proprietà del limite di successioni e funzioni a valori reali. Definiamo tale funzione come:
>$$e^{x}:=\lim_{n\to+\infty}\sum\limits_{k=0}^{n}\frac{x^{k}}{k!}\qquad x\in[0,+\infty)$$

### Seno e coseno iperbolico
>[!note]
>Definiamo il seno e coseno iperbolico come:
>$$\begin{align*}
&\sinh x= \frac{e^{x}-e^{-x}}{2}&&D\space\sinh x=\begin{cases}
\sinh x&n\text{ pari}\\
\cosh x&n\text{ dispari}
\end{cases}\\
&\cosh x= \frac{e^{x}+e^{-x}}{2}&&D\space\cosh x=\begin{cases}
\cosh x&n\text{ pari}\\
\sinh x&n\text{ dispari}
\end{cases}
\end{align*}$$
![[Pasted image 20240508175406.png]]

Da qui ricaviamo i valori e relazioni delle funzioni iperboliche:
- Tangente iperbolica: $$\tanh(x)=\frac{\sinh(x)}{\cosh(x)}$$
- Identità fondamentale: $$\cosh^{2}x-\sinh^{2}x=1$$
- Comportamento asintotico: $$\begin{align*}
\sinh x&\sim x\\
\cosh x-1&\sim \frac{x^{2}}{2}\\
\tanh x&\sim x 
\end{align*}$$
- Inverse: $$\begin{align*}
\sinh^{-1}x=\text{settsinh}(x)=\log\left(x+\sqrt{x^{2}+1}\right)\\
\cosh^{-1}x=\text{settcosh}(x)=\log\left(x+\sqrt{x^{2}-1}\right)
\end{align*}$$
