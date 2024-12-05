### Punti critici
>[!note]
>Sia $A\subseteq\mathbb{R}^{2}$ aperto e sia $f: A\to\mathbb{R}$ derivabile in $\overrightarrow{x}_{0}\in A$. Osserviamo che $\overrightarrow{x}_{0}$ è un punto critico se:
>- Il piano tangente è orizzontale, in quanto è dato da: $$z=f(\overrightarrow{x}_{0})+\langle \nabla f(\overrightarrow{x}_{0},\overrightarrow{x}-\overrightarrow{x}_{0})=f(\overrightarrow{x}_{0})\qquad \overrightarrow{x}\in\mathbb{R}^{2}, z\in\mathbb{R}$$
>- La formula di Taylor al secondo ordine diventa: $$f(\overrightarrow{x}_{0}+\overrightarrow{h})-f(\overrightarrow{x}_{0})= \frac{1}{2}q(\overrightarrow{h})+o(||\overrightarrow{h}||^{2})$$

>[!tip] Caso generico
>Sia $A\subseteq\mathbb{R}^{n}$ aperto e sia $f: A\to\mathbb{R}$ derivabile in $\overrightarrow{x}_{0}\in A$. Diciamo che $\overrightarrow{x}_{0}$ è un punto critico o stazionario di $f$ se: $$\nabla f(\overrightarrow{x}_{0})=0$$ 

### Punti di massimo e minimo
>[!note]
>Sia $A\subseteq\mathbb{R}^{2}$ e sia $f: A\to\mathbb{R}$. Un punto $\overrightarrow{x}=(x_{0},y_{0})$ in $A$ si dice:
>- Punto di massimo (o di minimo) locale o relativo di $f$ se $\exists\delta>0$ tale che: $$f(x_{0},y_{0})\geq f(x,y)\qquad(\text{ o }\quad f(x_{0},y_{0})\leq f(x,y))$$ $\forall (x,y)\in B_{\delta}(x_{0},y_{0})\cap A$ e $f(x_{0},y_{0})$ si dice massimo (o minimo) locale o relativo di $f$.
>- Punto di massimo (o di minimo) assoluto o globale se: $$f(x_{0},y_{0})\geq f(x,y)\qquad(\text{ o }\quad f(x_{0},y_{0})\leq f(x,y))$$ $\forall (x,y)\in A$ e $f(x_{0},y_{0})$ si dice massimo (o minimo) assoluto o globale di $f$.

>[!tip]
>Il valore del massimo (o minimo) assoluto di $f$ è unico, se esiste, mentre i punti di massimo (o minimo) assoluto possono essere molti.

### Punto estremante
>[!note]
>Se $(x_{0},y_{0})$ è un punto di massimo o minimo locale, allora è detto punto estremante o punto di estremo relativo di $f$. Inoltre, se $(x_{0},y_{0})$ è un punto critico di $f$ che non è estremante allora si dice punto di sella di $f$.

### Teorema di Weierstrass
>[!note]
>Sia $A\subseteq\mathbb{R}^{n}$ un insieme chiuso e limitato e sia $f: A\to\mathbb{R}$ una funzione continua. Allora $f$ ammette massimo e minimo assoluti in $A$, cioè $\exists \overrightarrow{x}_{m}, \overrightarrow{x}_{M}\in A$ tali che: $$f(\overrightarrow{x}_{m})\leq f(\overrightarrow{x})\leq f(\overrightarrow{x}_{M})\quad \forall x\in A$$
>E quindi ne segue che $f$ è limitata.

### Teorema degli zeri
>[!note]
>Sia $A$ un insieme connesso per archi in $\mathbb{R}^{n}$ e sia $f: A\to\mathbb{R}$ continua. Se $f(\overrightarrow{x})>0$ e $f(\overrightarrow{y})<0$ per due punti $\overrightarrow{x}$ e $\overrightarrow{y}$ in $A$, allora $\exists \overrightarrow{z}\in A$ tale che $f(\overrightarrow{z})=0$.

