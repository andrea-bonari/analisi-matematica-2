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

>[!example] Dimostrazione
>Dal principio di sovrapposizione deduciamo che l'insieme di tutte le soluzioni è uno spazio vettoriale (perché è chiuso rispetto alla somma di soluzioni e al prodotto per uno scalare). Per dimostrare che la dimensione è $2$ dobbiamo:
>1) Determinare due soluzioni linearmente indipendenti $y_{\sigma1}$ e $y_{\sigma2}$
>2) Verificare che ogni soluzione $\overline{y}_{\sigma}(t)$ si possa scrivere come combinazione lineare di $y_{\sigma1}$ e $y_{\sigma2}$
>
>Per soddisfare la prima condizione, fissiamo $t_{0}\in I$ e scegliamo $y_{\sigma1}$ e $y_{\sigma2}$ come soluzioni di due problemi di Cauchy, rispettivamente, $y_{\sigma1}$ come soluzione di: $$\begin{cases}
>a(t)y''(t)+b(t)y'(t)+c(t)y(t)=0 \\
>y(t_{0})=1 \\
>y'(t_{0})=0
>\end{cases}$$
>E $y_{\sigma2}$ come soluzione di: $$\begin{cases}
>a(t)y''(t)+b(t)y'(t)+c(t)y(t)=0 \\
>y(t_{0})=0 \\
>y'(t_{0})=1
>\end{cases}$$
>Tali soluzioni esistono grazie al teorema di esistenza e unicità globale per il problema di Cauchy. Verifichiamo adesso che $y_{\sigma1}$ e $y_{\sigma2}$ sono linearmente indipendenti assumendo per assurdo che $\exists c\neq0$ tale che $y_{\sigma1}(t)=c\times y_{\sigma2}(t)\quad \forall t\in I$. Per la definizione di $y_{\sigma1}$ e $y_{\sigma2}$ abbiamo che: $$1=y_{\sigma1}(t_{0})=c\cdot y_{\sigma2}(t_{0})=c\cdot 0$$
>Che è una contraddizione.
>
>Per soddisfare la seconda condizione, sia $\overline{y}_{\sigma}$ una qualunque soluzione particolare e cerchiamo costanti $c_{1},c_{2}\in\mathbb{R}$ per cui $\overline{y}_{\sigma}$ coincida con la funzione: $$Z(t):=c_{1}y_{\sigma1}(t)+c_{2}y_{\sigma2}(t)$$
>Che è soluzione per il principio di sovrapposizione per ogni $t$. Scegliamo $c_{1}$ e $c_{2}$ in maniera tale che $\overline{y}_{\sigma}(t_{0})=Z(t_{0})$ e $\overline{y}_{\sigma}\space'(t_{0})=Z'(t_{0})$, cioè poniamo: $$\begin{cases}
>\overline{y}_{\sigma}(t_{0})=Z(t):=c_{1}y_{\sigma1}(t)+c_{2}y_{\sigma2}(t)=c_{1} \\
>\overline{y}_{\sigma}'(t_{0})=Z'(t):=c_{1}y'_{\sigma1}(t)+c_{2}y'_{\sigma2}(t)=c_{2}
>\end{cases}$$
>E otteniamo $c_{1}=\overline{y}_{\sigma}(t_{0})$ e $c_{2}=\overline{y}_{\sigma}(t_{0})$. Quindi la combinazione lineare $Z(t)$ candidata a coincidere con $\overline{y}_{\sigma}$ è: $$\overline{Z}(t)=\overline{y}_{\sigma}(t_{0})y_{\sigma}(t)+\overline{y}_{\sigma1}'(t_{0})y_{\sigma2}(t)$$
>Concludiamo osservando che sia $\overline{Z}(t)$ che $\overline{y}_{\sigma}(t)$ sono soluzioni dello stesso problema di Cauchy: $$\begin{cases}
>a(t)y''(t)+b(t)y'(t)+c(t)y(t)=0 \\
>y(t_{0})=\overline{y}_{\sigma}(t_{0}) \\
>y'(t_{0})=\overline{y}'_{\sigma}(t_{0})
>\end{cases}$$
>E quindi per il teorema di esistenza e unicità globale del problema di Cauchy abbiamo che $$\overline{y}_{\sigma}(t)=\overline{Z}(t)\qquad\forall t\in I$$

