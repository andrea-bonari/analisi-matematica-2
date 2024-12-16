>[!note]
>Consideriamo un integrale su insiemi $k$-dimensionali con $k>1$ che indichiamo in questo modo: $$\int_{A}f(\overrightarrow{x})\text{ d}\overrightarrow{x}$$
>Dove $\text{d}\overrightarrow{x}=\text{d}x_{1}\cdots\text{ d}x_{_{k}}$ rappresenta l'elemento di volume infinitesimale. L'integrale multiplo calcola il volume (con segno) della regione racchiusa tra il dominio $A$ della funzione e $G(f)$.
>![[Pasted image 20241206101631.png]] 

>[!tip]
>Gli integrali doppi e tripli godono delle stesse proprietà elementari degli integrali per $k=1$:
>- Linearità: $$\int_{\Omega} \left(f_{1}(\overrightarrow{x})+\lambda f_{2}(\overrightarrow{x})\right)\text{ d}\overrightarrow{x}=\int_{\Omega} f_{1}(\overrightarrow{x})\text{ d}\overrightarrow{x}+\lambda\int_{\Omega} f_{2}(\overrightarrow{x})\text{ d}\overrightarrow{x}$$
>- Monotonia: $$f\geq g\text{ in }r\Longrightarrow \int_{\Omega} f(\overrightarrow{x})\text{ d}\overrightarrow{x}\geq\int_{\Omega} g(\overrightarrow{x})\text{ d}\overrightarrow{x}$$
>- Additività: $$\int_{\Omega_{1}\cup \Omega_{2}}f(\overrightarrow{x})\text{ d}\overrightarrow{x}=\int_{\Omega_{1}}f(\overrightarrow{x})\text{ d}\overrightarrow{x}+\int_{\Omega_{2}} f(\overrightarrow{x})\text{ d}\overrightarrow{x}\quad\text{se Int}(\Omega_{1})\cap\text{Int}(\Omega_{2})\neq\emptyset$$

### Cambiamento di variabili
>[!note]
>Sia $n=2,3$. Chiamiamo cambiamento (o cambio o trasformazione) di variabili (o di coordinate) tra due regioni $U$ e $V$ contenute in $\mathbb{R}^{n}$ ogni differmorfismo $\overrightarrow{T}$ tra $U$ e $V$, ovvero ogni funzione $\overrightarrow{T}:U\to V$ tale che: $$\begin{align*}
&\overrightarrow{T}\in c^{1}(U;\mathbb{R}^{n})\\
&\exists \overrightarrow{T}^{-1}: V\to U\\
&\overrightarrow{T}^{-1}\in c^{1}(V;\mathbb{R}^{n})
\end{align*}$$

### Teorema di inversione locale
>[!note]
>Sia $\overrightarrow{f}:A\subseteq\mathbb{R}^{n}\to\mathbb{R}^{n}\in c^{1}(A;\mathbb{R}^{n})$ con $A$ aperto. Se la Jacobiana di $\overrightarrow{f}$ in $\overrightarrow{x}_{0}\in A$, cioè $\det J_{\overrightarrow{f}}(\overrightarrow{x}_{0})$, è non nullo, allora $\exists U\text{ aperto }\subseteq A$ contenente $\overrightarrow{x}_{0}$ e $V$ aperto contenente $f(\overrightarrow{x}_{0})$ tale che $f:U\to V$ è un cambiamento di variabile, e $\forall \overrightarrow{x}\in U$: $$J_{\overrightarrow{f}^{-1}}(\overrightarrow{f}(\overrightarrow{x}))= \left(J_\overrightarrow{f}(\overrightarrow{x}) \right)^{-1}$$

### Teorema di formula di integrazione con cambio di variabili
>[!note]
>Sia $\Omega\subseteq\mathbb{R}^{n}$ un dominio regolare per $n=2,3$ e sia $f$ una funzione continua. Se $\overrightarrow{T}:U\to V$ è un cambiamento di variabili tra le regioni $U$ e $V$ con $R\subseteq\overrightarrow{V}$ allora denotiamo: $$\begin{pmatrix}x_{1}\\\vdots \\x_{n}\end{pmatrix}=\overrightarrow{T}(u_{1},\cdots,u_{n})\quad\text{ o }\quad\begin{cases}
>x_{1}=T_{1}(u_{1},\cdots,u_{n})\\\vdots\\ x_{n}=T_{n}(u_{1},\cdots,u_{n})
>\end{cases}$$
>E abbiamo che: $$\begin{align*}
\left(\int\right)&\iint_{\Omega}f(x_{1},\cdots,x_{n})\text{ d}x_{1}\cdots \text{ d}{x_{n}}=\\
&=\left(\int\right)\iint_{\overrightarrow{T}^{-1}(\Omega)}f(\overrightarrow{T}(u_{1},\cdots,u_{n}))\cdot|\det J_{\overrightarrow{T}(u_{1},\cdots,u_{n})} |\text{ d}u_{1},\cdots \text{ d}u_{n}
\end{align*}$$

