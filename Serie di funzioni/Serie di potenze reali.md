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

>[!example] Dimostrazione
>È sufficiente verificare che la serie $\sum\limits_{n=0}^{\infty} |a_{n}(x-x_{0})^{n}|$ converga per $|x-x_{0}|<R$ o non converga per $|x-x_{0}|>R$.
>
>##### Primo caso:
>Osserviamo che $\forall x\in\mathbb{R}$: $$\lim_{n\to+\infty}\sqrt[n]{|a_{n}(x-x_{0})^{n}|}=|x-x_{0}|\cdot\lim_{n\to+\infty}\sqrt[n]{|a_{n}|}= \frac{|x-x_{0}|}{R}$$
>E quindi le condizioni menzionate precedentemente sono conseguenza del criterio della radice per la serie numerica $\sum\limits_{n=0}^{\infty}|a_{n}(x-x_{0})^{n}|$.
>
>##### Secondo caso:
>Osserviamo che tutte le serie di potenze convergono per $x=x_{0}$ e che per $x\neq x_{0}$ abbiamo: $$\lim_{n\to+\infty}\frac{| a_{n+1}(x-x_{0})^{n+1} |}{| a_{n}(x-x_{0})^{n} |}=|x-x_{0}|\cdot\lim_{n\to+\infty}\frac{|a_{n+1}|}{|a_{n}|}$$
>E quindi le condizioni menzionate precedentemente sono conseguenza diretta del criterio del rapporto per la serie numerica $\sum\limits_{n=0}^{\infty}|a_{n}(x-x_{0})^{n}|$.

### Convergenza della serie
>[!note]
>Data una serie di potenze: $$\sum\limits_{n=0}^{+\infty}a_{n}(x-x_{0})^{n}$$
>Avente raggio di convergenza $0<R\leq\infty$, si ha:
>- Se $R=+\infty$ la serie converge totalmente in ogni intervallo chiuso $[a,b]\subseteq\mathbb{R}$
>- Se $R\in(0,+\infty)$ la serie converge totalmente in ogni intervallo chiuso $[a,b]\subseteq(x_{0}-R,x_{0}+R)$ per ogni $a,b\in\mathbb{R}\quad a<b$

### Proprietà della funzione somma
>[!note] Continuità della somma
>Sia $I\subseteq\mathbb{R}$ un intervallo e siano $f_{n}:I\to\mathbb{R}$ funzioni continue in $x_{0}\in I\quad\forall n\in \mathbb{N}$. Se la serie di funzioni $\sum\limits_{n}f_{n}(x)$ converge totalmente in $I$, allora la somma della serie $f(x):=\sum\limits_{n} f_{n}(x)$ è una funzione continua in $x_{0}$. In particolare, se le $f_{n}$ sono continue in tutto $I$, anche $f$ è continua in $I$.
>
>Questa proprietà è una delle motivazioni per l'introduzione della convergenza totale.

>[!tip]
>Data una serie di potenze $\sum\limits_{n=0}^{\infty} a_{n}(x-x_{0})^{n}$ avente raggio di convergenza $0<R<\infty$ si ha che la somma $p(x):=\sum\limits_{n=0}^{\infty}a_{n}(x-x_{0})^{n}$ è una funzione continua in $(x_{0}-R,x_{0}+R)$.
>

>[!note] Derivabilità della somma
>Sia $I\subseteq\mathbb{R}$ un intervallo aperto e siano $f_{n}:I\to\mathbb{R}$ funzioni derivabili in $I\quad\forall n\in\mathbb{N}$. Se La serie $\sum\limits_{n=0}^{\infty}f_{n}(x)$ converge puntualmente $\forall x\in I$ e la serie $\sum\limits_{n=0}^{\infty}f_{n}'(x)$ converge totalmente in $I$ allora la funzione somma $f(x):=\sum\limits_{n}f_{n}(x)$ è derivabile in $I$ e $f'(x)=\sum\limits_{n} f'_{n}(x)$.

>[!tip]
>Data una serie di potenze $\sum\limits_{n=0}^{\infty} a_{n}(x-x_{0})^{n}$ avente raggio di convergenza $0<R<\infty$ si ha che la somma $p(x):=\sum\limits_{n=0}^{\infty}a_{n}(x-x_{0})^{n}$ è derivabile in $(x_{0}-R,x_{0}+R)$ e $p'(x)=\sum\limits_{n=1}^{\infty}n a_{n}(x-x_{0}^{n-1})$. Inoltre la serie derivata è anch'essa una serie di potenze con centro $x_{0}$ con lo stesso raggio di convergenza, e quindi iterando il procedimento $p(x)$ è derivabile $\infty$ volte in $(x_{0}-R,x_{0}+R)$.

>[!note] Integrabilità termine a termine
>Siano $a,b\in\mathbb{R}$ con $a<b$ e siano $f_{n}:[a,b]\to\mathbb{R}$ funzioni continue in $[a,b]\quad\forall n\in\mathbb{N}$. Se $\sum\limits_{n} f_{n}(x)$ converge totalmente in $[a,b]$, allora la somma $f(x)=\sum\limits_{n=1}^{\infty} f_{n}(x)$ è una funzione integrabile e: $$\int^{b}_{a}f(x)\text{ d}x=\sum\limits_{n=1}^{\infty} \left(\int_{a}^{b}f_{n}(x)\text{ d}x\right)$$
>Possiamo scambiare il segno di integrazione con la sommatoria sotto tali condizioni.

>[!tip]
>Data una serie di potenze $\sum\limits_{n=0}^{\infty} a_{n}(x-x_{0})^{n}$ avente raggio di convergenza $0<R<\infty$ si ha che la somma $p(x):=\sum\limits_{n=0}^{\infty}a_{n}(x-x_{0})^{n}$ è soddisfa i seguenti assetti:
>- $p(x)$ ammette primitiva in $(x_{0}-R,x_{0}+R)$ che può essere calcolata "termine a termine", è una serie di potenze centrata in $x_{0}$ e con raggio di convergenza $R$: $$\int_{x_{0}}^{x} p(s)\text{ d}s=\sum\limits_{n=0}^{\infty} \int_{x_{0}}^{x} a_{n}(s-x_{0})^{n}\text{ d}s=\sum\limits_{n=0}^{\infty} \frac{a_{n}}{n+1}(x-x_{0})^{n+1}\quad\forall x\in(x_{0}-R,x_{0}+R)$$
>- $\forall a,b\in\mathbb{R}$ con $a<b$ la funzione $p(x)$ è integrabile su $[a,b]$ e: $$\int^{b}_{a}p(x)\text{ d}x=\sum\limits_{n=0}^{+\infty}\int_{a}^{b} a_{n}(x-x_{0})^{n}\text{ d}x$$

### Serie di Taylor
>[!note]
>Data una funzione $f:(a,b)\subseteq\mathbb{R}\to\mathbb{R}$ derivabile $n$ volte in $x_{0}\in(a,b)$, si dice polinomio di Taylor $T_{n,x_{0}}$ di grado $n$ in $x_{0}$ il polinomio definito da: $$T_{n,x_{0}}(x):=\sum\limits_{k=0}^{n}\frac{f^{(k)}(x_{0})}{k!}(x-x_{0})^{k}$$
>Inoltre abbiamo che: $$f(x)=T_{n,x_{0}}+o((x-x_{0})^{n})$$
>In caso la funzione sia derivabile $n+1$ volte, allora $\exists c$ compreso tra $x$ e $x_{0}$ tale che: $$f(x)=T_{n,x_{0}}(x)+\frac{f^{(n+1)}(c)}{(n+1)!}(x-x_{0})^{n+1}$$

Se la funzione $f$ è derivabile $\infty$ volte in $x_{0}\in(a,b)$. Si chiama serie di Taylor con centro $x_{0}$ della funzione $f$ la serie di potenze definita da: $$\sum\limits\frac{f^{(n)}(x_{0})}{n!}(x-x_{0})^{n}$$Dove i coefficiente sono detti coefficienti di Taylor, e se $x_{0}$ la serie viene detta serie di McLaurin.

>[!tip]
>Osserviamo che per $x=x_{0}$ la serie converge a $f(x_{0})$.

Sia $f:(a,b)\subseteq\mathbb{R}\to\mathbb{R}$ derivabile $\infty$ volte in $x_{0}\in(a,b)$. Si dice che $f$ è una funzione analitica in $x_{0}$ (o anche sviluppabile in serie di Taylor centrata in $x_{0}$) se la serie di Taylor con centro $x_{0}$ e raggio di convergenza $R\in(0,+\infty)\cup\set{+\infty}$ esiste $R_{0}\in(0,R]$ tale che: $$f(x)=\sum\limits_{n=0}^{+\infty} \frac{f^{(n)}(x)}{n!}(x-x_{0})^{n}$$
Per ogni $x\in(x_{0}-R_{0},x_{0}+R_{1})$.

### Serie di potenze in $\mathbb{C}$
>[!note]
>Una serie di potenze in $\mathbb{C}$ è una serie di funzioni della forma: $$\sum\limits_{n=0}^{\infty} a_{n}(z-z_{0})^{n}$$
>Con $a_{n}\in\mathbb{C}$ chiamati coefficienti della serie, $z_{0}\in\mathbb{C}$ chiamato centro della serie e $z\in\mathbb{C}$ è la variabile della serie.

Osserviamo che le nozioni di convergenza puntuale, assoluta e totale si trasportano direttamente dal caso reale alle serie di potenze complesse con la stessa definizione.

>[!tip] Raggio di convergenza per serie di potenze in $\mathbb{C}$
>Data una serie di potenze $\sum\limits_{n=0}^{\infty} a_{n}(z-z_{0})^{n}$ in $\mathbb{C}$ si verifica sempre una delle seguenti tre opzioni:
>- La serie converge solo per $z=z_{0}$ (raggio di convergenza nullo)
>- La serie converge assolutamente $\forall z\in\mathbb{C}$ (raggio di convergenza infinito)
>- Esiste $R\in(0,+\infty)$ detto raggio di convergenza tale che la serie converge assolutamente $\forall z\in\mathbb{C}$ tale che $|z-z_{0}|<R$, e non converge $\forall \in\mathbb{C}$ tale che $|z-z_{0}|>R$.

Siccome $\mathbb{C}$ è isomorfo a $\mathbb{R}^{2}$, possiamo rappresentare ogni numero complesso su un piano e l'intorno di convergenza per una serie di potenze con centro $z_{0}\in\mathbb{C}$ e raggio $R>0$ è la palla: $$B_{R}(z_{0}):=\set{z\in\mathbb{C}:\quad|z-z_{0}|<R}$$
Come nel caso reale bisogna studiare separatamente la convergenza sul bordo dell'intorno di convergenza, che è: $$\partial B_{R}(Z_{0})=\set{z\in\mathbb{C}:\quad|z-z_{0}|=R}$$
Per calcolare il raggio di convergenza $R$ rimane valido il teorema relativo del caso reale.

>[!tip] Formula di Eulero
>La serie esponenziale in $\mathbb{C}$ è: $$\sum\limits_{n=0}^{\infty} \frac{z^{n}}{n!}\quad z\in\mathbb{C}$$
>Con la stessa verifica effettuata nel caso reale otteniamo che il raggio di convergenza è $R=+\infty$. Anche analogamente al caso reale, si verifica che: $$e^{z}=\sum\limits_{n=0}^{\infty} \frac{z^{n}}{n!}\quad \forall z\in\mathbb{C}$$
>Questo ci permette di ricavare la formula di Eulero: $$\begin{align*}
>e^{ix} &= \sum\limits_{n=0}^{\infty} \frac{(ix)^{n}}{n!}= \frac{(ix)^{0}}{0!}+ \frac{(ix)^{1}}{1!}+ \frac{(ix)^{2}}{2!}+\cdots\\
>&= 1+ ix- \frac{x^{2}}{2}-i \frac{x^{3}}{3!}+ \frac{x^{4}}{4!}+i \frac{x^{5}}{5!}- \frac{x^{6}}{6!}+\cdots\\
>&= \left(1- \frac{x^{2}}{2}+ \frac{x^{4}}{4!}- \frac{x^{6}}{6!}+\cdots\right)+ i\left(x- \frac{x^{3}}{3!}+ \frac{x^{5}}{5!}+\cdots\right)\\
>&= \cos x+i\sin x
>\end{align*}$$
>Quindi: $$e^{ix}=\cos(x)+i\sin(x)\quad\forall x\in\mathbb{R}$$

