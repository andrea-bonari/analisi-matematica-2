>[!note]
>Una curva in $\mathbb{R}^{n}$ è definita da $n$ funzioni $$r_{1},\cdots,r_{n}:I\subseteq\mathbb{R}\to\mathbb{R}^{n}$$
>Dove $I\subseteq\mathbb{R}$ è un intervallo che può essere chiuso, aperto, semiaperto o illimitato. La curva si può scrivere come funzione vettoriale nel seguente modo: $$\overrightarrow{r}=I\subseteq\mathbb{R}\to\mathbb{R}^{n}$$
>$$\overrightarrow{r}(t)=\begin{pmatrix}r_{1}(t)\\\vdots\\ r_{n}(t)\end{pmatrix}=\sum\limits_{i=1}^{n}r_{i}(t)\overrightarrow{e}_{i}$$
>Inoltre, ci si riferisce a: $$\gamma:=\set{(x_{1},\cdots,x_{n})\in\mathbb{R}^{n}:\quad\exists t\in I\quad r_{i}(t)=x_{i}\quad\forall i=1,\cdots,n}$$
>Come al sostegno della curva.

>[!tip]
>Due curve con stesso sostegno sono dette equivalenti.

Diciamo che $\overrightarrow{r}:[a,b]\to\mathbb{R}^{n}$ con $a<b$ è:
- Chiusa se $\overrightarrow{r}(a)=\overrightarrow{r}(b)$
- Semplice se $\overrightarrow{r}$ ristretta all'intervallo aperto $(a,b)$ è iniettiva

$\overrightarrow{r}$ è continua in $t$ se e solo se $r_{1},\cdots,r_{n}$ sono continue in $t$.

>[!tip]
>Un insieme $E\subseteq\mathbb{R}^{n}$ si dice connesso per archi se $\forall\overrightarrow{x},\overrightarrow{y}\in E$ esiste una curva continua $\overrightarrow{r}(t)$ con sostegno contenuto in $E$ e con estremi $\overrightarrow{x}$ e $\overrightarrow{y}$.

### Limiti di curve
>[!note]
>Sia $\overrightarrow{r}:I\subseteq\mathbb{R}\to\mathbb{R}^{n}$ una curva su un intervallo $I$, allora: $$\begin{align*}
&\exists\lim_{t\to t_{0}}\overrightarrow{r}(t)=\overrightarrow{r}\space^{0}=\begin{pmatrix}r_{1}^{0}\\\vdots\\r_{n}^{0}\end{pmatrix}\in\mathbb{R}^{n}\\
\iff&\forall i=1,\cdots,n\quad\exists\lim_{t\to t_{0}}r_{i}(t)=r_{i}^{0}\in\mathbb{R}\\
\iff&\exists\lim_{t\to t_{0}} ||\overrightarrow{r}(t)-\overrightarrow{r}\space^{0}||=0
\end{align*}$$

È possibile estendere alle curve le proprietà dei limiti di funzioni in una variabile (unicità del limite, algebra dei limiti, ...).

### Curve regolari
>[!note]
>Sia $\overrightarrow{r}:I\subseteq\mathbb{R}\to\mathbb{R}^{n}$ una curva definita su un intervallo aperto $I$. Diciamo che $\overrightarrow{r}$ è regolare se:
>- $\overrightarrow{r}\in c^{1}(I;\mathbb{R}^{n})$
>- $\overrightarrow{r}\space'(t)\neq0\quad\forall t\in I$
>
>Oppure, Sia $I=[a,b]$ per $a<b$ e $\overrightarrow{r}:[a,b]\to\mathbb{R}^{n}$ sia una curva. Diciamo che $\overrightarrow{r}$ è regolare se $\overrightarrow{r}\space\bigg|_{(a,b)}$ è regolare.

>[!tip] Derivate di vettori
>$$\overrightarrow{r}\space'(t)=\begin{pmatrix}r_{1}'(t)\\\vdots\\r_{n}'(t)\end{pmatrix}\qquad \forall t\in I$$

>[!tip] Curve regolari a tratti
>Diciamo che una curva $\overrightarrow{r}:I\subseteq\mathbb{R}\to\mathbb{R}^{n}$ è regolare a tratti se:
>- $\overrightarrow{r}\in c^{0}(I;\mathbb{R}^{n})$
>- ad eccezione di un numero finito di $k\in\mathbb{N}$ punti $t_{1},\cdots,t_{k}\in I$ la curvatura è regolare.

### Versore tangente
>[!note]
>Sia $\overrightarrow{r}:I\subseteq\mathbb{R}\to\mathbb{R}^{n}$ una curva regolare. Chiamiamo versore tangente a $\overrightarrow{r}$ (o al sostegno di $\overrightarrow{r}$) il vettore $\overrightarrow{T}$ definito $\forall t\in I$ da:
>$$\overrightarrow{T}(t)=\frac{\overrightarrow{r}\space'(t)}{||\overrightarrow{r}\space'(t)||}=\begin{pmatrix}\frac{\overrightarrow{r}_{1}\space'(t)}{\sqrt{(r'_{1}(t))^{2}+\cdots+(r_{2}'(t))^{2}}}\\\vdots\\\frac{\overrightarrow{r}_{n}\space'(t)}{\sqrt{(r'_{1}(t))^{2}+\cdots+(r_{2}'(t))^{2}}}\end{pmatrix}$$

### Lunghezza
>[!note]
>Sia $\overrightarrow{r}: I\subseteq\mathbb{R}\to\mathbb{R}^{n}$ una curva regolare su un intervallo $I$ con sostegno $\gamma$. Si dica lunghezza di $\gamma$ (o lunghezza della curva) il numero: $$\text{Lunghezza}(\gamma):=\int_{I}||\overrightarrow{r}\space'(t)||\text{ d}t$$

>[!tip] Lunghezza di una curva regolare a tratti
>Sia $I$ un intervallo in $\mathbb{R}$ con estremi $a,b\in \mathbb{R}\cup\set{\pm\infty}$ con $a<b$ e sia $\overrightarrow{r}:I\to\mathbb{R}^{n}$ una curvatura regolare a tratti con sostegno $\gamma$. Siano $t_{1}<\cdots<t_{k}\in I$ tali che $\overrightarrow{r}$ è regolare in $I\smallsetminus\set{t_{1},\cdots,t_{k}}$. Si dice lunghezza (del sostegno) della curva: $$\text{Lunghezza}(\gamma):=\int_{a}^{t_{1}}||\overrightarrow{r}\space'||\text{ d}t+\int_{t_{1}}^{t_{2}}||\overrightarrow{r}\space'||\text{ d}t+\cdots+\int_{t_{k}}^{b}||\overrightarrow{r}\space'||\text{ d}t$$




