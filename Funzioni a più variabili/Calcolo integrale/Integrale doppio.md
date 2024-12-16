>[!note]
>L'integrale doppio è un integrale multiplo con $k=2$. Definiamo alcune regioni $D\subseteq\mathbb{R}^{2}$ adatte all'integrazione.

### Insieme y-semplice
>[!note]
>Un insieme $D\subseteq\mathbb{R}^{2}$ si dice $y$-semplice se è del tipo: $$D=\set{(x,y)\in\mathbb{R}^{2}:\quad x\in [a,b],\quad g_{1}(x)\leq y\leq g_{2}(x)}$$
>Dove $a,b\in\mathbb{R}$ con $a<b$ e $g_{1},g_{2}:[a,b]\to\mathbb{R}$ sono funzioni tali che:
>- $g_{1}$ e $g_{2}$ sono continue
>- $g_{1}(x)\leq g_{2}(x)\quad \forall x\in[a,b]$
>
>Abbiamo che: $$\text{Area}(D)=\int_{a}^{b}g_{2}(x)\text{ d}x-\int_{a}^{b}g_{1}(x)\text{ d}x=\int_{a}^{b}g_{2}(x)-g_{1}(x)\text{ d}x$$

>[!tip]
>Osserviamo che il volume tra $D$ e il grafico della funzione $f:D\to\mathbb{R}$: $$f(x,y)=1$$
>Coincide con l'area di $D$: $$\int_{D}f(\overrightarrow{x})\text{ d}\overrightarrow{x}=\iint_{D}1\text{ d}x \text{ d}y=\text{Area}(D)$$

### Insieme x-semplice
>[!note]
>Un inseme $D\subseteq\mathbb{R}^{2}$ si dice $x$-semplice se è del tipo: $$D=\set{(x,y)\in\mathbb{R}^{2}:\quad x\in[c,d],\quad h_{1}(y)\leq x\leq h_{2}(y)}$$
>Dove $c,d\in\mathbb{R}$ con $c<d$ e $h_{1},h_{2}:[c,d]\to\mathbb{R}$ tali che:
>- $h_{1}$ e $h_{2}$ sono continue
>- $h_{1}(y)\leq h_{2}(y)\quad\forall y\in[c,d]$
>
>Abbiamo che: $$\text{Area}(D)=\int^{d}_{c}h_{2}(y)-h_{1}(y)\text{ d}y$$

### Insieme regolare
>[!note]
>Un insieme $E\subseteq\mathbb{R}^{2}$ si dice regolare se è unione finita di insiemi $x$-semplici e $y$-semplici.

>[!tip]
>Siccome l'area di un insieme regolare è dato dalla somma delle aree dei suoi insiemi $x$-semplici e $y$-semplici possiamo definire: $$\iint_{E}1\text{ d}x \text{ d}y=\text{Area}(E)$$

### Somma di Cauchy-Riemann
>[!note]
>Consideriamo una funzione $f:A\subseteq\mathbb{R}^{2}\to\mathbb{R}$ limitata con $A:=[a,b]\times[c,d]$ per $a,b,c,d\in\mathbb{R}$ con $a<b$ e $c<d$. Consideriamo una partizione $\set{x_{h}}^{n}_{h=0}$ di $[a,b]$ equiparziata, cioè $a=x_{0}<\cdots<x_{n}=b$ con $x_{h}-x_{h-1}= \frac{b-a}{n}$. In analogia, consideriamo una partizione $\set{y_{k}}^{k}_{k=0}$ di $[c,d]$ equiparziata, cioè $c=y_{0}<\cdots<y_{n}=d$ con $y_{k}-y_{k-1}= \frac{d-c}{n}$.
>Definiamo $I_{h,k}=[x_{h-1},h]\times[y_{k-1},y_{k}]\quad\forall h,k=1,\cdots, n$. Scegliamo un punto $p_{h,k}\in I_{h,k}$ e chiamiamo $P_{h,k}$ il parallelepipedo con base $I_{h,k}$ e altezza $f(p_{h,k})$.
>Abbiamo che il volume di ciascun $P_{h,k}$ è dato da: $$\text{Vol}(P_{h,k})=\text{Area}(I_{h,k})\cdot f(p_{h,k})= \frac{b-a}{n}\cdot \frac{d-c}{n}\cdot f(p_{h,k})$$
>Diciamo che $f$ è integrabile su $A=[a,b]\times[c,d]$ se: $$\exists\lim_{n\to\infty}\sum\limits^{n}_{h,k=1}\text{Vol}(P_{h,k})=\lim_{n\to\infty} \frac{b-a}{n} \frac{c-d}{n}\sum\limits_{h,k=1}^{n}f(P_{h,k})$$
>Finito e non dipende dalla scelta dei punti $p_{h,k}$ nei rettangolini $I_{h,k}$.
>In questo caso definiamo: $$\iint_{A}f(x,y)\text{ d}x \text{ d}y= \lim_{n\to\infty} \frac{b-a}{n} \frac{c-d}{n}\sum\limits_{h,k=1}^{n}f(P_{h,k})$$

Questa definizione è la naturale estensione dell'idea usata per definire gli integrali con $k=1$.

### Teorema di integrabilità di funzioni continue
>[!note]
>Sia $D\subseteq\mathbb{R}^{2}$ un insieme regolare e sia $f:D\to\mathbb{R}$ una funzione continua in $D$. Allora $f$ è integrabile in $D$.

### Teorema delle formule di riduzione (a integrali iterati)
>[!note]
>Sia $D$ un dominio $y$-semplice, cioè: $$D=\set{(x,y)\in\mathbb{R}^{2}:\quad x\in[a,b]\quad g_{1}(x)\leq y\leq g_{2}(x)}$$
>Per appropriati $a,b,g_{1},g_{2}$, e sia $f:D\to\mathbb{R}$ una funzione continua in $D$. Allora abbiamo che: $$\iint_{D}f(x,y)\text{ d}x \text{ d}y=\int_{a}^{b} \left(\int\limits_{g_{1}(x)}^{g_{2}(x)}f(x,y)\text{ d} y\right)\text{ d}x$$
>Analogamente, sia $D$ un dominio $x$-semplice, cioè: $$D=\set{(x,y)\in\mathbb{R}^{2}:\quad y\in[c,d]\quad h_{1}(y)\leq x\leq h_{2}(y)}$$
>Per appropriati $c,d,h_{1},h_{2}$, e sia $f: D\to\mathbb{R}$ continua in $D$. Allora abbiamo che: $$\iint_{D}f(x,y)\text{ d}x \text{ d}y=\int_{c}^{d} \left(\int\limits_{h_{1}(y)}^{h_{2}(y)}f(x,y)\text{ d}x\right)\text{ d}y$$

### Coordinate polari
>[!note]
>Sia il cambiamento di variabili $\overrightarrow{T}_{\rho}:\mathbb{R}^{+}\times[0,2\pi]\to\mathbb{R}^{2}$ un cambiamento che associa ogni punto nel piano $(x,y)$ alle sue coordinate polari: $$\overrightarrow{T}_{\rho}(\rho,\theta)=\begin{pmatrix}\rho\cos\theta\\\rho\sin\theta\end{pmatrix}=\begin{pmatrix}x\\y\end{pmatrix}$$
>La sua matrice Jacobiana è definita come: $$J_{\overrightarrow{T}_{\rho}}(\rho,\theta)=\begin{pmatrix}\cos\theta&-\rho\sin\theta\\\sin\theta&\rho\cos\theta\end{pmatrix}$$
>E quindi $\det J_{\overrightarrow{T}_{\rho}}(\rho,\theta)=\rho\cos^{2}\theta+\rho\sin^{2}\theta=\rho\neq0$.

>[!tip]
>Quindi $\overrightarrow{T}_{\rho}$ ristretto a $(0,+\infty)\times(0,2\pi)$ è un cambio di variabili con immagine: $$\mathbb{R}^{2}\smallsetminus\set{(x,y):\quad x\geq0,y=0}$$

