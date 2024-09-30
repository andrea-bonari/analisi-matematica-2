>[!note]
>Un'EDO del secondo ordine si dice a lineare se è nella forma: $$a(t)y''(t)+b(t)y'(t)+c(t)y(t)=f(t)$$
>Con $a,b,c,f: I\subseteq\mathbb{R}\to\mathbb{R}$ funzioni continue. e $a\neq0$.
>Si dice omogenea quando $f(t)=0$, e l'omogenea associata di un equazione si trova imponendo $f(t)=0$.

>[!tip]
>Un'EDO del secondo ordine ha infinite soluzioni dipendenti da due parametri.

### Principio di sovrapposizione
>[!note]
>Se $y_{1}$ è soluzione di $ay''+by'+cy=f_{1}$ e $y_{2}$ è soluzione di $a''+b'+cy=f_{2}$, allora la funzione $$y(t)=C_{1}y_{1}(t)+C_{2}y_{2}(t)$$è soluzione di $$ay''+by'+cy=C_{1}f_{1}+C_{2}f_{2}$$

>[!example] Dimostrazione
>Il primo membro dell'equazione può essere visto come un operatore chiamato $L$, ponendo $Ly$ come $ay''+by+cy$. Questo operatore gode di una proprietà di linearità:
$$L(C_{1}y_{1}+C_{2}y_{2})=C_{1}Ly_{1}+C_{2}Ly_{2}$$
Data questa proprietà possiamo definire l'equazione come lineari. A queste operazioni possiamo quindi applicare il principio di sovrapposizione. Per questo possiamo affermare che: $$\begin{align*}
&C_{1}Ly_{1}+C_{2}Ly_{2}=C_{1}f_{1}+C_{2}f_{2}\\
\Longrightarrow & L(C_{1}y_{1}+C_{2}y_{2})=C_{1}f_{1}+C_{2}f_{2}\\
\Longrightarrow & L(y)=C_{1}f_{1}+C_{2}f_{2}
\end{align*}$$

### Teorema di struttura
>[!note]
>L'integrale generale di  $a(t)y''+b(t)y'+c(t)y=0$ con $a,b,c$ funzioni continue in $I$ e $a(t)\neq0$ in $I$ è dato da tutte le combinazioni lineari $$y(t)=C_{1}y_{1}(t)+C_{2}y_{2}(t)\qquad \forall C_{1},C_{2}\in\mathbb{R}$$
>Dove $y_{1},y_{2}$ sono due soluzioni linearmente indipendenti dell'equazione stessa.

Possiamo dire che le soluzioni di $Ly$ sono: $$y(t)=y_{0}(t)+y_{P}(t)$$
Dove $y_{P}$ è soluzione di $Ly=f$, e $y_{0}$ è soluzione di $Ly=0$.
