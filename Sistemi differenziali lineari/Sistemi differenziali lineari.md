>[!note]
>Un Sistema Differenziale Lineare (SDL) di ordine $n$ è un insieme di $n$ EDO lineari del primo ordine, ovvero $$\overrightarrow{y}\space'(t)=A(t)\cdot \overrightarrow{y}(t)+\overrightarrow{b}(t)\qquad t\in I$$
>Nella funzione incognita $\overrightarrow{y}:J\subseteq I\to\mathbb{R}^{n}$ con: $$\overrightarrow{y}(t)=\begin{pmatrix}y_{1}(t)\\\vdots\\y_{n}(t)\end{pmatrix}\qquad A(t)=\begin{pmatrix}a_{11}(t)&\cdots&a_{1n}(t)\\ \vdots&\ddots&\vdots\\a_{m1}(t)&\cdots&a_{mn}(t)\end{pmatrix}\qquad \overrightarrow{b}(t)=\begin{pmatrix}b_{1}(t)\\\vdots\\b_{n}(t)\end{pmatrix}$$
>Con $a_{ij},b_{i}:I\subseteq\mathbb{R}\to\mathbb{R}$.
>Se $b_{i}\equiv0\quad\forall i=1,\cdots, n$, allora il SDL è detto omogeneo, altrimenti non omogeneo o completo.

### Espressione di un EDO del secondo ordine in un SDL
>[!note] Espressione di EDO del secondo ordine in un SDL
>Sia una generica EDO del secondo ordine lineare a coefficienti costanti: $$ay''(t)+by'(t)+cy(t)=f$$
>Con $a,b,c,f\in\mathbb{R}$ e $a\neq0$. Siano $y_{1}(t):=y(t)$ e $y_{2}(t)=y'(t)$ e otteniamo: $$\begin{cases}
y_{1}'(t)=y_{2}(t) \\
y_{2}'(t)=- \frac{b}{a}y_{2}(t)- \frac{c}{a}y_{1}(t)+ \frac{f}{a}
\end{cases}$$
>O in forma matriciale: $$\overrightarrow{y}\space'(t)= A\cdot \overrightarrow{y}(x)+\overrightarrow{b}$$
>Con:
>$$\overrightarrow{y}(x):=\begin{pmatrix}
y_{1}(x) \\
y_{2}(x)
\end{pmatrix}\qquad A=\begin{pmatrix}0&1\\ - \frac{c}{a}& \frac{-b}{a}\end{pmatrix}\in M_{2\times2}\qquad \overrightarrow{b}=\begin{pmatrix}0\\ \frac{f}{a}\end{pmatrix}$$

>[!tip]
>È possibile trasformare una qualunque EDO lineare di ordine $n$ come un sistema di $n$ EDO lineari del primo ordine.

### Problema di Cauchy Associato
>[!note]
>Dato un SDL: $$\overrightarrow{y}\space'(t)=A(t)\cdot\overrightarrow{y}(t)+\overrightarrow{b}(t)$$
>Con $A:I\subseteq\mathbb{R}\to M_{n\times m}$ e $\overrightarrow{b}: I\to \mathbb{R}^{n}$ e dati $t_{0}\in I$ e $\overrightarrow{y}_{0}\in\mathbb{R}^{n}$, si chiama problema di Cauchy associato al SDL il sistema: $$\begin{cases}
\overrightarrow{y}\space'(t)=A(t)\cdot\overrightarrow{y}(t)+\overrightarrow{b}(t) \\
\overrightarrow{y}(t_{0})=\overrightarrow{y}_{0}
\end{cases}$$

>[!note] Teorema di esistenza e unicità globale per problemi di Cauchy per SDL
>Se $A: I\subseteq \mathbb{R}\to M_{n\times m}$ e $\overrightarrow{b}:i\to\mathbb{R}^{n}$ sono funzioni continue, allora il problema di Cauchy: $$\begin{cases}
\overrightarrow{y}\space'(t)=A(t)\cdot\overrightarrow{y}(t)+\overrightarrow{b}(t) \\
\overrightarrow{y}(t_{0})=\overrightarrow{y}_{0}\end{cases}$$
>Ammette un'unica soluzione definita su tutto $I$. Inoltre, se $\overrightarrow{b}\equiv0$, allora l'unica soluzione costante è la soluzione $\overrightarrow{y}(t)\equiv0$ in $I$.

>[!tip]
>Se $\overrightarrow{b}\equiv0$ e $\overrightarrow{y}_{0}=0$ nel problema di Cauchy, allora l'unica soluzione è $\overrightarrow{y}\equiv0$. Nel caso in cui $A(t)\equiv A\in M_{m\times n}$, e $\overrightarrow{b}(t)\equiv\overrightarrow{b}\in\mathbb{R}^{n}$, allora si può prendere $I=\mathbb{R}$.

### Principio di sovrapposizione
>[!note]
>Sia $A:I\subseteq\mathbb{R}\to M_{m\times n}$ e $\overrightarrow{b}_{1},\overrightarrow{b}_{2}:I\to\mathbb{R}^{n}$ continue. L'operatore $L$ definito da: $$L\overrightarrow{y}\mapsto \overrightarrow{y}\space'-A\times \overrightarrow{y}$$
>È lineare e quindi se $\exists \overrightarrow{y_{1}}\space|\quad L\overrightarrow{y}_{1}=\overrightarrow{b}_{1}$ e $\exists \overrightarrow{y_{2}}\space|\quad L\overrightarrow{y}_{2}=\overrightarrow{b}_{2}$, allora $$\forall c_{1},c_{2}\in\mathbb{R}\qquad L(c_{1}\overrightarrow{y}_{1}+c_{2}\overrightarrow{y}_{2})=c_{1}\overrightarrow{b}_{1}+c_{2}\overrightarrow{b}_{2}$$

>[!tip]
>Se $y_{1}$ e $y_{2}$ sono soluzioni dello stesso SDL omogeneo, allora una qualunque combinazione lineare ne è anche soluzione.

