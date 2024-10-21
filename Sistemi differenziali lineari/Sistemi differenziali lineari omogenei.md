>[!note]
>Un SDL omogeneo è un sistema differenziale lineare definito come: $$\overrightarrow{y}\space'(t)=A(t)\cdot \overrightarrow{y}(t)\qquad t\in I$$

### Integrale generale
>[!note]
>Sia $A:I\subseteq \mathbb{R}\to M_{n\times m}$ continua. L'integrale generale di $$\overrightarrow{y}\space'(t)=A(t)\cdot \overrightarrow{y}(t)\qquad t\in I$$
>È uno spazio vettoriale di dimensione $n$, cioè si può scrivere come: $$\overrightarrow{y}_{\sigma}(t)=c_{1}y_{\sigma1}(t)+\cdots+c_{n}y_{\sigma n}(t)\qquad t\in I$$
>Con $\overrightarrow{c}=\begin{pmatrix}c_{1}\\\vdots\\ c_{n}\end{pmatrix}\in\mathbb{R}^{n}$, dove $y_{\sigma1},\cdots,y_{\sigma n}$ sono $n$ soluzioni linearmente indipendenti.
>In particolare $\set{y_{\sigma1},\cdots,y_{\sigma n}}$ sono una base dello spazio delle soluzioni e vengono chiamate Sistema Fondamentale di Soluzioni (SFS).

>[!note] Risoluzione esplicita con $A(x)\equiv A\in M_{n\times n}$
>Per trovare $n$ soluzioni esplicitamente trattiamo due casi:
>1. Con $A(x)\equiv A\in M_{n\times n}$ diagonalizzabile
>2. Con $A(x)\equiv A\in M_{2\times 2}$ con due autovalori complessi e coniugati.
>
>##### Caso 1
>Data $A\in M_{n\times n}$ diagonalizzabile, un SFS per $\overrightarrow{y}\space'(x)=A\overrightarrow{y}(x)$ per $x\in\mathbb{R}$ è $$\overrightarrow{y}_{\sigma i}=e^{\lambda_{i}x}\overrightarrow{v}_{i}$$
>Dove $v_{i}$ sono autovettori relativi agli autovalori $\lambda_{i}$. Quindi l'integrale generale è: $$\overrightarrow{y}_{\sigma}(x)=\sum\limits_{i=1}^{n}c_{i}e^{\lambda_{i}x}\overrightarrow{v}_{i}\quad x\in\mathbb{R}\quad c_{1},\cdots,c_{n}\in\mathbb{R}$$

>[!tip]
>Data $A\in M_{n\times n}$ è diagonalizzabile in $\mathbb{R}$ se è simile ad una matrice diagonale del tipo: $$D=\begin{pmatrix}d_{1}&0&0\\0&\ddots&0\\0&0&d_{n}\end{pmatrix}$$
>Con $d_{i}\in\mathbb{R}$ con $\forall i=1,\cdots, n$, cioè se esiste una matrice invertibile $D$ tale che $D=D^{-1}AP$In genere $D$ è la matrice di autovalori di $A$ e $P$ è la matrice con i corrispondenti autovettori come colonne.

### Matrice Wroskiana
>[!note]
>Date $n$ soluzioni $y_{i}: J\subseteq\mathbb{R}\to\mathbb{R}^{n}$, con $i=1,\cdots,n$, chiamiamo matrice Wroskiana la matrice costruita affiancando i vettori colonna $\overrightarrow{y}_{i}(t)$, cioè: $$W(t)=\begin{pmatrix}y_{1}(t)&|&\cdots&|&y_{n(t)}\end{pmatrix}\quad x\in J$$
>E si definisce determinante Wroskiano il suo determinante.

>[!tip]
>Data una matrice $A\in M_{n\times n}$ abbiamo che:
>$$\det(A)\neq0\iff \text{linearmente indipendente}$$
>Quindi per verificare che $n$ soluzioni $\overrightarrow{y}_{1},\cdots, \overrightarrow{y}_{n}$ sono linearmente indipendenti, verifichiamo: $$\exists t_{0}\in J\quad|\qquad \det(W_{\overrightarrow{y}_{i}}(t_{0}))\neq0$$

>[!note] Determinante Wroskiano
>Date $n$ soluzioni $\overrightarrow{y}_{\sigma i}:J\subseteq\mathbb{R}\to\mathbb{R}^{n}$ con $i=1,\cdots,n$ di $$\overrightarrow{y}\space'(x)=A(x)\cdot\overrightarrow{y}(x)$$
>Se $\exists x_{0}\in J$ tale che $\det(W(x_{0}))\neq0$, dove $W$ è la matrice Wroskiana associata a $\overrightarrow{y}_{\sigma i}$, con $i=1,\cdots, n$, allora le funzioni $\overrightarrow{y}_{\sigma 1,},\cdots,\overrightarrow{y}_{\sigma n}$, formano un SFS e l'integrale generale del SDL si può scrivere nella forma: $$y_{\sigma}(x)=c_{1}y_{\sigma1}(x)+\cdots+c_{n}y_{\sigma n}(x)=W(x)\cdot\overrightarrow{c}$$
>Dove $\overrightarrow{c}=\begin{pmatrix}c_{1}\\\vdots\\c_{n}\end{pmatrix}\in\mathbb{R}^{n}$ è il vettore costante generico.
>Inoltre la soluzione del problema di Cauchy associato con la condizione $\overrightarrow{y}(x_{0})=\overrightarrow{y}_{0}$ per $\overrightarrow{y}_{0}\in\mathbb{R}^{n}$ è: $$\overrightarrow{y}(x)=W(x)W^{-1}(x_{0})\overrightarrow{y}_{0}$$

