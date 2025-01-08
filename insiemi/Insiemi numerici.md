>[!note]
>Un insieme è un raggruppamento di elementi di qualsiasi tipo che soddisfa due caratteristiche:
>1. È possibile stabilire con assoluta certezza se un elemento appartiene all'insieme
>2. Gli elementi dell'insieme sono tutti diversi tra loro
>
>In particolare, gli insiemi numerici sono dei particolari insiemi infiniti, cioè raggruppamenti di numeri formati da infiniti elementi e classificati in base a determinate caratteristiche comuni.

>[!tip]
>Alcuni insiemi numerici comuni sono:$$\begin{align*}
>\mathbb{N}&= \set{0,1,2,\cdots}\\
>\mathbb{Z}&= \set{0,\pm 1,\pm2,\cdots}\\
>\mathbb{Q}&=  \left\{ \frac{m}{n}: m,n\in\mathbb{Z}, n\neq0\right\}
>\end{align*}$$
>Inoltre esistono insiemi numerici come:
>- $\mathbb{R}$: Insieme di tutti i numeri non rappresentati nella linea dei numeri, ad esempio $\sqrt{2}$ che non è esprimibile sotto forma di frazione di interi.
>- $\mathbb{C}$: Utilizzato per trovare soluzioni ad equazioni impossibili in $\mathbb{R}$, come ad esempio $\sqrt{2}=-1$

### Operazioni tra insiemi
>[!note]
>Unione: $A\cup B$
>Intersezione (`and` logico): $A\cap B$
>Disgiunzione (`or` logico): $A\vee B$
>Sottrazione: $(A\smallsetminus B):=\set{\forall a\in A\quad|\quad a\notin B}$
>Complementare: $A\subseteq B\quad A^{C}:=\set{\forall b\in B\quad|\quad b\notin A}$
>Prodotto cartesiano: $$A\times B:=\{(a,b): a\in A, b\in B\}$$
>$$A\times A:= A^{2}$$
>![[Pasted image 20240304160224.png]]

Sia $X$ un insieme, una relazione di equivalenza su $X$ è un sottoinsieme $R$ del prodotto cartesiano di $X$ per se stesso:$$R\subset\set{X\times X}$$
Ha le seguenti proprietà:
1. Riflessività: $$(x,x)\in R\quad\forall x\in X$$
2. Transitività: $$(x,y),(y,z)\in R\Longrightarrow (x,z)\in R$$
3. Simmetricità: $$(x,y)\in R\Longrightarrow (y,x)\in R$$

>[!note] Insieme quoziente
>L'insieme quoziente forma la classe di equivalenza secondo una specifica regola, l'insieme $X$ di equivalenza è l'unione fra le classi di equivalenza di tale insieme: $$X\mathbin{ / }R :=\set{x_{R}\quad|\quad x\in X}$$
>Si può scrivere con la notazione $$[x]_{R}:=\set{y\in X\quad|\quad x\text{ in relazione con }y}\subset X$$

### Intervalli tra insiemi
>[!note]
>Dati due numeri $a,b\in\mathbb{Q}$ l'intervallo $(a,b)$ è dato da: $$(a,b):=\{x\in\mathbb{Q}:a<x<b\}$$
>L'intervallo può essere:
>- Chiuso: $(a,b):=\{x\in\mathbb{Q}:a<x<b\}$
>- Aperto: $[a,b]:=\{x\in\mathbb{Q}:a\leq x\leq b\}$
>- Misto: $[a,b):=\{x\in\mathbb{Q}:a\leq x<b\}$

### Insiemi limitati in $\mathbb{Q}$
>[!note]
>Dato un insieme $A\subset \mathbb{Q}$, esso viene definito limitato se è contenuto in un insieme $B\in \mathbb{Q}$ che include strettamente $A$:
>$$\exists A\subset B=(b_{1},b_{2})\subset\mathbb{Q}:\quad b_{1}<b_{2}\quad|\quad A\subset(b_{1},b_{2})$$
>Possiamo affermare che:
>- Tutti gli insiemi sono limitati
>- Gli insiemi $\mathbb{N}$, $\mathbb{Z}$, $\mathbb{Q}$ non sono limitati
>- Ogni insieme finito $\#(A)<\infty$ è limitato

