>[!note]
> Sia $k\in\mathbb{N}$ e $A\subseteq\mathbb{R}^{k}:=\underbrace{\mathbb{R}\times\cdots\times\mathbb{R}}_{k}\text{ volte}$. Una funzione $f$ di $k$ variabili ha valori reali e una relazione che associa ad ogni $k$-upla $\overrightarrow{x}=(x_{1},\cdots, x_{n})\in A$ un unico numero reale $f(\overrightarrow{x})$ o $f(x_{1},\cdots, x_{k})$.
> $$f: A\subseteq \mathbb{R}^{k}\to \mathbb{R}$$
>E diciamo che $A$ è l'insieme di definizione o dominio di $f$. Il grafo di $f$ è definito come.
>$$G(f):=\set{(x_{1},\cdots,x_{k}, x_{k+1})\in \mathbb{R}^{k+1}\quad|\quad (x_{1},\cdots,x_{k})\in A, x_{k+1}=f(\overrightarrow{x})}$$

>[!tip] Osservazione
>Per $k=2$ spesso implicheremo con $(x,y)$ o $(t,s)$ invece di $(x_{1},x_{2})$

>[!note]
>Si dice insieme di livello $c\in\mathbb{R}$ della funzione: $$f:A\subseteq\mathbb{R}^{n}\to\mathbb{R}$$
>L'insieme $I_{C}:=\set{\overrightarrow{x}\in A:\quad f(\overrightarrow{x})=c}=f^{-1}(c)\subseteq A$

### Classe di una funzione
>[!note]
>Sia $I\subseteq\mathbb{R}$ un intervallo aperto. Una funzione $f:I\to\mathbb{R}$ si dice di classe:
>- $c^{0}$ su $I$, cioè $f\in c^{0}(I)$ se $f$ è continua su $I$
>- $c'$ su $I$, cioè $f\in c^{1}(I)$ se $f$ è derivabile su $I$ e $f'$ è continua su $I$
>
>Osserviamo che $f\in c^{1}(I)\Longrightarrow f\in c^{0}(I)$.
>
>Sia adesso $I\subseteq\mathbb{R}$ un intervallo aperto. Una funzione di variabile reale a valori vettoriali $$\overrightarrow{f}: I\subseteq\mathbb{R}\to\mathbb{R}^{n}$$ definita $\forall t\in I$ da: $$\overrightarrow{f}(t)=\begin{pmatrix}f_{1}(t)\\\vdots\\ f_{n}(t)\end{pmatrix}\qquad f_{i}: I\subseteq\mathbb{R}\to\mathbb{R}\quad \forall i$$
Si dice di classe $c^{\alpha}(I;\mathbb{R}^{n})$ per $\alpha=0,1$ se $f_{i}\in c^{\alpha}(I)\quad\forall i,\cdots, n$.



