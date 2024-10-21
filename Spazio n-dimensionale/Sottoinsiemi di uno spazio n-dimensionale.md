>[!note] Punti di un sottoinsieme
>Sia $E$ un sottoinsieme di $\mathbb{R}^{n}$, e sia $\overrightarrow{x}_{0}\in\mathbb{R}^{n}$:
>
>- $\overrightarrow{x}_{0}$ si dice interno ad $E$ se $$\exists r>0:\quad B_{r}(\overrightarrow{x}_{0})\subseteq E$$L'insieme dei punti interni di $E$ è indicato con $\text{Int}(E)$.
>- $\overrightarrow{x}_{0}$ si dice di frontiera (o di bordo) ad $E$ se $$\forall r>0:\quad B_{r}(\overrightarrow{x}_{0})\cap E\neq\emptyset\text{ e }B_{r}(\overrightarrow{x}_{0})\cap E^{C}=B_{r}(\overrightarrow{x}_{0})\smallsetminus E\neq\emptyset$$ L'insieme dei punti di frontiera formano la frontiera (o bordo) di $E$ ed è indicato con $\partial E$.
>- $\overrightarrow{x}_{0}$ si dice esterno ad $E$ se: $$\overrightarrow{x}_{0}\notin E\text{ e }\exists r>0:\quad B_{r}(\overrightarrow{x}_{0})\subseteq E^{C}$$ 

>[!note] Tipologie di sottoinsiemi
>Sia $E\subseteq\mathbb{R}^{n}$. $E$ si dice:
>- Aperto se $\forall \overrightarrow{x}\in E$ si ha che $\overrightarrow{x}$ è interno ad $E$, e quindi $E=\text{Int}(E)$.
>- Chiuso se $E^{C}$ è aperto.
>  
>Possono esistere insiemi che non sono ne aperti ne chiusi: $\mathbb{R}^{n}$ e $\emptyset$ si considerano sia aperti che chiusi.

>[!tip] Chiusura
>Chiamiamo chiusura $\overline{E}$ di un insieme $E\subseteq\mathbb{R}^{n}$ l'insieme: $$\overline{E}:=\text{Int}(E)\cup \partial E$$
>La chiusura di un insieme è sempre un insieme chiuso, se $E$ è chiuso, allora la chiusura $\overline{E}=E$.

### Punti di accumulazione
>[!note]
>Sia $E\subseteq\mathbb{R}^{n}$ e $\overrightarrow{x}_{0}\in\mathbb{R}^{n}$. Diciamo che $\overrightarrow{x}_{0}$ è un punto di accumulazione per $E$ (punto di accumulazione) se $\forall n>0$ si ha che $(B_{r}(\overrightarrow{x}_{0})\cap E)\smallsetminus\set{\overrightarrow{x}_{0}}\neq0$.

