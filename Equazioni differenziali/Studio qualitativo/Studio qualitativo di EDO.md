### Teorema di Peano (o di esistenza locale)
>[!note]
>Siano $A=I\times B\subseteq \mathbb{R}^{2}$ con $I$ intervallo aperto e $B$ insieme aperto, $\overrightarrow{x}_{0}=(x_{0},y_{0})\in A$ e $f:A\to\mathbb{R}$ continua. Allora il problema di Cauchy: $$\begin{cases}
>y'(x)=f(x,y(x))\quad x\in I \\
>y(x_{0})=y_{0}
>\end{cases}$$
>Ammette una soluzione $y\in c^{1}(J)$ definita su un intervallo $J\subseteq I$ con $x_{0}\in J$.

### Teorema di Cauchy (o di esistenza unica locale)
>[!note]
>Siano $A=I\times B\subseteq\mathbb{R}^{2}$ con $I$ intervallo aperto e $B$ insieme aperto, $\overrightarrow{x}_{0}=(x_{0},y_{0})\in A$ e $f:A\to\mathbb{R}$ continua. Se inoltre $\exists\delta>0$ tale che $\frac{\partial f}{\partial y}$ esiste ed è continua in $B_{\delta}(\overrightarrow{x}_{0})$, allora il problema di Cauchy ammette una soluzione $y\in c^{1}(J)$ definita su un intervallo $J\subseteq I$ con $x_{0}\in J$ che si può prendere sufficientemente piccolo per avere che $y$ è anche l'unica soluzione in $B_{\delta}(\overrightarrow{x}_{0})$.

### Teorema di esistenza e unicità globale
>[!note]
>Consideriamo il problema di Cauchy: $$\begin{cases}
>y'(x)=f(x,y(x))\quad x\in I \\
>y(x_{0})=y_{0}
>\end{cases}$$
>sulla striscia $A=(\lambda,\beta)\times\mathbb{R}$ con $-\infty\leq\lambda<\beta\leq+\infty$, con $f\in c^{0}(A)$ tale che $\exists \frac{\partial f}{\partial y}\in c^{0}(A)$ e sia $y:J\to\mathbb{R}$ la sua unica soluzione con $J$ intervallo massimale di definizione (cioè non ulteriormente prolungabile). Abbiamo che:
>- Se esistono due costanti $k_{1},k_{2}\geq0$ tali che: $$|f(x,y)|\leq k_{1}+k_{2}|y|\quad\forall(x,y)\in A$$allora $J=(\lambda,\beta)$
>- Se $y$ è limitata su $J$, allora $J=(\lambda,\beta)$.

