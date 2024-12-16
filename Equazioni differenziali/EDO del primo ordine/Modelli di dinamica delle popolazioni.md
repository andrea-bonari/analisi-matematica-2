### Modello di Malthus
>[!note]
>Si tratta di un modello di crescita delle popolazioni assumendo che la popolazione evolva isolata e i suoi fattori di evoluzione quindi siano esclusivamente la natalità e la mortalità.
>Indichiamo $N(t)$ il numero di membri della popolazione al tempo $t$, quindi:$$N:\mathbb{R}\to \mathbb{R}_{+}:=\set{r\in\mathbb{R}\quad r\geq 0}$$
>Il tasso di natalità come $\lambda>0$ e il tasso di mortalità come $\mu>0$. Il modello è quindi: $$N'(t)=(\lambda-\mu)N(t)$$
Definendo $\varepsilon=\lambda-\mu$ il tasso di potenziali biologica, allora l'EDO è equivalente a: $$N'(t)=\varepsilon N(t)$$
Questa è un EDO a variabili separabili.

>[!example]
>Se $\varepsilon=0$, allora è banale: $$N'(t)=0\qquad N(t)=c\geq0$$
>Se $\varepsilon\neq0$, allora usiamo il metodo a variabili separabili:
>La soluzione costante è: $$N=0$$
>Quando $N\neq0$:
>$$\begin{align*}
&\int^{t}_{t_{0}} \frac{\text{ d} N}{N}=\int^{t}_{t_{0}}\varepsilon \text{ d}N\\
\Longrightarrow&\bigg[\log(N)\bigg]^{t}_{t_{0}}=\varepsilon(t-t_{0})\\
\Longrightarrow&\log\left( \frac{N(t)}{N(t_{0})}\right)=\varepsilon(t-t_{0})\\
\Longrightarrow& N(t)=N(t_{0})e^{\varepsilon(t-t_{0})}
\end{align*}$$
>L'integrale generale è: $$N(t)\equiv0\quad t\in\mathbb{R},\qquad N(t)=N(t_{0})e^{\varepsilon(t-t_{0})}\quad t\in\mathbb{R}$$

>[!tip]
>Abbiamo trovato 3 comportamenti che dipendono da $\varepsilon$ e $N(t_{0})$:
>1. $N(t_{0})=0$ o $\varepsilon=0$: abbiamo che la popolazione rimane costante.
>2. $N(t_{0})\neq0$ e $\varepsilon>0$: la popolazione cresce esponenzialmente
>3. $N(t_{0})\neq0$ e $\varepsilon<0$: la popolazione si estingue esponenzialmente

### Equazione logistica
>[!note]
>L'equazione logistica (o modello di Verhulst) considera che il tasso di nuovi nati è sia proporzionale al numero di popolazione presente, ma anche all'ammontare di risorse disponibili: $$N'(t)=\lambda N(t)- g( N(t))$$
>con $g$ una funzione opportuna, per esempio $g(N)=\sigma N^{2}$, dove $\lambda,\sigma>0$, cioè: $$N'(t)=\lambda N(t)-\sigma N^{2}(t)$$
