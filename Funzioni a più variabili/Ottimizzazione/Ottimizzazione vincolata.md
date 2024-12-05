>[!note]
>Sia $A\subseteq\mathbb{R}^{2}$ aperto e $f,F\in c^{1}(A)$. Sia $Z$ l'insieme di livello $0$ di $F$, cioè $Z=I_{0}^{F}$, o esplicitamente: $$Z=\set{(x,y)\in A:\quad F(x,y)=0}$$Che viene chiamato vincolo dell'ottimizzazione. Dato $\overrightarrow{x}_{0}=(x_{0},y_{0})\in Z$ abbiamo che:
>- $\overrightarrow{x}_{0}$ è un punto di massimo (rispettivamente di minimo) locale o relativo di $f$ vincolato a $z$ se $\exists\delta >0$ tale che: $$f(x_{0},y_{0})\geq f(x,y)\qquad(o\quad f(x_{0},y_{0})\leq f(x,y))$$ $\forall (x,y)\in B_{\delta}(\overrightarrow{x}_{0})\cap Z$ e $f(\overrightarrow{x}_{0})$ si dice massimo (rispettivamente minimo) locale o relativo di $f$ vincolato a $Z$.
>- $\overrightarrow{x}_{0}$ è un punto di massimo (rispettivamente di minimo) assoluto o globale di $f$ se: $$f(x_{0},y_{0})\geq f(x,y)\qquad(o\quad f(x_{0},y_{0})\leq f(x,y))$$ $\forall (x,y)\in Z$ e $f(\overrightarrow{x}_{0})$ si dice massimo (rispettivamente minimo) assoluto o globale di $f$ vincolato a $Z$.
>- $\overrightarrow{x}_{0}$ è un punto esternale o di estremo relativo vincolato a $Z$ se è punto di massimo o minimo locale vincolato a $Z$.
>
>SI parla di ottimizzazione vincolata di $f$ con vincolo $Z$ per indicare la ricerca dei punti esternali di $f$ vincolati a $Z$.

### Metodo per sostituzione
>[!note]
>1. Considerare la funzione $g$ di una variabile ottenuta "restringendo $f$ a $z$"
>	1. Esprimere il vincolo come curva dipendente da una delle coordinate: $y=h(x)$ e $x=h'(y)$
>	2. Definiamo $g(x)=f(x,h(x))$ o $g(y)=f(h'(y),y)$
>2. Studio la funzione $g$ come funzione in una variabile nel suo dominio e trovo i suoi punti estremali.
>3. Consideriamo tutti i punti $(x_{0},h(x_{0}))$ dove $x_{0}$ è stato trovato al passo precedente (è equivalente se avessimo esplicitato $y$ con $h'$) e valutiamo l'immagine di $f$ in tali punti.

### Teorema dei moltiplicatori di Lagrange
>[!note]
>Sia $A\subseteq\mathbb{R}^{2}$ aperto e siano $f,F\in C^{1}(A)$. Inoltre, sia $(x_{0},y_{0})\in A$ un punto di estremo di $f$ vincolato al vincolo $Z=\set{(x,y)\in A:\quad F(x,y)=0}$. Se $\nabla F(x_{0},y_{0})\neq0$, allora esiste $\lambda_{0}\in\mathbb{R}$, detto moltiplicatore di Lagrange, tale che: $$\nabla f(x_{0},y_{0})=\lambda_{0} \nabla F(x_{0},y_{0})$$

>[!tip]
>Il teorema ci fornisce una condizione necessaria per un punto ad essere punto estremale vincolato, cioè $$\nabla f(\overrightarrow{x}_{0})\parallel\nabla F(\overrightarrow{x}_{0})$$
>Inoltre, possiamo riscrivere la condizione necessaria insieme al fatto che $(x_{0},y_{0})$ è sul vincolo come un sistema non lineare nelle tre incognite $(x_{0},y_{0},\lambda_{0})$: $$\begin{cases}
>\frac{\partial f}{\partial x}(x_{0},y_{0})= \lambda_{0} \frac{\partial F}{\partial x}(x_{0},y_{0}) \\
>\frac{\partial f}{\partial y}(x_{0},y_{0})= \lambda_{0} \frac{\partial F}{\partial >y}(x_{0},y_{0}) \\
>F(x_{0},y_{0})=0
>\end{cases}$$
>In particolare, questo sistema lineare viene spesso riscritto in forma compatta come: $$\nabla L(x_{0},y_{0},\lambda_{0})=\overrightarrow{0}$$
>Dove $L$ è una funzione in $3$ variabili detta Lagrangiana definita da: $$L(x,y,\lambda):= f(x,y)- \lambda F(x,y)$$

### Vincoli con disuguaglianza
>[!note]
>Sia $f: A\subseteq \mathbb{R}^{2}\to\mathbb{R}$ definita continua su $A$ con $A$ insieme chiuso e limitato.
>
>1. Osserviamo che siccome $f$ è continua e $A$ è chiuso e limitato esistono i punti di massimo e minimo assoluti di $f$ in $A$ (teorema di Weierstrass)
>2. Escludo per il momento il bordo $\partial A$ di $A$ e considero $\text{Int}(A)$. Usando il teorema di Fermat applico quanto detto per l'ottimizzazione libera, cioè:
>	- Cerco i punti critici $P_{1},\cdots,P_{k}$ con $k\in \mathbb{N}_{0}=\mathbb{N}\cup\set{0}$ di $f$ in $\text{Int}(A)$ e eventualmente applico il criterio dell'Hessiana per classificarli.
>	- Se $f$ non è derivabile ovunque, identifico anche i punti di non derivabilità di $f$, che indico con $Q_{1},\cdots,Q_{n}$ con $n\in\mathbb{N}_{0}$
>3. Cerco i punti sul bordo di $A$ come punti estremali di $f$ vincolati al vincolo $Z=\partial A$ utilizzando le strategie dell'ottimizzazione vincolata e trovo i punti $R_{1},\cdots, R_{p}\in Z$ con $p\in\mathbb{N}_{0}$
>4. Confronto i valori delle immagini di tutti i punti trovati nei passi precedenti: $$\begin{align*}
>\max_{\overrightarrow{x}\in A} f(\overrightarrow{x})&= \max\set{f(P_{1}),\cdots, f(P_{k}),f(Q_{1}),\cdots, f(Q_{n}), f(R_{1}),\cdots, f(R_{p})}\\
>\min_{\overrightarrow{x}\in A} f(\overrightarrow{x})&= \min\set{f(P_{1}),\cdots, f(P_{k}),f(Q_{1}),\cdots, f(Q_{n}), f(R_{1}),\cdots, f(R_{p})}
>\end{align*}$$
>	E ci ricordiamo di scrivere i punti dove $f$ raggiunge il massimo e il minimo come punti di massimo e minimo, rispettivamente.

