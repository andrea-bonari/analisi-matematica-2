>[!note]
>Un equazione differenziale ordinaria (EDO o ODE) di ordine $n$ è un equazione che ha come incognita una funzione $y(t)$ che coinvolge la derivata $n$-esima di $y$ e può coinvolgere le derivate $j$-esime con $0\leq j<n$, cioè si può scrivere nella forma: $$F(t, \space y(t),\space y'(t),\space\cdots,\space y^{(n)}(t))=0\qquad t\in I$$
>Dove $I$ è un intervallo in $\mathbb{R}$ e $F$ è una funzione in $n+2$ variabili.
>
>Inoltre sono dette soluzioni particolari della EDO in un intervallo $J\subset I$ ogni funzione $\overline{y}(t)\in C^{n}(j)$, cioè continua con derivate continue fino all'ordine $n$, che soddisfi la precedente equazione. L'insieme di tutte le soluzioni si dice integrale generale della EDO.

>[!tip]
>In generale le EDO hanno $\infty$ soluzioni per via della costante $c$.

>[!tip]
>La soluzione di un'EDO dipende anche dall'intervallo di definizione (anch'esso è incognita). L'intervallo di definizione della funzione può essere più piccolo dell'intervallo della EDO.

### Forma normale
>[!note]
>Un'EDO di ordine $n$ è in forma normale se è nella forma:
>$$y^{(n)}(t)=f(t,\space y(t),\space\cdots,\space y^{(n-1)}(t))\qquad t\in I$$
>Cioè, è in forma normale se esplicitiamo la derivata di ordine massimo.

### Problema di Cauchy
>[!note]
>Data un'EDO di ordine $n$ in forma normale, cioè: $$y^{(n)}=f(t, \space y(t),\space\cdots,\space y^{(n-1)}(t))\qquad t\in I$$
>Per un dato intervallo $I\subseteq\mathbb{R}$, data una funzione $f$ con dominio $A$: $$A:= I\times B\qquad B\subseteq \mathbb{R}^{n}$$
>E dato un punto $(t_{0}, \space y_{0},\space y_{0}^{1},\space\cdots,\space y_{0}^{n-1})\in A$, si dice problema di Cauchy associato alla EDO il problema che consiste nel determinare una soluzione particolare: $$\overline{y}=J\to\mathbb{R}$$
>Della EDO per un intervallo $J\subseteq I$, tale che $t_{0}\in J$ e che soddisfi il sistema: $$\begin{cases}
y^{(n)}(t)= f(t, \space y(t),\space \cdots,\space y^{(n)}(t)) \\
y(t_{0})=y_{0} \\
y'(t_{0})=y_{0}^{1} \\
\qquad\vdots \\
y^{(n-1)}(t_{0})=y_{0}^{n-1}
\end{cases}$$

>[!tip]
>Nel problema di Cauchy servono tante condizioni quante costanti compaiono nell'integrale generale dell'EDO associata. Nel caso $n=1$ c'è una sola costante e quindi mi basta la condizione $y(t_{0})=y_{0}$.

Risoluzione di un problema di Cauchy:
1. Determinare l'integrale generale dell'EDO
2. Sostituisco l'integrale generale nel sistema e determino le costanti presenti nell'integrale generale
3. Sostituisco il valore delle costanti trovate al passo 2 nell'integrale generale del passo 1
