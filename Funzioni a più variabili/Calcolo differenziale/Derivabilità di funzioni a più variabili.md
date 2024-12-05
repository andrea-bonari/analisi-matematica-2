>[!note]
>Sia $A\subseteq\mathbb{R}^{n}$ aperto, $f: A\to\mathbb{R}$, $\overrightarrow{x}_{0}=(x^{0}_{1},\cdots,x_{n}^{0})\in A$. Diciamo che:
>- La derivata parziale di $f$ rispetto alla $i$-esima coordinata in $\overrightarrow{x}_{0}$ è: $$\frac{\partial f}{\partial x_{i}}(\overrightarrow{x}_{0})=\lim_{h\to0}\frac{f(x_{1}^{0},\cdots,f_{i}^{0}+h,\cdots,f_{n}^{0})-f(\overrightarrow{x}_{0})}{h}$$Perché tale limite esista finito per $i=1,\cdots,n$
>- $f$ è derivabile in $\overrightarrow{x}_{0}$ se esistono tutte le derivate $i$-esime $\frac{\partial f}{\partial x_{i}}(\overrightarrow{x}_{0})$
>- $f$ è derivabile in $A'\subseteq A$ se $f$ è derivabile in tutti i punti $\overrightarrow{x_{0}\in A'}$

La notazione per la derivata parziale è: $$\frac{\partial f}{\partial x_{i}}(\overrightarrow{x}_{0})=\partial_{x_{i}}f(\overrightarrow{x}_{0})=D_{x_{i}}f(\overrightarrow{x}_{0})=f_{x_{i}}(\overrightarrow{x}_{0})$$
>[!tip]
>Se $f$ è definita per casi è spesso necessario usare direttamente la definizione.

### Gradiente
> [!note]
> Sia $A\subseteq\mathbb{R}^{n}$ aperto, $f:A\to\mathbb{R}$, $\overrightarrow{x}_{0}=(x_{1}^{0},\cdots,x_{n}^{0})\in A$. Se $f$ è derivabile in $\overrightarrow{x}_{0}$, allora diciamo che il gradiente di $f$ in $\overrightarrow{x}_{0}$ è: $$\nabla f(\overrightarrow{x_{0}})=\begin{pmatrix} \frac{\partial f}{\partial x_{1}}\\\vdots\\\frac{\partial f}{\partial x_{n}} \end{pmatrix}\in\mathbb{R}^{n}$$
> In generale, se $f$ è derivabile in $A'\subseteq A$, allora possiamo definire la funzione gradiente $\nabla f$.

### Derivata direzionale
>[!note]
>Sia $A\subseteq\mathbb{R}^{n}$ aperto, $f: A\to\mathbb{R}$, $\overrightarrow{x}_{0}=(x_{1}^{0},\cdots,x_{n}^{0})\in A$. Sia $\overrightarrow{v}\in\mathbb{R}^{n}$ un vettore di norma unitaria. Diciamo che la derivata direzionale di $f$ in $\overrightarrow{x}_{0}$ nella direzione individuata da $v$ è: $$\frac{\partial f}{\partial \overrightarrow{v}}(\overrightarrow{x}_{0})=\lim_{t\to 0}\frac{f(\overrightarrow{x}_{0}+t\overrightarrow{v})-f(\overrightarrow{x}_{0})}{t}$$
>Dove $t\in\mathbb{R}$ con $\overrightarrow{x}_{0}+t\overrightarrow{v}\in A$, perché il limite esista finito.

### Differenziabilità per funzioni a più variabili
>[!note]
>Sia $A\subseteq\mathbb{R}^{n}$, $f:A\to\mathbb{R}$, $\overrightarrow{x}_{0}=(x_{1}^{0},\cdots,x_{n}^{0})\in A$. Diciamo che $f$ è differenziabile in $\overrightarrow{x}_{0}$ se $\exists \overrightarrow{a}\in\mathbb{R}^{n}$ tale che, ponendo $\overrightarrow{h}=(h_{1},\cdots,h_{n})$ e: $$R(h):=f(\overrightarrow{x}_{0}+h)-f(\overrightarrow{x}_{0})-\langle\overrightarrow{a},\overrightarrow{b}\rangle$$
>Si ha che: $$\lim_{\overrightarrow{h}\to\overrightarrow{0}}\frac{R(\overrightarrow{h})}{||\overrightarrow{h}||}$$
>O utilizzando la notazione o piccolo, e ponendo $\overrightarrow{x}=\overrightarrow{x}_{0}+\overrightarrow{h}$: $$f(\overrightarrow{x}_{0}+\overrightarrow{h})=f(\overrightarrow{x}_{0})+\langle\overrightarrow{a},\overrightarrow{x}-\overrightarrow{x}_{0}\rangle+o(||\overrightarrow{x}-\overrightarrow{x}_{0}||)$$
>Inoltre, possiamo verificare che tale vettore $\overrightarrow{a}\in\mathbb{R}^{n}$ coincide con $\nabla f(\overrightarrow{x}_{0})$: $$a=\nabla f(\overrightarrow{x}_{0})$$

### Teorema della condizione necessaria per la differenziabilità
>[!note]
>Sia $A\subseteq\mathbb{R}^{n}$ aperto e sia $f: A\to\mathbb{R}$ differenziabile nel punto $\overrightarrow{x}_{0}\in A$. Allora $f$ è continua in $\overrightarrow{x}_{0}$.

>[!example] Dimostrazione
>Dobbiamo dimostrare che $\exists \lim_{\overrightarrow{x}\to\overrightarrow{x}_{0}}f(\overrightarrow{x})=f(\overrightarrow{x}_{0})$. Siccome $f$ è differenziabile in $\overrightarrow{x}_{0}$, abbiamo che: $$f(\overrightarrow{x})=f(\overrightarrow{x}_{0})+\langle\nabla f(\overrightarrow{x}_{0}),\overrightarrow{x}-\overrightarrow{x}_{0}\rangle+o(||\overrightarrow{x}-\overrightarrow{x}_{0}||)$$
>E quindi: $$\begin{align*}
>0&\leq |f(\overrightarrow{x})-f (\overrightarrow{x}_{0})|=|\langle \nabla f(\overrightarrow{x}_{0}), \overrightarrow{x}-\overrightarrow{x}_{0}\rangle+o\left(||\overrightarrow{x}-\overrightarrow{x}_{0}||\right)|\\
>&\leq |\langle\nabla f(\overrightarrow{x}_{0}),\overrightarrow{x}-\overrightarrow{x}_{0}\rangle|+|o\left(||\overrightarrow{x}-\overrightarrow{x}_{0}||\right)|\\
>&= |\langle\nabla f(\overrightarrow{x}_{0}),\overrightarrow{x}-\overrightarrow{x}_{0}\rangle|+o\left(||\overrightarrow{x}-\overrightarrow{x}_{0}||\right)\\
>&\leq ||\nabla f(\overrightarrow{x}_{0})||\cdot||\overrightarrow{x}-\overrightarrow{x}_{0}||+o\left(||\overrightarrow{x}-\overrightarrow{x}_{0}||\right)
>\end{align*}$$
>Dove abbiamo usato le disuguaglianze triangolare e di Cauchy-Schwarz. Prendendo il limite per $\overrightarrow{x}\to\overrightarrow{x}_{0}$ otteniamo: $$\begin{align*}
>0&\leq\lim_{\overrightarrow{x}\to\overrightarrow{x}_{0}}|f(\overrightarrow{x}-\overrightarrow{x}_{0})|\leq\lim_{\overrightarrow{x}\to\overrightarrow{x}_{0}}\left(||\nabla f(\overrightarrow{x}_{0})||\cdot ||\overrightarrow{x}-\overrightarrow{x}_{0}|| \right)+\lim_{\overrightarrow{x}\to\overrightarrow{x}_{0}}o\left(||\overrightarrow{x}-\overrightarrow{x}_{0}||\right)\\
>&= ||\nabla f(\overrightarrow{x}_{0})||\lim_{\overrightarrow{x}\to\overrightarrow{x}_{0}}||\overrightarrow{x}-\overrightarrow{x}_{0}||+ \lim_{\overrightarrow{x}\to\overrightarrow{x}_{0}}\left(\frac{o\left(||\overrightarrow{x}-\overrightarrow{x}_{0}||\right)}{||\overrightarrow{x}-\overrightarrow{x}_{0}||}\cdot ||\overrightarrow{x}-\overrightarrow{x}_{0}||\right)=0
>\end{align*}$$
>E quindi concludiamo che: $$\exists\lim_{\overrightarrow{x}\to\overrightarrow{x}_{0}}|f(\overrightarrow{x})-f(\overrightarrow{x}_{0})|=0$$

### Classe di una funzione
>[!note]
>Sia $A\subseteq\mathbb{R}^{n}$ aperto, $f: A\to\mathbb{R}$ derivabile in $A$. Diciamo che $f$ è di classe $c^{1}$ in $A$, e scriviamo: $$f\in c^{1}(A)$$
>Se tutte le derivate parziali di $f$ esistono e sono funzioni continue in $A$.
>

### Teorema del differenziale totale
>[!note]
>Sia $A\subseteq\mathbb{R}^{n}$ e sia $f\in c^{1}(A)$. Allora $f$ è differenziabile in ogni punto di $A$, cioè: $$f\in c^{1}(A)\Longrightarrow f\text{ differenziabile in }A$$

### Teorema della formula del gradiente
>[!note]
>Sia $A\subseteq\mathbb{R}^{n}$ aperto e sia $f:A\to\mathbb{R}$ differenziabile in $\overrightarrow{x}_{0}\in A$. Allora per ogni $\overrightarrow{v}\in\mathbb{R}^{n}$ con $||\overrightarrow{v}||=1$ esiste la derivata dimensionale in $\overrightarrow{x}_{0}$ lungo la direzione $\overrightarrow{v}$ e inoltre: $$\frac{\partial f}{\partial \overrightarrow{v}}(\overrightarrow{x}_{0})=\langle\nabla f(\overrightarrow{x}_{0}),\overrightarrow{v}\rangle$$

>[!example] Dimostrazione
>Siccome $f$ è differenziabile in $\overrightarrow{x}_{0}$, abbiamo che: $$f(\overrightarrow{x}_{0}+\overrightarrow{h})= f(\overrightarrow{x}_{0})+\langle\nabla f(\overrightarrow{x}_{0}),\overrightarrow{h}\rangle+o(||\overrightarrow{h}||)$$
>per $\overrightarrow{h}\to\overrightarrow{0}$ e possiamo applicare tale equazione a $\overrightarrow{h}= t\overrightarrow{v}$ per ogni $t\in\mathbb{R}$ abbastanza piccolo: $$\begin{align*}
>f(\overrightarrow{x}_{0}+t\overrightarrow{v})&= f(\overrightarrow{x}_{0})+\langle\nabla f(\overrightarrow{x}_{0}), t\overrightarrow{v}\rangle + o(||t\overrightarrow{v}||)\\
>&= f(\overrightarrow{x}_{0}) + t\langle\nabla f(\overrightarrow{x}_{0}), \overrightarrow{v}\rangle+o(t)\\
>\end{align*}$$
>Dove abbiamo utilizzato che $||\overrightarrow{v}||=1$. Quindi abbiamo che: $$\frac{f(\overrightarrow{x}_{0}+t\overrightarrow{v})- f(\overrightarrow{x}_{0})}{t}= \frac{t\langle \nabla f(\overrightarrow{x}_{0}, \overrightarrow{v})\rangle}{t} + \frac{o(t)}{t}$$
>E concludiamo grazie a definizione di derivata direzionale che: $$\begin{align*}
\frac{\partial f}{\partial\overrightarrow{v}}(\overrightarrow{x}_{0})&= \lim_{t\to0} \frac{f(\overrightarrow{x}_{0}+t\overrightarrow{v})-f(\overrightarrow{x}_{0})}{t}\\
&= \lim_{t\to0}\space \langle \nabla f(\overrightarrow{x}_{0}), \overrightarrow{v}\rangle+\lim_{t\to0} \frac{o(t)}{t}\\
&= \langle\nabla f(\overrightarrow{x}_{0}),\overrightarrow{v}\rangle
\end{align*}$$

### Teorema della direzione di massima e minima pendenza
>[!note]
>Sia $A\subseteq\mathbb{R}^{n}$ aperto e $f: A\to\mathbb{R}$, $\overrightarrow{x}_{0}\in A$. Assumiamo che:
>- $f$ è differenziabile in $\overrightarrow{x}_{0}$
>- $\nabla f(\overrightarrow{x}_{0})\neq\overrightarrow{0}$
>
>Allora per ogni $\overrightarrow{v}\in\mathbb{R}^{n}$ con $||\overrightarrow{v}||=1$ si ha che: $$\left|\frac{\partial f}{\partial\overrightarrow{v}}(\overrightarrow{x}_{0})\right|\leq ||\nabla f(\overrightarrow{x}_{0})||$$
>E inoltre, detti: $$\overrightarrow{v}_{\max}:=\frac{\nabla f(\overrightarrow{x}_{0})}{||\nabla f(\overrightarrow{x}_{0})||}\qquad \overrightarrow{v}_{\min}:=-\frac{\nabla f(\overrightarrow{x}_{0})}{||\nabla f(\overrightarrow{x}_{0})||}$$
>Abbiamo che: $$\frac{\partial f}{\partial\overrightarrow{v}_{\max}}=||\nabla f(\overrightarrow{x}_{0})||\qquad \frac{\partial f}{\partial\overrightarrow{v}_{\min}}=-||\nabla f(\overrightarrow{x}_{0})||$$

>[!example] Dimostrazione
>Diretta conseguenza della formula del gradiente: $$\left| \frac{\partial f}{\partial\overrightarrow{v}}\right|=|\langle\nabla f(\overrightarrow{x}_{0}),\overrightarrow{v}\rangle|\leq ||\nabla f(\overrightarrow{x}_{0})||\cdot ||\overrightarrow{v}||=||\nabla f(\overrightarrow{x}_{0})||$$

### Teorema della derivazione composta 1-n-1
>[!note]
>Sia $I\subseteq\mathbb{R}$ un intervallo e $A\subseteq\mathbb{R}^{n}$ aperto. Sia $\overrightarrow{r}: I\to A$ una curva regolare e $f: A\to\mathbb{R}$ una funzione differenziabile in $A$. Detta $F: I\to \mathbb{R}$ la funzione composta definita per ogni $t\in I$ come $F(t)=(f\circ\overrightarrow{r})(t)=f(\overrightarrow{r}(t))$, abbiamo che $F$ è derivabile in $I$ e inoltre: $$F'(t)=\langle\nabla f(\overrightarrow{r}(t)), \overrightarrow{r}\space'(t)\rangle\qquad \forall t\in I$$

>[!tip]
>Possiamo vedere la derivata direzionale come la derivata di una funzione composta: sia $A\subseteq\mathbb{R}^{n}$ aperto e $f:A\to\mathbb{R}$ differenziabile in $A$, $\overrightarrow{x}_{0}\in A$ e $\overrightarrow{v}\in\mathbb{R}^{n}$ con $||\overrightarrow{v}||=1$, allora: $$\frac{\partial f}{\partial\overrightarrow{v}}(\overrightarrow{x}_{0})=F'(0)$$
>Dove $F(t):= f(x_{0}+t\overrightarrow{v})$. Infatti applicando la formula precedente a $F$: $$F'(0)=\langle \nabla f(\overrightarrow{r}(0)),\overrightarrow{r}\space'(0)\rangle=\langle \nabla f(\overrightarrow{x}_{0}),\overrightarrow{v}\rangle$$

>[!tip] Caso di funzione composta n-1-1
>Consideriamo la funzione $G:A\to\mathbb{R}$ definita da: $$G(\overrightarrow{x}):=(g\circ f)(\overrightarrow{x})=g(f(\overrightarrow{x}))$$
>Se $g$ e $f$ sono derivabili, allora $G$ è derivabile e: $$\nabla G(\overrightarrow{x})=g'(f(\overrightarrow{x}))\cdot \nabla f(\overrightarrow{x})$$

### Teorema di ortogonalità del gradiente agli insiemi di livello
>[!note]
>Sia $A\subseteq\mathbb{R}^{n}$ aperto e sia $f: A\to\mathbb{R}$ differenziabile in $A$. Supponiamo che l'insieme di livello $k\in\mathbb{R}$ di $f$, cioè: $$I_{k}:=\set{\overrightarrow{x}\in A:\quad f(\overrightarrow{x})=k}$$
>Sia il sostegno di una curva regolare $\overrightarrow{r}:I\to A$ dove $I\subseteq \mathbb{R}$ è un intervallo, abbiamo che: $$\langle \nabla f(\overrightarrow{r}(t)), \overrightarrow{r}\space'(t)\rangle =0\qquad\forall t\in I$$

>[!example] Dimostrazione
>Consideriamo la funzione $F: I\to\mathbb{R}$ definita da: $$F(t):= (f\circ\overrightarrow{r})(t)=f(\overrightarrow{r}(t))$$
>Osserviamo che: $$I_{k}:=\set{\overrightarrow{x}\in A:\quad f(\overrightarrow{x})=k}=\set{\overrightarrow{r}(t):\quad t\in I}$$
>E quindi $F(t)= f(\overrightarrow{r}(t))=k$. Abbiamo che $F$ è costante su $I$ e quindi: $$F'(t)=0\quad\forall t\in I$$
>Per il teorema di derivazione delle funzioni composte 1-n-1 abbiamo che: $$F'(t)=\langle\nabla f(\overrightarrow{r}(t)), \overrightarrow{r}\space'(t)\rangle\qquad \forall t\in I$$
>Quindi dalle due formule otteniamo che: $$0=F'(t)=\langle\nabla f(\overrightarrow{r}(t)), \overrightarrow{r}\space'(t)\rangle\qquad \forall t\in I$$

