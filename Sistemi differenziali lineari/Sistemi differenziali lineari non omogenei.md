>[!note]
>Un SDL non omogeneo è un sistema differenziale lineare definito come: $$\overrightarrow{y}\space'(t)=A(t)\cdot \overrightarrow{y}(t) + \overrightarrow{b}(t)\qquad t\in I$$

### Teorema di struttura per SDL non omogenei
>[!note]
>Dati $A: I\subseteq\mathbb{R}\to M_{n\times n}$ e $\overrightarrow{b}:I\to\mathbb{R}^{n}$ continui, l'integrale generale del sistema completo: $$\overrightarrow{y}\space'(t)=A(t)\cdot \overrightarrow{y}(t) + \overrightarrow{b}(t)\qquad t\in I$$è: $$\overrightarrow{y}(t)=\overrightarrow{y}_{\sigma}(t)+\overrightarrow{y}_{p}(t)$$
>Dove $\overrightarrow{y}_{\sigma}(t)$ è l'integrale generale del SDL omogeneo associato e $\overrightarrow{y}_{p}(t)$ è una soluzione particolare del sistema completo.

Possiamo usare il metodo di somiglianza per trovare la soluzione particolare $\overrightarrow{y}_{p}$.

Generalizzando la formula dell'integrale generale nel caso omogeneo otteniamo: $$\overrightarrow{y}(x)= W(x) \left(\int [w(s)]^{-1}\cdot \overrightarrow{b}(s)\text{ d}s + \overrightarrow{c} \right)$$
In particolare, nel caso $A$ sia diagonalizzabile possiamo scrivere $\overrightarrow{y}_{\sigma}$ anche come: $$\overrightarrow{y}_{\sigma}(x)=e^{Ax}\cdot\overrightarrow{c}\space'$$
Con $\overrightarrow{c}\space'\in\mathbb{R}^{n}$, e quindi abbiamo che: $$W(x)= c_{0}e^{Ax}$$
Con $c_{0}\in\mathbb{R}\smallsetminus\set{0}$. Quindi: $$\overrightarrow{y}(x)=c_{0}e^{Ax}\left(\int\left[c_{0}e^{As} \right]^{-1}\cdot \overrightarrow{b}(s)\text{ d}s+\overrightarrow{c}\right)$$
Semplificando $c_{0}$ e usando un po di algebra otteniamo: $$\overrightarrow{y}(x)=e^{Ax}\left(\int a^{-As}\cdot\overrightarrow{b}(s)\text{ d}s+\overrightarrow{c} \right)$$
Con $\overrightarrow{c}\in\mathbb{R}^{n}$ vettore costante.

