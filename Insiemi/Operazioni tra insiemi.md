>[!note]
>Unione: $A\cup B$
>Intersezione (`and` logico): $A\cap B$
>Disgiunzione (`or` logico): $A\vee B$
>Sottrazione: $(A\setminus B):=\set{\forall a\in A\quad|\quad a\notin B}$
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
>L'insieme quoziente forma la classe di equivalenza secondo una specifica regola, l'insieme $X$ di equivalenza è l'unione fra le classi di equivalenza di tale insieme: $$X/R :=\set{x_{R}|x\in X}$$
>Si può scrivere con la notazione $$[x]_{R}:=\set{y\in X|\text{ }x\text{ in relazione con }y}\subset X$$



