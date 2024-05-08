## Asintotico e limiti

Siano $s_{h}x= \frac{e^{x}-e^{-x}}{2}$, $c_{h}x= \frac{e^{x}+e^{-x}}{2}$, $t_{h}x= \frac{s_{h}x}{c_{h}x}$

Verificare che per $x\to0$, risulta:
$s_{h}x\sim x\qquad c_{h}x-1\sim \frac{x^{2}}{2}\qquad t_{h}x \sim x$

a)
$$s_{h}x= \frac{e^{2x}-1}{2e^{x}}\sim \frac{2x}{x}=x$$

b)
$$c_{h}x-1= \frac{e^{x}+e^{-x}-2}{2}=\frac{e^{2x}-2e^{x}+1}{2e^{x}}=\frac{(e^{x}-1)^{2}}{2e^{x}}\sim \frac{x^{2}}{2}$$

c)
$$t_{h}x= \frac{s_{h}x}{c_{h}x}\sim \frac{x}{1}=x$$

2. Verificare che, per $x\to0$, pur essendo $\tan x\sim x$ e $\sin x\sim x$ non vale $$\tan x+x^{3}-\sin x\sim x^{3}$$ e poi determinare una stima asintotica corretta di $\tan x + x^{3}-\sin x$.
$$\frac{\tan x+x^{3}-\sin x}{x}=1+ \frac{\sin x}{x^{3}}( \frac{1}{\cos x}-1)=$$
$$=1+ \frac{\sin x}{x^{3}}\cdot\frac{1-\cos x}{\cos x}\to1+ \frac{1}{2}=\frac{3}{2}\neq 1$$

Poiché:
$$\frac{\sin x}{x^{3}}\cdot \frac{1-\cos x}{\cos x}\sim \frac{x\cdot \frac{x^{2}}{2}}{x^{3}}=\frac{1}{2}$$
Non vale $$\tan x+x^{3}-\sin x\sim x^{3}$$

---

Calcolare i limiti delle funzioni o successioni seguenti per $x$ tendente a valore indicato da volta in volta

3) per $x\to0^{+}: f(x)= \frac{\arcsin\sqrt{x}}{\cos x^{\sqrt{4}}-1}$
$$\arcsin t\sim t\Rightarrow\arcsin\sqrt{x}\sim \sqrt{x}=x^{\frac{1}{2}}$$
$$1-\cos\sim \frac{t^{2}}{2}\Rightarrow\cos x^{\frac{1}{4}}-1\sim- \frac{(x^{\frac{1}{4})^{2}}}{2}= - \frac{x^{\frac{1}{2}}}{2}$$
4) per $x\to+\infty: f(x)=x\left(e^{\frac{2x+1}{x^{2}+1}}-1\right)$

$$\frac{2x+1}{x^{2}+1}\sim \frac{2x}{x^{2}}=\frac{2}{x}\to0\Rightarrow 3^{\frac{2x+1}{x^{2+1}}}-1\to0$$
$$3^{\frac{2x+1}{x^{2+1}}}-1\to0=e^{\log_{3}\frac{2x+1}{x^{2}+1}}\sim\log_{3}\frac{2x+1}{x^{2}+1}\sim \frac{2\log 3}{x}$$
$$f(x)\sim2\log 3$$

5) per $x\to+\infty: f(x)= (x^{5}+x)^{\frac{1}{3}}+x^{\frac{5}{3}}$
$$f(x)=\left[x^{5}\left(\frac{1+ 1}{x^{4}}\right)\right]^{\frac{1}{3}}-x^{\frac{5}{3}}=x^{\frac{5}{3}}[(1+ \frac{1}{x^{4}})^{\frac{1}{3}}-1]\sim x^{\frac{5}{3}} \cdot \frac{1}{3}\cdot \frac{1}{x^{4}}= \frac{1}{3x^{\frac{7}{3}}}\to0$$
6) per $x\to0: f(x)=\frac{\sqrt{\cos x-1}}{x\sin x}$

$$\sqrt{\cos x}-1=[1+(\cos x-1)]^{\frac{1}{2}}-1\sim \frac{1}{2}(\cos x-1)\sim - \frac{x^{2}}{4}$$
$$f(x)\sim - \frac{x^{2}}{4x^{2}}= - \frac{1}{4}$$
7) per $x\to0: f(x)= \frac{(\log x)^{2}-3\log x}{\log(1+x)+(1+2\log x)^{2}}$

Per $x\to0:\qquad\log x\to-\infty$

$$(\log x)^{2}-3\log x\sim (\log x)^{2}$$
Verifica:
$$\frac{(\log x)^{2}-3\log x}{(\log x)^{2}}= 1- \frac{3}{\log x}\to 1$$
...

8) Per $x\to0: f(x)=[1+\sin(3x)]^{\frac{\cos 2x}{x}}$

Abbiamo $F.I. 1^{\infty}$


$$f(x)=\{[1+\sin 3x]^{\frac{1}{\sin 3x}}\}^{\sin 3x\cdot \frac{\cos 2x}{x}}$$
$$\lim_{x\to0}[1+\sin 3x]^{\frac{1}{\sin 3x}}=\lim_{t\to0} (1+t)^{\frac{1}{t}}=l$$

$$\sin 3x\cdot\frac{\cos 2x}{x}\sim 3x \cdot \frac{1}{x}=3$$
$$f(x)\to l^{3}$$

9) Per $x\to0^{+}: f(x)=(\sin x^{2})^{1/\log_{3}x}$

F.I $$0^{0}$$
$$f(x)=(e^{\log\sin x^{2}})^{\frac{1}{\log x}}=e^{\frac{\log\sin x^{2}}{\log_{3} x}}$$
$$\frac{\log\sin x^{2}}{\log_{3} x}\sim \frac{\log x^{2}}{\log_{3} x}=2\log 3$$
$$f(x)\to e^{2\log3}=9$$
