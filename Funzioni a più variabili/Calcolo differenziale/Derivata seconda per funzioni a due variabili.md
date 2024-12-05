>[!note]
>Siano $A\subseteq\mathbb{R}^{2}$ aperto e $f: A\to\mathbb{R}$ una funzione derivabile in $A$ con derivate parziali: $$\frac{\partial f}{\partial x}(x,y)\text{ e }\frac{\partial f}{\partial y}(x,y)$$
>Anch'esse derivabili in $A$. Definiamo le derivate parziali seconde di $f$ con: $$\begin{align*}
>\frac{\partial^{2} f}{\partial x^{2}}(x,y)&:=  \frac{\partial}{\partial x} \left(\frac{\partial f}{\partial x}(x,y)\right)\\
>\frac{\partial^{2} f}{\partial y\partial x}(x,y)&:=  \frac{\partial}{\partial y} \left(\frac{\partial f}{\partial x}(x,y)\right)\\
>\frac{\partial^{2} f}{\partial x\partial y}(x,y)&:=  \frac{\partial}{\partial x} \left(\frac{\partial f}{\partial y}(x,y)\right)\\
>\frac{\partial^{2} f}{\partial y^{2}}(x,y)&:=  \frac{\partial}{\partial y} \left(\frac{\partial f}{\partial y}(x,y)\right)
>\end{align*}$$

Diciamo che $f$ è derivabile due volte:
- in $(x_{0},y_{0})$ se esistono le $4$ derivate parziali seconde in $(x_{0},y_{0})$
- in $A'\subseteq A$ se $f$ è derivabile due volte in ogni $(x_{0},y_{0})\in A'$

### Matrice Hessiana
>[!note]
>Se $f$ è derivabile due volte in $(x_{0},y_{0})$, allora definiamo la matrice Hessiana di $f$ in $(x_{0},y_{0})$ come: $$H_{f}(x_{0},y_{0}):=\begin{pmatrix}\frac{\partial^{2} f}{\partial x^{2}}(x,y) & \frac{\partial^{2} f}{\partial y\partial x}(x,y) \\ \frac{\partial^{2} f}{\partial x\partial y}(x,y) & \frac{\partial^{2} f}{\partial y^{2}}(x,y) \end{pmatrix}=\begin{pmatrix} \left(\nabla \left(\frac{\partial f}{\partial x}(x_{0},y_{0})\right)\right)^{T}\\ \left(\nabla \left(\frac{\partial f}{\partial y}(x_{0},y_{0})\right)\right)^{T}\end{pmatrix}\in M_{2\times2}(\mathbb{R})$$

### Funzioni di seconda classe
>[!note]
>Se $f$ è derivabile due volte in $A$ e tutte le sue derivate parziali sono continue, allora diciamo che $f$ è di classe $c^{2}$ in $A$ e scriviamo: $$f\in c^{2}(A)$$

### Teorema di Schwarz
>[!note]
>Sia $A\subseteq\mathbb{R}^{2}$ aperto e $f\in c^{2}(A)$, allora: $$\frac{\partial^{2} f}{\partial y\partial x}(x,y)=\frac{\partial^{2} f}{\partial x\partial y}(x,y)\qquad\forall (x,y)\in A$$
>Cioè $H_{f}(x,y)$ è una matrice simmetrica $\forall(x,y)\in A$.

### Teorema della formula di Taylor al secondo ordine
>[!note]
>Siano $A\subseteq\mathbb{R}^{2}$ aperto, $f\in c^{2}(A)$, $\overrightarrow{x}_{0}\in A$. Vale la seguente formula: $$f(\overrightarrow{x}_{0}+\overrightarrow{h})=f(\overrightarrow{x}_{0})+\langle\nabla f(\overrightarrow{x}_{0}), \overrightarrow{h}\rangle + \frac{1}{2}\langle \overrightarrow{h}, H_{f}(\overrightarrow{x}_{0})\cdot \overrightarrow{h}\rangle+ o(||\overrightarrow{h}||^{2})$$
>Per $\overrightarrow{h}\to\overrightarrow{0}$. Ponendo $x_{1}=x_{1}^{0}+h_{1}$ e $x_{2}=x_{2}^{0}+h_{2}$ e considerando $\overrightarrow{x}=(x_{1},x_{2})$: $$\begin{align*}
f(\overrightarrow{x})&= f(\overrightarrow{x}_{0})+\langle\nabla f(\overrightarrow{x}_{0}), \overrightarrow{x}- \overrightarrow{x}_{0}\rangle+ \frac{1}{2}(\overrightarrow{x}-\overrightarrow{x}_{0})^{T}\cdot H_{f}(\overrightarrow{x}_{0})\cdot (\overrightarrow{x}-\overrightarrow{x}_{0})+o(||\overrightarrow{x}-\overrightarrow{x}_{0}||^{2})\\
&= f(x_{1}^{0},x_{2}^{0})+ \frac{\partial f}{\partial x_{1}}(x_{1}^{0},x_{2}^{0})(x_{1}-x_{1}^{0})+\frac{\partial f}{\partial x_{2}}(x_{1}^{0},x_{2}^{0})(x_{2}-x_{2}^{0})\\
&+ \frac{1}{2}\cdot \frac{\partial^{2} f}{\partial x_{1}^{2}}(x_{1}^{0},x_{2}^{0})(x_{1}-x_{1}^{0})^{2}+\frac{\partial^{2} f}{\partial x_{1}\partial x_{2}}(x_{1}^{0},x_{2}^{0})(x_{1}-x_{1}^{0})(x_{2}-x_{2}^{0})\\
&+ \frac{1}{2}\cdot \frac{\partial^{2} f}{\partial x_{2}^{2}}(x_{1}^{0},x_{2}^{0})(x_{2}-x_{2}^{0})^{2}+ o\left((x_{1}-x_{1}^{0})^{2}+(x_{2}-x_{2}^{0})\right) 
\end{align*}$$
Per $\overrightarrow{x}(x_{1},x_{2})\to (x_{1}^{0},x_{2}^{0})=\overrightarrow{x}_{0}$.

### Forma quadratica
>[!note]
>Sia $f\in c^{2}(A)$. Chiamiamo forma quadratica indotta della matrice Hessiana $H_{f}(\overrightarrow{x}_{0})$ per $\overrightarrow{x}_{0}\in A$ la funzione $q: \mathbb{R}^{2}\to\mathbb{R}$ definita da: $$\begin{align*}
q(h_{1},h_{2}):&= \begin{pmatrix}h_{1}\\ h_{2}\end{pmatrix}^{T}\cdot H_{f}(\overrightarrow{x}_{0})\cdot \begin{pmatrix}h_{1}\\ h_{2}\end{pmatrix}\\
&= \frac{\partial^{2} f}{\partial x_{1}^{2}}(x_{1}^{0},x_{2}^{0})h_{1}^{2}+ \frac{\partial^{2} f}{\partial x_{1}\partial x_{2}}(x_{1}^{0},x_{2}^{0})h_{1}h_{2}+ \frac{\partial^{2} f}{\partial x_{2}^{2}}(x_{1}^{0},x_{2}^{0})h_{2}^{2}
\end{align*}$$
$\forall (h_{1},h_{2})\in\mathbb{R}^{2}$, $\overrightarrow{x}_{0}=(x_{1}^{0},x_{2}^{0})$.

>[!tip] Richiami alle forme quadratiche
>Puoi vedere un richiamo alle forme quadratiche [qui](https://andrea-bonari.github.io/geometria-e-algebra-lineare/quadratiche/forme-quadratiche.html).

### Estensione a funzioni in $\mathbb{R}^{n}$
>[!note]
>Sia $A\subseteq\mathbb{R}^{n}$ aperto e sia $f: A\to\mathbb{R}$ derivabile in $A$ e tale che $\frac{\partial f}{\partial x_{1}}$ con $i=1,\cdots, n$ siano derivabili. Definiamo le derivate parziali seconde di $f$ in $\overrightarrow{x}\in A$ come: $$\frac{\partial^{2} f}{\partial x_{j} \partial x_{i}}(\overrightarrow{x})= \frac{\partial}{\partial x_{j}}\left(\frac{\partial}{\partial x_{i}}(\overrightarrow{x}) \right)\qquad \forall i,j\in\set{1,\cdots, n}$$
>E la matrice Hessiana è: $$H_{f}(\overrightarrow{x})=\begin{pmatrix} \frac{\partial^{2} f}{\partial x_{1}^{2}}(\overrightarrow{x})&\cdots & \frac{\partial^{2} f}{\partial x_{n} \partial x_{1}}(\overrightarrow{x}) \\ \vdots&\ddots&\vdots \\ \frac{\partial^{2} f}{\partial x_{1} \partial x_{n}}(\overrightarrow{x})&\cdots&\frac{\partial^{2} f}{\partial x_{n}^{2}}(\overrightarrow{x}) \end{pmatrix}$$
>Anche il teorema di Schwarz e lo sviluppo di Taylor si estendono allo stesso modo al caso $n>2$.



