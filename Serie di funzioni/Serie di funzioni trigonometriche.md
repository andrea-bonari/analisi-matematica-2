>[!note]
>Denotiamo come polinomio trigonometrico di ordine $n\in\mathbb{N}$ una funzione $P_{n}$ periodica di periodo $2\pi$ del tipo: $$P_{n}(x):= a_{0}+\sum\limits_{n=1}^{n}\left(a_{n}\cos(nx)+b_{n}\sin(nx)\right)$$
>$a_{0},a_{n},b_{n}\in\mathbb{R}$ che vengono chiamati coefficienti del polinomio trigonometrico, definito $\forall x\in\mathbb{R}$. In particolare i polinomi trigonometrici con $a_{0}=0$ e tutti gli altri coefficienti nulli, tranne uno uguale a $1$. Cioè $\cos(nx)$ e $\sin(nx)$ $\forall n\in\mathbb{N}$, sono dette armoniche $n$-esime.

Ogni armonica $n$-esima è periodica di periodo $\frac{2\pi}{n}$ e quindi $P_{n}(x)$ è periodica di periodo $2\pi$.
Inoltre le armoniche $\sin(nx)$ sono tutte funzioni dispari, e le armoniche $\cos(nx)$ sono tutte funzioni pari.

La somma, differenza e prodotto di due polinomi trigonometrici è ancora un polinomio trigonometrico. Abbiamo delle formule di ortogonalità delle armoniche $n$-esime: $$\begin{align*}
&\int^{\pi}_{-\pi}\cos(nx)\cos(kx)\text{ d}x=\begin{cases}0&\text{se }n\neq k\\\pi&\text{se }n= k\end{cases}\\
&\int^{\pi}_{-\pi}\sin(nx)\sin(kx)\text{ d}x=\begin{cases}0&\text{se }n\neq k\\\pi&\text{se }n= k\end{cases}\\
&\int^{\pi}_{-\pi}\sin(nx)\cos(kx)\text{ d}x=0\quad\forall n,k\in\mathbb{N}
\end{align*}$$
L'integrale del prodotto di due armoniche diverse è sempre nullo, mentre l'integrale del quadrato di una di queste è $\pi$ (osserviamo che il caso $n=0$ è eccezione, infatti otteniamo $2\pi$).

### Serie trigonometriche
>[!note]
>Si definisce serie trigonometrica l'espressione $$a_{0}+\sum\limits_{n=1}^{\infty}(a_{n}\cos(n x)+b_{n}\sin(nx))$$
>Dove $a_{0},a_{n},b_{n}\in\mathbb{R}$ sono assegnati e $x\in\mathbb{R}$.

>[!tip]
>Diciamo che una funzione $f:\mathbb{R}\to\mathbb{R}$ è periodica di periodo $T>0$ se $\forall x\in\mathbb{R}$ abbiamo che: $$f(x+T)=f(x)$$
>La proprietà di periodicità non implica alcuna regolarità. Stiamo quindi includendo anche funzioni discontinue.

In generale ci soffermeremo su funzioni $2\pi$-periodiche.

### Coefficienti di Fourier
>[!note]
>Data $f:\mathbb{R}\to\mathbb{R}$ $2\pi$-periodica, definiamo i coefficienti di Fourier relativi a $f$ come i seguenti coefficienti: $$\begin{align*}
a_{0}&:= \frac{1}{2\pi}\int_{-\pi}^{\pi}f(x)\text{ d}x\\
a_{n}&:= \frac{1}{\pi}\int_{-\pi}^{\pi}f(x)\cos(nx)\text{ d}x\\
b_{n}&:= \frac{1}{\pi}\int_{-\pi}^{\pi}f(x)\sin(nx)\text{ d}x
\end{align*}$$
>$\forall n\in\mathbb{N}$, quando gli integrali sono ben definiti ed esistono finiti.

>[!tip] Calcolo dei coefficienti di Fourier
>Se una funzione $2\pi$-periodica $f:\mathbb{R}\to\mathbb{R}$ è somma di una serie trigonometrica, cioè: $$f(x)=a_{0}+\sum\limits_{n=1}^{\infty}(a_{n}\cos(n x)+b_{n}\sin(nx))$$
>Con $a_{0},a_{n},b_{n}\in\mathbb{R}$, con convergenza totale su $[-\pi,\pi]$, allora abbiamo che necessariamente $a_{0}, a_{n},b_{n}$ sono i coefficienti di Fourier di $f\quad\forall n\in\mathbb{N}$.

>[!example] Dimostrazione
>Assumiamo che $\exists a_{0},a_{n},b_{n}\in\mathbb{R}$ tale che: $$f(x)=a_{0}+\sum\limits_{n=1}^{\infty}(a_{n}\cos(n x)+b_{n}\sin(nx))$$
>Con convergenza totale su $[-\pi,\pi]$.
>
>Iniziamo con $a_{0}$ e calcoliamo: $$\begin{align*}
>\int_{-\pi}^{\pi}f(x)\text{ d}x&= \int_{-\pi}^{\pi}a_{0}+\sum\limits_{n=1}^{\infty}(a_{n}\cos(n x)+b_{n}\sin(nx))\text{ d}x\\
>&= \int_{-\pi}^{\pi}a_{0}\text{ d}x+\sum\limits_{n=1}^{\infty}a_{n}\int_{-\pi}^{\pi}\cos(nx)\text{ d}x+\sum\limits_{n=1}^{\infty}b_{n}\int_{-\pi}^{\pi}\sin(nx)\text{ d}x\\
>&= a_{0}\cdot2\pi+\sum\limits_{n=1}^{\infty}(a_{n}\cdot 0)+\sum\limits_{n=1}^{\infty}(b_{n}\cdot 0)=a_{0}\cdot 2\pi
>\end{align*}$$
>E quindi $a_{0}= \frac{1}{2\pi}\int_{-\pi}^{\pi}f(x)\text{ d}x$.
>Proseguiamo con il calcolo degli $a_{k}\quad\forall k\in\mathbb{N}$:
>$$\begin{align*}
>\int_{-\pi}^{\pi}f(x)\cos(kx)\text{ d}x&=\int_{-\pi}^{\pi}\left[a_{0}+\sum\limits_{n=1}^{\infty}(a_{n}\cos(n x)+b_{n}\sin(nx))\right]\cos(kx)\text{ d}x\\
>&=a_{0}\int_{-\pi}^{\pi}\cos(kx)\text{ d}x\space\begin{matrix}\\\\+\sum\limits_{n=1}^{\infty}a_{n}\int_{-\pi}^{\pi}\cos (nx)\cos(kx)\text{ d}x\\+\sum\limits_{n=1}^{\infty}b_{n}\int_{-\pi}^{\pi}\sin (nx)\cos(kx)\text{ d}x\end{matrix}\\\\
>&= a_{0}\cdot 0+\sum\limits_{\begin{matrix}n=1\\ n\neq k\end{matrix}}^{\infty}a_{n}\cdot0+a_{k}\cdot \pi+\sum\limits_{n=1}^{\infty}b_{n}\cdot0\\
>&= a_{k}\cdot \pi
>\end{align*}$$
>E quindi $a_{k}=\frac{1}{\pi}\int_{-\pi}^{\pi}f(x)\cos(kx)\text{ d}x$.
>
>Si procede analogamente per i coefficienti $b_{k}\quad k\in\mathbb{N}$.

### Serie di Fourier
>[!note]
>Data una funzione $f:\mathbb{R}\to\mathbb{R}$ $2\pi$-periodica chiamiamo polinomio di Fourier di ordine $n\in\mathbb{N}$ associato a $f$ il seguente polinomio trigonometrico: $$F_{m}(x)=a_{0}+\sum\limits_{n=1}^{m}(a_{n}\cos(n x)+b_{n}\sin(nx))$$
>Con $a_{0},a_{n},b_{n}\in\mathbb{R}$ definiti come coefficienti di Fourier, mentre chiamiamo serie di Fourier di $f$ il limite (quando esiste): $$\lim_{m\to+\infty} F_{m}(x)$$

### Teorema di convergenza di una serie trigonometrica a partire dai coefficienti
>[!note]
>Data una serie trigonometrica: $$a_{0}+\sum\limits_{n=1}^{\infty}(a_{n}\cos(n x)+b_{n}\sin(nx))$$
>Con $a_{0},a_{n},b_{n}\in\mathbb{R}\quad\forall n\in\mathbb{N}$ abbiamo che:
>- Se la serie numerica di termine generale $|a_{n}|+|b_{n}|$ (considerata per indici $n\in\mathbb{N}$) è convergente, allora la serie trigonometrica converge totalmente in $\mathbb{R}$. Inoltre la somma è continua ed è possibile integrare termine a termine (su intervalli limitati), cioè: $$\begin{align*}
>&\int_{x_{0}}^{x}a_{0}+\sum\limits_{n=1}^{\infty}(a_{n}\cos(n s)+b_{n}\sin(ns))\text{ d}s\\=&a_{0}(x-x_{0})+\sum\limits_{n=1}^{\infty} \left[a_{n}\int_{x_{0}}^{x}\cos(ns)\text{ d}s+b_{n}\int_{x_{0}}^{x}\sin(ns)\text{ d}s\right]\qquad\forall x,x_{0}\in\mathbb{R}
>\end{align*}$$
>- Se la serie numerica di termine generale $n(|a_{n}|+|b_{n}|)$ (considerata per indici $n\in\mathbb{N}$) è convergente, allora la somma della serie trigonometrica è derivabile, e la derivata è data dalla serie delle derivate (derivazione termine a termine), cioè: $$\begin{align*}
>& \frac{\text{ d}}{\text{ d}x}\left[ a_{0}+\sum\limits_{n=1}^{\infty}(a_{n}\cos(n x)+b_{n}\sin(nx))\text{ d}x\right]\\=&\sum\limits_{n=1}^{\infty}n[-a_{n}\sin(nx)+b_{n}\cos(nx)]
>\end{align*}$$

La condizione nel secondo caso è più forte della condizione nel primo caso. Inoltre c'è una differenza rispetto a quanto visto per le serie di potenze, che sono integrabili e derivabili $\infty$ volte senza richiedere ulteriori condizioni aggiuntive.

Siccome la derivata è ancora una serie trigonometrica, possiamo iterare il teorema:
- se $\sum\limits n^{2}(|a_{n}|+|b_{n}|)$ è convergente, allora la somma della serie trigonometrica è derivabile 2 volte con derivata seconda calcolata termine a termine.
- Genericamente, se $\sum\limits_{n=1}^{\infty}n^{\alpha}(|a_{n}|+|b_{n}|)$ è convergente con $\alpha>2$, allora la somma della serie trigonometrica è derivabile $\alpha$ volte.

### Teorema di convergenza puntuale delle serie di Fourier
>[!note]
>Sia $f:\mathbb{R}\to\mathbb{R}$ $2\pi$-periodica e regolare a tratti in $[-\pi,\pi]$. Allora la serie di Fourier converge puntualmente in tutto $\mathbb{R}$.
>In particolare, sia $F_{m}(x)$ il polinomio di Fourier di ordine $m\in\mathbb{N}$ associato a $f$, allora: $$\lim_{m\to\infty} F_{m}(x)= \frac{1}{2}\left(\lim_{s\to x^{+}} f(s)+ \lim_{s\to x^{-}} f(s)\right)$$
>E quindi, se $f$ è continua in $x$, allora: $$\lim_{m\to\infty}F_{m}(x)= f(x)$$

>[!tip] Funzioni regolare a tratti
>Sia $f:[a,b]\to\mathbb{R}$. Diciamo che $f$ è regolare a tratti in $[a,b]$ se esiste un numero finito $N$ di punti $a=x_{1}<x_{2}<\cdots<x_{N}=b$, cioè una partizione dell'intervallo $[a,b]$ tale che:
>- $f$ è continua in $(x_{i},x_{i+1})\quad\forall i=1,\cdots,N-1$ ed esistano finiti i limiti: $$\lim_{x\to x_{i}^{+}}f(x)\qquad \lim_{x\to x_{i+1}^{-}}f(x)$$
>- $f$ è derivabile in $(x_{i},x_{i+1})\quad\forall i=1,\cdots,N-1$ ed esistano finiti i limiti: $$\lim_{x\to x_{i}^{+}}f'(x)\qquad\lim_{x\to x_{i+1}^{-}}f'(x)$$

### Teorema di convergenza totale della serie di Fourier e integrabilità
>[!note]
>Sia $f:\mathbb{R}\to\mathbb{R}$ $2\pi$-periodica e regolare a tratti in $[-\pi,\pi]$. Se $f$ è continua in $\mathbb{R}$, allora la serie di Fourier di $f$ converge totalmente a $f$ in tutto $\mathbb{R}$ e vale la formula di integrabilità termine a termine negli intervalli limitati.

### Derivabilità della serie di Fourier
>[!note]
>Sia $f:\mathbb{R}\to\mathbb{R}$ $2\pi$-periodica e tale che:
>- $f$ sia derivabile su $\mathbb{R}$
>- $f'$ è regolare a tratti in $[-\pi,\pi]$
>- $f'$ continua
>
>Allora la serie di Fourier di $f$ è derivabile su $\mathbb{R}$ termine a termine.

### Convergenza in media
>[!note]
>Data una funzione $f:\mathbb{R}\to\mathbb{R}$ $2\pi$-periodica si dice che la serie di Fourier associata a $f$ converge in norma (o in media) quadratica a $f$ se: $$\lim_{n\to\infty}\int_{-\pi}^{\pi}|f(x)-F_{n}(x)|^{2}\text{ d}x=0$$
>Dove $F_{n}$ è il polinomio di Fourier di ordine $n\in\mathbb{N}$.

### Identità di Bessel-Parseval
>[!note]
>Sia $f:\mathbb{R}\to\mathbb{R}$ $2\pi$-periodica e regolare a tratti in $[-\pi,\pi]$. Abbiamo che se i seguenti asserti sono verificati:
>- La serie di Fourier di $f$ converge sempre in norma quadratica.
>- Se indichiamo con $a_{0},a_{n},b_{n}$ i coefficienti di Fourier di $f\quad\forall n\in\mathbb{N}$, allora vale la seguente identità detta identità di Bessel-Parseval: $$2a_{0}^{2}+\sum\limits_{n=1}^{\infty}\left(a_{n}^{2}+b_{n}^{2}\right)= \frac{1}{\pi}\int_{-\pi}^\pi|f(x)|^{2}\text{ d}x$$
