>[!note]
>Una serie di potenze reali è una serie di funzioni della forma: $$\sum\limits_{n=0}^{+\infty}a_{n}(x-x_{0})^{n}=a_{0}+a_{1}(x-x_{0})+a_{2}(x-x_{0})^{2}+\cdots$$
>Con $a_{n}\in\mathbb{R}$ che viene chiamato coefficiente $n$-esimo della serie e $x_{0}\in\mathbb{R}$ che viene chiamato centro della serie.

>[!tip]
>Tutte le serie di potenze convergono puntualmente per $x=x_{0}$.

### Teorema del raggio di convergenza di una serie di potenze
>[!note]
>Data una serie di potenze: $$\sum\limits_{n=0}^{+\infty}a_{n}(x-x_{0})^{n}$$
>Si verifica sempre una delle seguenti 3 opzioni:
>- La serie converge solo per $x=x_{0}$, e in questo caso diciamo che il raggio di convergenza della serie è nullo
>- La serie converge assolutamente su tutto $\mathbb{R}$ e in questo caso diciamo che il raggio di convergenza della serie è infinito.
>- $\exists R>0$ detto raggio di convergenza tale che la serie converge assolutamente $\forall x$ tale che $|x-x_{0}|<R$, e non converge per $x$ con $|x-x_{0}|>R$.

>[!tip]
>L'insieme di convergenza è sempre un intervallo simmetrico rispetto al centro $x_{0}$ con raggio $R$ in $[0,+\infty)\cup\set{+\infty}$ (a meno degli estremo dell'intervallo). Nel terzo caso bisogna controllare se c'è convergenza per punti $x_{0}\pm R$.

### Teorema del calcolo del raggio di convergenza
>[!note]
>Data la serie di potenze: $$\sum\limits_{n=0}^{+\infty}a_{n}(x-x_{0})^{n}$$
>Abbiamo che se uno dei seguenti limiti esiste:
>$$\begin{align*}
>R&:=\lim_{n\to+\infty} \left| \frac{a_{n}}{a_{n+1}}\right|\\
>R&:=\lim_{n\to+\infty} \frac{1}{\sqrt[n]{|a_{n}|}}
>\end{align*}$$
>Con $R\in[0,+\infty)\cup\set{+\infty}$, allora la serie ha raggio di convergenza $R$.

>[!tip]
>Attenzione che i criteri del rapporto e della radice per serie numeriche $\sum\limits_{n=1}^{k}a_{n}$, che dipendono da: $$\lim_{n\to+\infty}\frac{a_{n+1}}{a_{n}}\text{ e }\lim_{n\to+\infty}\sqrt[n]{|a_{n}|}$$ sono legati a $\frac{1}{R}$. Se esistono entrambi i limiti, allora coincideranno. Dal teorema precedente deduciamo che per $|x-x_{0}|<R$ la convergenza è assoluta, e per $|x-x_{0}|>R$ la serie non converge, mentre per $x_{0}\pm R$ bisogna controllare sia la convergenza puntuale che la convergenza assoluta.

### Convergenza della serie
>[!note]
>Data una serie di potenze: $$\sum\limits_{n=0}^{+\infty}a_{n}(x-x_{0})^{n}$$
>Avente raggio di convergenza $0<R\leq\infty$, si ha:
>- Se $R=+\infty$ la serie converge totalmente in ogni intervallo chiuso $[a,b]\subseteq\mathbb{R}$
>- Se $R\in(0,+\infty)$ la serie converge totalmente in ogni intervallo chiuso $[a,b]\subseteq(x_{0}-R,x_{0}+R)$ per ogni $a,b\in\mathbb{R}\quad a<b$

