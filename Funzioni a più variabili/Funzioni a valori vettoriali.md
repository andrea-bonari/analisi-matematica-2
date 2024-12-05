>[!note]
>Siano $n,m\in\mathbb{N}$ e $A\subseteq\mathbb{R}^{n}$ un insieme aperto. Una funzione di $n$ variabili a valori vettoriali (con $m$ componenti) è una relazione: $$\overrightarrow{f}: A\to \mathbb{R}^{m}$$
>Che associa ad ogni $n$-upla $\overrightarrow{x}=\set{x_{1},\cdots,x_{n}}\in A$ un'unica $m$-upla in $\mathbb{R}^{m}$, cioè: $$\overrightarrow{f}(\overrightarrow{x})=\begin{pmatrix}f_{1}(\overrightarrow{x})\\\vdots\\ f_{m}(\overrightarrow{x})\end{pmatrix}$$

>[!tip]
>Le funzioni $f_{1},\cdots,f_{n}$ sono funzioni di più variabili a valori reali dette componenti di $f$. $\overrightarrow{f}$ si dice anche funzione vettoriale e le $f_{i}$ funzioni (o campi) scalari.

### Limiti
>[!note]
>Siano $A\subseteq\mathbb{R}^{n}$ aperto, $\overrightarrow{f}:A\to\mathbb{R}^{n}$ e $\overrightarrow{x}_{0}\in A$. Scriviamo: $$\exists\lim_{\overrightarrow{x}\to\overrightarrow{x}_{0}}\overrightarrow{f}(\overrightarrow{x})=\overrightarrow{l}$$
>Per un vettore $l=(l_{1},\cdots,l_{m})\in\mathbb{R}^{m}$ se $\forall i\in=1,\cdots, n$ abbiamo che: $$\exists\lim_{\overrightarrow{x}\to\overrightarrow{x}_{0}}f_{i}(\overrightarrow{x})=l_{i}$$

>[!tip]
>Una funzione $\overrightarrow{f}: A\subseteq\mathbb{R}^{n}\to\mathbb{R}^{m}$ è detta:
>- continua in $\overrightarrow{x}_{0}$ se tutte le $f_{i}$ sono continue in $\overrightarrow{x}_{0}$.
>- derivabile in $\overrightarrow{x}_{0}$ se tutte le $f_{i}$ sono derivabili in $\overrightarrow{x}_{0}$.
>- differenziabile in $\overrightarrow{x}_{0}$ se tutte le $f_{i}$ sono differenziabili in $\overrightarrow{x}_{0}$
>- in $c^{1}(A;\mathbb{R})$ se tutte le $f_{i}$ sono in $c^{1}(A;\mathbb{R})$

### Matrice Jacobiana
>[!note]
>Siano $A\subseteq\mathbb{R}^{n}$ aperto, $\overrightarrow{f}:A\to\mathbb{R}^{m}$ e $\overrightarrow{x}_{0}\in A$. Se $\overrightarrow{f}$ è derivabile in $\overrightarrow{x}_{0}$, definiamo la matrice Jacobiana di $\overrightarrow{f}$ in $\overrightarrow{x}_{0}$ come la matrice $m\times n$ data da: $$J_{\overrightarrow{f}}(\overrightarrow{x}_{0})=\begin{pmatrix}\frac{\partial f_{1}}{\partial x_{1}}(\overrightarrow{x}_{0})&\cdots&\frac{\partial f_{1}}{\partial x_{n}}(\overrightarrow{x}_{0})\\\vdots&\ddots&\vdots\\ \frac{\partial f_{m}}{\partial x_{1}}(\overrightarrow{x}_{0})&\cdots&\frac{\partial f_{m}}{\partial x_{n}}(\overrightarrow{x}_{0})\end{pmatrix}$$

>[!tip]
>Nel caso $m=1$, allora $J_{f}(\overrightarrow{x}_{0})=(\nabla f(\overrightarrow{x}_{0}))^{T}$.
>Nel caso $n>1$, allora in ogni riga $i$-esima troviamo gli elementi del $\nabla f_{i}(\overrightarrow{x}_{0})$.

