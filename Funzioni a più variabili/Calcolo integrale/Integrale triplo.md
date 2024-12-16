>[!note]
>L'integrale doppio è un integrale multiplo con $k=3$. L'interpretazione geometrica della funzione $1$ è: $$\text{Volume}(r):=\iiint_{\Omega} 1\text{ d}x \text{ d}y \text{ d}z\quad\forall \Omega\subseteq\mathbb{R}^{3}$$
>Le formule di riduzione si hanno anche per $k=3$, ma rispetto a "fili" e a "strati".
>

### Teorema di integrazione per fili
>[!note]
>Sia $\Omega\subseteq\mathbb{R}^{3}$ un insieme rappresentabile nella forma: $$\Omega=\set{(x,y,z)\in\mathbb{R}^{3}:\quad (x,y)\in D\quad l_{1}(x,y)\leq z\leq l_{2}(x,y)}$$
>Dove $D$ è una regione regolare nel piano $xOy$ e $l_{1},l_{2}:D\to\mathbb{R}$ tali che:
>- Siano continue
>- $l_{1}(x,y)\leq l_{2}(x,y)\qquad\forall(x,y)\in D$
>  
>Se $f:\Omega\to\mathbb{R}$ è continua, allora $f$ è integrabile su $\Omega$ e l'integrale si può calcolare con la formula: $$\iiint_{\Omega}f(x,y,z)\text{ d}x \text{ d}y \text{ d} z=\iint_{D} \left(\int\limits_{l_{1}(x,y)}^{l_{2}(x,y)}f(x,y,z)\text{ d}z\right)\text{ d}x \text{ d}y$$

>[!tip]
>Il teorema è espresso con i "fili" paralleli all'asse $z$, ma con una rotazione si può facilmente esprimere con i "fili" paralleli agli altri assi.

### Teorema di integrazione per strati
>[!note]
>Sia $\Omega\subseteq\mathbb{R}^{3}$ rappresentabile della forma: $$\Omega=\set{(x,y,z)\in \mathbb{R}^{3}:\quad z_{1}\leq z\leq z_{2}\quad (x,y)\in D(z)}$$
>Dove $z_{1},z_{2}\in\mathbb{R}$ con $z_{1}\leq z_{2}$ e $\forall z\in[z_{1},z_{2}]$ l'insieme $D(z)$ detto "strato" è un dominio regolare del piano. Se $f$ è continua, allora $f$ è integrabile per $\Omega$ e: $$\iiint_{\Omega} f(x,y,z) \text{ d}x \text{ d}y \text{ d}z=\int_{z_{1}}^{z_{2}} \left(\iint_{D(z)}f(x,y,z)\text{ d}x \text{ d}y\right)\text{ d}z$$

### Coordinate cilindriche
>[!note]
>La funzione relativa alle coordinate cilindriche è: $$\begin{align*}
>&\overrightarrow{T}_{c}:\mathbb{R}^{+}\times[0,2\pi]\times\mathbb{R}\to\mathbb{R}^{>3}\\
>&\overrightarrow{T_{c}}(\rho,\theta, z)= >\begin{pmatrix}\rho\cos\theta\\\rho\sin\theta\\z\end{pmatrix}=\begin{pmatrix}x\\y\\>z\end{pmatrix}
>\end{align*}$$
>E quindi otteniamo: $$\det J_{\overrightarrow{T}_{c}}(\rho,\theta,z)=\rho\neq0$$
>E la formula di integrazione diviene: $$\iiint_{\Omega}f(x,y,z)\text{ d}x \text{ d}y \text{ d}z=\iiint_{\overrightarrow{T}^{-1}_{c}(\Omega)}f(\rho\cos\theta,\rho\sin\theta,z)\rho \text{ d}\rho \text{ d}\theta \text{ d}z$$

### Coordinate sferiche
>[!note]
>La funzione relativa alle coordinate sferiche è: $$\begin{align*}
>&\overrightarrow{T}_{s}:\mathbb{R}^{+}\times[0,\pi]\times[0,2\pi]\to\mathbb{R}^{3}
>\\&\overrightarrow{T}_{s}(\rho,\varphi,\theta)=\begin{pmatrix}\rho\sin\varphi\cos\theta\\\rho\sin\varphi\sin\theta\\\rho\cos\varphi\end{pmatrix}=\begin{pmatrix}x\\y\\z\end{pmatrix}
>\end{align*}$$
>Abbiamo che $\det J_{\overrightarrow{T}_{s}}(\rho,\varphi,\theta)=\rho^{2}\sin\varphi$.
>La formula di integrazione diviene: $$\begin{align*}
&\iiint_{\Omega}f(x,y,z)\text{ d}x \text{ d}y \text{ d}z=\\
=&\iiint_{\overrightarrow{T}^{-1}_{s}(\Omega)}f(\rho\sin\varphi\cos\theta,\rho\sin\varphi\sin\theta,\rho\cos\varphi) \rho^{2}\sin\varphi \text{ d}\rho \text{ d}\varphi \text{ d}\theta 
\end{align*}$$

>[!tip]
>Se immaginiamo la terra come una sfera perfetta:
>- $\theta$ è relativa alla longitudine
>- $\varphi$ è relativa alla latitudine


