>[!note]
>Siano $A\subseteq\mathbb{R}^{n}$ un insieme aperto, $\overrightarrow{x}_{0}\in A$ e $f$ una funzione a valori reali definita su $A$ (con al più il punto $\overrightarrow{x}_{0}$ mancante). Diciamo che $f$ tende al limite $l\in\mathbb{R}$ per $\overrightarrow{x}$ che tende a $\overrightarrow{x}_{0}$ e scriviamo: $$\lim_{\overrightarrow{x}\to\overrightarrow{x}_{0}}f(\overrightarrow{x})=l$$
>Se e solo se per ogni $\varepsilon>0$ esiste $\delta>0$ tale che $|f(\overrightarrow{x})-l|<\varepsilon$ per ogni $\overrightarrow{x}\in B_{\delta}(\overrightarrow{x}_{0})\smallsetminus\set{\overrightarrow{x}_{0}}$.

### Teorema per le maggiorazioni con funzioni radiali
>[!note]
>Sia $\overrightarrow{x}_{0}\in A\subseteq\mathbb{R}^{n}$ con $A$ aperto, e sia $f$ una funzione a valori reali definita su $A\smallsetminus\set{\overrightarrow{x}_{0}}$ e sia $l\in\mathbb{R}$. Se $\exists g:(0,+\infty)\to\mathbb{R}$ tale che $g(r)\to0$ per $r\to0$ e: $$|f(\overrightarrow{x})-l|\leq g(|\overrightarrow{x}-\overrightarrow{x}_{0}|)$$
>Per ogni $\overrightarrow{x}\in A\smallsetminus\set{\overrightarrow{x}_{0}}$, allora: $$\exists\lim_{\overrightarrow{x}\to\overrightarrow{x}_{0}}f(\overrightarrow{x})=l$$

### Metodo delle coordinate polari
>[!note]
>Sia $f:A\subset\mathbb{R}^{2}\to\mathbb{R}$, per valutare il limite $\lim_{\overrightarrow{x}\to\overrightarrow{x_{0}}}f(x,y)$, dove $x_{0}=\overrightarrow{0}$:
>1. Cerchiamo il candidato limite $l$ utilizzando i percorsi particolari (se troviamo candidati diversi concludiamo che il limite non esiste per l'unicità del limite).
>2. Scriviamo $f$ in coordinate polari: $$\widetilde{f}(\rho,\theta):=f(\rho \cos\theta,\rho\sin\theta)$$
>3. Troviamo $g$ del teorema maggiorando $\widetilde{f}$: $$|\underbrace{\widetilde{f}(\rho,\theta)}_\text{Passo 2}-\underbrace{l}_\text{passo 1}|\leq g(\rho)$$
>4. Verifichiamo che $\lim_{\rho\to0}g(\rho)=0$.
>5. Deduciamo quindi il limite.
>
>Se $\overrightarrow{x}_{0}\neq\overrightarrow{0}$, allora bisogna applicare i passaggi alla funzione $h(\overrightarrow{x})=f(\overrightarrow{x}-\overrightarrow{x}_{0})$.

### Limite ad infinito
>[!note]
>Sia $f:\mathbb{R}^{n}\to\mathbb{R}$. Si dice limite di $f$ per $||\overrightarrow{x}||\to\infty$ è $+\infty$ (rispettivamente $-\infty$) se $\forall k>0\quad\exists R>0$ tale che $f(\overrightarrow{x})>k$ (rispettivamente $f(\overrightarrow{x})<-k$) $\forall \overrightarrow{x}\in\mathbb{R}^{n}$ con $||\overrightarrow{x}||>R$.

### Continuità
>[!note]
>Sia $\overrightarrow{x}_{0}\in A\subseteq\mathbb{R}^{n}$ con $A$ aperto e $f:A\to\mathbb{R}$. Diciamo che $f$ è continua in $\overrightarrow{x}_{0}$ se: $$\exists \lim_{\overrightarrow{x}\to\overrightarrow{x}_{0}}f(\overrightarrow{x})=f(\overrightarrow{x}_{0})$$
>Inoltre, $f$ è continua in $A$ se $f$ è continua in ogni punto $\overrightarrow{x}_{0}\in A$.

>[!tip]
>Le funzioni elementari sono continue nel loro dominio di definizione. Se $f$ e $g$ sono continue, allora lo sono anche $f\pm g$, $f\cdot g$, $f\circ g$, se $g\neq0$ $\frac{f}{g}$, se $f>0$ $f^{g}$.

