### Soluzioni costanti
>[!note]
>Data un'EDO del primo ordine in forma normale: $$y'(t)=f(t,\space y(t))\qquad t\in\mathbb{R}$$
>Per un certo intervallo $I\subseteq\mathbb{R}$, può esistere una soluzione costante dell'EDO del tipo: $$y(t)\equiv k\in\mathbb{R}\qquad\forall t\in I$$

>[!tip]
>Siccome $\forall k\in\mathbb{R}$, la derivata è $0$, necessariamente $f(t,\space k)=0$
>$$y(t)\equiv k\quad\forall t\in I\iff f(t,\space k)=0\quad\forall t\in I$$

### EDO del primo ordine a variabili separabili
>[!note]
>Un'EDO del primo ordine si dice a variabili separabili se è nella forma: $$y'(t)=h(t)\cdot g(y(t))\qquad t\in I$$
>Con $h: I_{1}\subseteq\mathbb{R}\to\mathbb{R}$ e $g: I_{2}\subseteq\mathbb{R}\to\mathbb{R}$ funzioni continue. Quando è in forma normale: $$f(t,\space s)=h(t)\cdot g(s)$$

Processo risolutivo di un'EDO del primo ordine a variabili separabili:
1. Cerchiamo soluzioni costanti dell'EDO, quindi imponiamo $$g(s)=0$$
2. Cerchiamo le soluzioni non costanti della EDO:
	1. Dividiamo la EDO per $g(y(t))$: $$\frac{y'(t)}{g(y(t))}=h(t)$$
	2. Cerchiamo la primitiva di entrambi i membri con il Teorema Fondamentale del Calcolo Integrale: $$\int \frac{y'(t)}{g(y(t))}\text{ d}t=\int h(t)\text{ d}t$$
	3. Risolvo direttamente a destra e risolvo a sinistra dopo aver imposto il cambio di variabili $z=y(t)$: $$\begin{cases} z=y(t) \\ \text{d}z=y'(t)\text{ d}t \end{cases}\Longrightarrow \int \frac{1}{g(z)}\text{ d}z=\int h(t)\text{ d}t$$
	4. Trovo la formula esplicita per $y(t)$ con appropriate condizioni sulle costanti di integrazione e sul dominio. Inoltre definiamo come $c$ i termini costanti.
3. Scrivo l'integrale generale inserendo insieme le soluzioni trovate ai passi 1 e 2.

>[!tip]
>È anche possibile risolvere un'EDO del primo ordine a variabili separabili utilizzando la seconda parte del Teorema Fondamentale del Calcolo Integrale, quindi utilizzando un integrale definito con estremi di integrazione $t$ e $t_{0}$.

>[!tip]
>I domini delle soluzioni sono diversi e possono essere strettamente inclusi nell'intervallo di definizione dell'EDO (anche se è definita ovunque)

>[!tip]
>I grafici delle soluzioni, pur riempendo tutto il dominio di $f$ non intersecano.

### EDO del primo ordine lineari
>[!note]
>Un'EDO del primo ordine si dice a lineare se è nella forma: $$y'(t)=a(t)\cdot y(t)+b(t)\qquad t\in I$$
>Con $a,b: I\subseteq\mathbb{R}\to\mathbb{R}$. Inoltre si dice omogenea se $b\equiv 0$, altrimenti è detta completa. L'EDO lineari sono in forma normali se $b\equiv 0$, allora l'EDO è anche a variabili separabili.

>[!tip]
>Le funzioni $a$ e $b$ possono anche non essere lineari.

>[!tip]
>Si intende come $I$ l'intervallo più grande su cui le funzioni $a$ e $b$ sono definite.

>[!note] Formula risolutiva per le EDO del primo ordine lineari
>Date $a,b:I\subseteq\mathbb{R}\to\mathbb{R}$ continue in $I$, l'integrale generale dell'EDO: $$y'(t)=a(t)\cdot y(t)+b(t)\qquad t\in I$$
>È dato dalla formula: $$y(t)=e^{A(t)}\cdot [B(t)+c]\qquad t\in I$$
>Con $$c\in\mathbb{R}\qquad A(t)=\int a(t)\text{ d}t\qquad B(t)=\int b(t)e^{-A(t)}\text{ d}t$$

>[!example] Dimostrazione
>Svolgiamo 3 passi:
>1. porto a sinistra il termine con la funzione a e moltiplico per $e^{-A}$: $$\begin{align*}
&y'e^{-A}-aye^{-A}=be^{-a}\\
\Longrightarrow & (ye^{-A})'=be^{-A}\\
\end{align*}$$
>Quindi l'EDO del primo ordine lineare è equivalente a $(ye^{-A})'=be^{-A}$
>2. Applico il TFCI e trovo la primitiva su entrambi i membri dell'equazione: $$ye^{-A}=\int be^{-A}+c\qquad c\in\mathbb{R}$$
>3. Moltiplico per $e^{A}$ entrambi i membri: $$y(t)=e^{A}\int be^{-A}$$

>[!tip]
>Le EDO del primo ordine lineari soddisfano il principio di sovrapposizione. Sia $L$ l'operatore: $$y\mapsto Ly:= y'-ay$$
>E osserviamo che è un operatore lineare, cioè: $$\forall c_{1},c_{2}\in \mathbb{R},\quad y_{1},y_{2}: I\subseteq \mathbb{R}\to\mathbb{R}\qquad L(c_{1}y_{1}+c_{2}y_{2})=c_{1}Ly_{1}+c_{2}Ly_{2}$$
>Se $y_{1}$ e $y_2$ sono soluzioni di EDO lineari con termine $b_{1}$ e $b_{2}$, rispettivamente, allora la combinazione lineare $c_{1}y_{1}+c_{2}y_{2}$ è soluzione della EDO lineare con termine noto $c_{1}b_{1}+c_{2}b_{2}$. Di conseguenza, se $y_{1}$ e $y_{2}$ sono soluzioni della EDO lineare omogenea, allora una qualunque combinazione lineare di $y_{1}$ e $y_{2}$ è anche soluzione di tale equazione.

>[!note] Problema di Cauchy
>Siano $I\subseteq\mathbb{R}$, $a,b:I\to\mathbb{R}$ continue, $t_{0}\in I$ e $y_{0}\in \mathbb{R}$. Abbiamo che esiste un unica soluzione $y$ definita su tutto $I$ per il problema di Cauchy: $$\begin{cases}
y'(t)=a(t)y(t)+b(t)\qquad t\in I \\
y(t_{0})=y_{0}
\end{cases}$$
>La soluzione quindi esiste sempre, è unica ed è definita su tutto $I$.

### Equazioni di Bernoulli
>[!note]
>Si chiamano equazioni di Bernoulli le EDO del primo ordine non lineari del tipo: $$y'(t)=g(t)y(t)+h(t)y^{\alpha}(t)\qquad t\in I\subseteq \mathbb{R}$$
>Dove $g,h: I\to\mathbb{R}$ continue, $\alpha\in\mathbb{R}\smallsetminus\set{0,1}$ e $h$ non costantemente nulla.

>[!tip]
>L'equazione di Bernoulli è in forma normale con $$f(t,y):=g(t)y+h(t)y^{\alpha}$$

Per la risoluzione effettuiamo 3 passi:
1. Ricerchiamo delle soluzioni costanti
	Se $\alpha>0,\quad y\equiv0$ è soluzione costante
	Se $h$ e $g$ sono funzioni costanti, allora possiamo formalmente trovare le seguenti soluzioni, e poi controllare se sono ben definite:
	- $\alpha\in(0,1):\qquad y^{\alpha}(gy^{1-\alpha}+h)=0\Longrightarrow y\equiv0, y= \left(- \frac{h}{g}\right)^{\frac{1}{1-\alpha}}$
	- $\alpha>1:\qquad y(g+h^{\alpha-1})=0\Longrightarrow y\equiv 0, y= \left(-\frac{g}{h}\right)^{\frac{1}{\alpha -1}}$
	- $\alpha<0:\qquad gy+ \frac{h}{y^{-1}}=0\Longrightarrow y= \left(- \frac{h}{g}\right)^{\frac{1}{1-\alpha}}$
	Se le funzioni costanti non sono definite non sono da considerare tra le soluzioni
2. Ricerca delle soluzioni non costanti
	2.1: divido la EDO per $y^{\alpha}$: $$\frac{y'(t)}{y^{\alpha}(t)}= g(t)\frac{y'(t)}{y^{\alpha}(t)}+h(t)$$ $$\left(\frac{1}{1-\alpha}\cdot \frac{1}{y^{\alpha-1}}\right)=g \frac{1}{y^{\alpha-1}}+h$$
	2.2: poniamo $z= y^{1-\alpha}(t)$ così da ottenere: $$\frac{1}{1-\alpha} z'(t)=g(t)z(t)+h(t)$$
	$$z'(t)=(1-\alpha)g(t)z(t)+(1-\alpha)h(t)$$
	Che è una EDO lineare con $a(t)= (1-\alpha)g(t)$ e $b(t)=(1-\alpha)h(t)$
	2.3: risolviamo la EDO lineare trovata in $z$ utilizzando la formula del teorema
	2.4 ricavo $y(t)=z(t)^{\frac{1}{1-\alpha}}$
3. Scrivere l'integrale generale mettendo insieme le soluzioni costanti e non costanti

