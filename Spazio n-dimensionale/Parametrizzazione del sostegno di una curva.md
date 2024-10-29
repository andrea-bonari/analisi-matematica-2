>[!note]
>Siano $I$ e $J$ due intervalli in $\mathbb{R}$. Sia $\overrightarrow{r}:I\to\mathbb{R}^{n}$ una curva con sostegno $\gamma$ e sia $\varphi:J\to I$ una funzione derivabile in $\text{Int}(J)$ e invertibile. Chiamiamo riparametrizzazione di $\gamma$ (relativa a $\varphi$) la curva $\overrightarrow{v}:J\to\mathbb{R}^{n}$ definita come: $$\overrightarrow{v}(s)=\overrightarrow{r}\circ \varphi(s)=\overrightarrow{r}\space(\varphi(s))\quad\forall s\in J$$
>$\varphi$ viene detta cambiamento di variabile.

>[!tip]
>$\varphi:J\to I$ derivabile in $\text{Int}(J)$ e invertibile implica che $\varphi$ sia monotona, cioè strettamente crescente o strettamente decrescente.

>[!note] Teorema dell'invarianza della lunghezza di una curva
>Sia $\overrightarrow{r}:[a,b]\subseteq\mathbb{R}\to\mathbb{R}^{n}$ una curva regolare con sostegno $\gamma$ e sia $\overrightarrow{v}:[c,d]\subseteq\mathbb{R}\to\mathbb{R}^{n}$ una riparametrizzazione di $\gamma$ relativa al cambiamento di variabile $\varphi:[c,d]\to[a,b]$, cioè: $$\overrightarrow{v}(s)=\overrightarrow{r}\circ\varphi(s)\qquad\forall s\in[c,d]$$
>Abbiamo che:
>$$\text{Lunghezza}(\overrightarrow{r}\space([a,b]))=\int_{c}^{d}||\overrightarrow{v}\space'(s)||\text{ d}s$$

>[!example] Dimostrazione
>Ricordiamo che siccome $\overrightarrow{r}$ è regolare, abbiamo che: $$\text{Lunghezza}(\overrightarrow{r}([a,b]))=\int_{a}^{b}||\overrightarrow{r}\space'(t)||\text{ d}t$$
>Usando la formula di derivazione di funzioni composte componente per componente otteniamo che $$\begin{align*}
>\forall s\in [c,d]\qquad \overrightarrow{v}\space'(s)&=\begin{pmatrix}v_{1}'(s)\\\vdots\\v_{n}'(s)\end{pmatrix}=\begin{pmatrix}(r_{1}(\varphi(s)))'\\\vdots\\(r_{n}(\varphi(s)))'\end{pmatrix}=\\
>&=\begin{pmatrix}r_{1}'(\varphi(s))\cdot\varphi'(s)\\\vdots\\r_{n}'(\varphi(s))\cdot \varphi'(s)\end{pmatrix}\\&=\varphi'(s)\begin{pmatrix}r_{1}'(\varphi(s))\\\vdots\\r_{n}'(\varphi(s))\end{pmatrix}=\varphi'(s)\overrightarrow{r}\space'(\varphi(s))
>\end{align*}$$
>E quindi: $$||\overrightarrow{v}\space'(s)||=||\varphi'(s)\overrightarrow{r}\space'(\varphi(s))||=|\varphi'(s)|\cdot||\overrightarrow{r}\space'(\varphi(s))||$$
>Eseguiamo quindi il cambio di variabile $t=\varphi(s)$, che implica che $\text{d}t=\varphi(s)\text{ d}s$ e per gli estremi di integrazione abbiamo due possibilità:
>1. Se $\varphi$ è crescente, allora $\varphi(c)=a< b=\varphi(d)$ e $\varphi'(s)\geq0\quad\forall s\in(c,d)$ e quindi: $$||\overrightarrow{v}\space'(s)||=\varphi'(s)\cdot||\overrightarrow{r}\space'(\varphi(s))||$$
>In questo caso abbiamo che: $$\int_{a}^{b}||\overrightarrow{r}\space'(t)||\text{ d}t=\int_{c}^{d}||\overrightarrow{r}\space'(\varphi(s))||\varphi'(s)\text{ d}s=\int_{c}^{d}||\overrightarrow{v}\space'(s)||\text{ d}s$$
>2. Se $\varphi$ è decrescente, allora $\varphi(c)=b> a=\varphi(d)$ e $\varphi'(s)\leq0\quad\forall s\in(c,d)$: $$||\overrightarrow{v}\space'(s)||=\varphi'(s)\cdot||\overrightarrow{r}\space'(\varphi(s))||$$
>In questo caso abbiamo che: $$\int_{a}^{b}||\overrightarrow{r}\space'(t)||\text{ d}t=\int^{c}_{d}||\overrightarrow{r}\space'(\varphi(s))||(-\varphi'(s))\text{ d} s=\int^{d}_{c}||\overrightarrow{v}\space'(s)||\text{ d}s$$
### Parametrizzazione come grafico
>[!note]
>Un sostegno $\gamma\subseteq\mathbb{R}^{2}$ si dice parametrizzabile come grafico di una funzione $f$ se esiste una funzione $f:I\subseteq\mathbb{R}\to\mathbb{R}$ tale che $\gamma$ è il sostegno della curva definita da: $$\overrightarrow{r}:I\subseteq\mathbb{R}\to\mathbb{R}^{2}$$
>con: $$\begin{cases}
r_{1}(t)=t \\
r_{2}(t)=f(t)
\end{cases}\qquad \forall t\in I$$

### Lunghezza d'arco
>[!note]
>Se $\overrightarrow{r}:[a,b]\to\mathbb{R}^{n}$ è una curva con sostegno $\gamma$, la lunghezza d'arco di $\overrightarrow{r}$ da $a$ a $t\in[a,b]$, è una funzione di $t$, definita da: $$s(t):=\int^{t}_{a}||\overrightarrow{r}\space'(\tau)||\text{ d}\tau$$
>Se $\overrightarrow{r}$ è regolare questa, è la formula della lunghezza del suo sostegno da $\overrightarrow{r}(a)$ a $\overrightarrow{r}(t)$.
>Quando l'integrale a destra nella formula esiste, mentre la lunghezza d'arco elementare, quando calcolabile, è la quantità: $$\text{d}s=||\overrightarrow{r}\space'(t)||\text{ d}t$$

>[!tip]
>Abbiamo che se la funzione lunghezza d'arco esiste, allora:
>- $s$ è derivabile e invertibile (e quindi può essere considerato come cambiamento di variabile)
>- possiamo riparametrizzare $\gamma$ ristretto alla lunghezza d'arco, che è anche detta parametro d'arco o ascissa curvilinea.
