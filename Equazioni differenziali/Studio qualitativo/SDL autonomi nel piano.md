>[!note]
>Un sistema differenziale autonomo di ordine $2$ è un sistema differenziale della forma: $$\overrightarrow{y}(t)=\overrightarrow{f}(\overrightarrow{y}(t))\iff\begin{cases}
>y'_{1}(t)=f_{1}(y_{1}(t),y_{2}(t)) \\
>y'_{2}(t)=f_{2}(y_{1}(t),y_{2}(t))
>\end{cases}$$
>Con $\overrightarrow{f}:D\subseteq \mathbb{R}^{2}\to\mathbb{R}^{2}$: $$\overrightarrow{f}(\overrightarrow{y}):=\begin{pmatrix}f_{1}(\overrightarrow{y})\\f_{2}(\overrightarrow{y})\end{pmatrix}$$

>[!tip]
>Come per le EDO del primo ordine autonome abbiamo che se $\overrightarrow{y}(t)$ è soluzione, allora $\overrightarrow{z}_{c}:=\overrightarrow{y}(x+c)$ è soluzione $\forall c\in\mathbb{R}$.

### Orbite, diagramma delle fasi e punti di equilibrio
>[!note]
>L'orbita (o traiettoria) di una soluzione $\overrightarrow{y}$ è l'immagine nel piano $y_{1}Oy_{2}$ delle soluzioni nel loro intervallo di esistenza.
>Il diagramma delle fasi è il piano $y_{1}Oy_{2}$ con le orbite delle soluzioni.
>I punti di equilibrio sono $\overrightarrow{\overline{y}}=(\overline{y}_{1},\overline{y}_{2})\in\mathbb{R}^{2}$ tale che $\overrightarrow{f}(\overrightarrow{\overline{y}})=\overrightarrow{0}$.
>![[Pasted image 20241216180743.png]]

>[!tip]
>Siccome $\det A\neq0$ l'unico punto di equilibrio è l'origine $\overrightarrow{0}$. Nel piano delle fasi vi sono infinite orbite che riempiono tutto il piano. Le orbite non si intersecano.

Studiando la stabilità dell'origine per gli SDL autonomi abbiamo 8 casi diversi rispetto agli autovalori $\lambda_{1}$ e $\lambda_{2}$ di $A$.

>[!tip] Punto di sella instabile
>$$\lambda_{1},\lambda_{2}\in\mathbb{R}\quad \lambda_{1}\neq\lambda_{2}\quad \text{sgn}(\lambda_{1})\neq\text{sgn}(\lambda_{2})$$
>![[Pasted image 20241216182835.png]]

>[!tip] Nodo a due tangenti instabile
>$$\lambda_{1},\lambda_{2}\in\mathbb{R}\quad \lambda_{1}\neq\lambda_{2}\quad \lambda_{1},\lambda_{2}>0$$
>![[Pasted image 20241216182847.png]]

>[!tip] Nodo a due tangenti stabile
>$$\lambda_{1},\lambda_{2}\in\mathbb{R}\quad \lambda_{1}\neq \lambda_{2}\quad \lambda_{1},\lambda_{2}<0$$
>![[Pasted image 20241216182939.png]]

>[!tip] Nodo a stella
>$$\lambda_{1},\lambda_{2}\in\mathbb{R}\quad \lambda_{1}=\lambda_{2}\quad\text{matrice diagonalizzabile}$$
>![[Pasted image 20241216183015.png]]

>[!tip] Nodo a una tangente o improprio
>$$\lambda_{1},\lambda_{2}\in\mathbb{R}\quad \lambda_{1}=\lambda_{2}\quad\text{matrice non diagonalizzabile}$$
>![[Pasted image 20241216183035.png]]

>[!tip] Centro stabile
>$$\lambda_{1},\lambda_{2}\in\mathbb{C}\quad\text{coniugati e immaginari puri}$$
>![[Pasted image 20241216183045.png]]

>[!tip] Fuoco instabile
>$$\lambda_{1},\lambda_{2}\in\mathbb{C}\quad\text{coniugati e }\text{Re}(\lambda_{1})>0$$
>![[Pasted image 20241216183056.png]]

>[!tip] Fuoco stabile
>$$\lambda_{1},\lambda_{2}\in\mathbb{C}\quad\text{coniugati e Re}(\lambda_{1})<0$$
>![[Pasted image 20241216183104.png]]

