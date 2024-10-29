>[!note]
>Dato un intervallo $J\subseteq\mathbb{R}$, siano $f_{n}:J\to\mathbb{R}$ funzioni per ogni $n\in\mathbb{N}$ (oppure $n\in \mathbb{N}_{0}=\mathbb{N}\cup\set{0}$). La serie di funzioni di termine generale $f_{n}(x)$ è la successione delle somme parziali definita da: $$S_{k}(x)=\sum\limits_{n=0}^{k}f_{n}(x)$$

>[!tip]
>Fissato un punto $\overline{x}\in J$, si ha che la serie di termine generale $f_{n}(\overline{x})$ è una serie numerica. Abbiamo quindi $\infty$ serie numeriche, una per ogni $x\in J$. 

### Convergenza semplice
>[!note]
>Diciamo che la serie di funzioni di termine generale $f_{n}(x)$, $x\in J\subseteq\mathbb{R}$, converge puntualmente (o semplicemente) nel punto $\overline{x}\in J$ se la serie numerica di termine generale $f_{n}(\overline{x})$ è convergente, cioè se esiste finito il limite: $$\exists\lim_{k\to+\infty} S_{k}(\overline{x})=\lim_{k\to+\infty}\sum\limits_{n=0}^{k}f_{n}(\overline{x})\in\mathbb{R}$$
>
>L'insieme $E\subseteq J$ dei punti $x$ in cui la serie converge puntualmente è detto insieme di convergenza puntuale (o semplice) della serie. Nell'insieme $E$ risulta definita la somma della serie, cioè: $$f(x):=\sum\limits_{n=0}^{+\infty} f_{n}(x)=\lim_{k\to+\infty} S_{k}(x)$$

>[!tip]
>Una serie di funzioni può essere convergente per alcuni $x\in J$ e divergente per altri $x\in J$, o anche indeterminata.

Si usa indicare con $\sum\limits_{n=0}^{+\infty}f_{n}(x)$ sia la somma che la serie, però si intende comunque che:
- La serie di funzioni è la successione delle somme parziali
- La somma della serie è una funzione con dominio l'insieme di convergenza

In alternativa si potrebbe indicare la somma come: $$\sum\limits_{n=0}^{+\infty}f_{n}: E\to \mathbb{R}$$
### Convergenza assoluta
>[!note]
>La serie di funzioni di termine generale $f_{n}(x)$, $x\in J$ converge assolutamente nel punto $\overline{x}\in J$ se la serie di termine generale $|f_{n}(x)|$ è convergente puntualmente in $\overline{x}\in J$.

>[!tip]
>Se la serie converge assolutamente in $\overline{x}\in J$, allora converge puntualmente in $\overline{x}\in J$, in quanto $$0\leq |\sum\limits_{n=0}^{k}f_{n}(\overline{x})|\leq\sum\limits_{n=0}^{k}|f_{n}(\overline{x})|$$

Per convenzione assumiamo che $0^{0}=1$.

### Convergenza totale
>[!note]
>La serie di termine generale $f_{n}(x)\quad x\in J$, converge totalmente in un intervallo $I\subseteq J$ se esiste una successione numerica $(a_{n})\in\mathbb{R}$ tale che:
>- $|f_{n}(x)|\leq a_{n}\qquad \forall n,\quad\forall x\in I$
>- La serie numerica con termine generale $a_{n}$, cioè $\sum\limits_{n} a_{n}$, è convergente.

>[!tip]
>Se $J=\mathbb{R}$, allora $I$ può essere $I\subseteq\mathbb{R}$, cioè la convergenza totale dipende dall'intervallo $I$, $f_{n}$ converge totalmente in i se e solo se: $$\sum\limits_{n}\left(\sup_{x\in I}|f_{n}(x)|\right)<\infty$$

