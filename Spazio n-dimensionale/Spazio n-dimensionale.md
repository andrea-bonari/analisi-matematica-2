>[!note]
>Definiamo $\mathbb{R}^{n}:=\underbrace{\mathbb{R}\times\cdots\times\mathbb{R}}_{n\text{ volte}}=\set{\overrightarrow{x}=\begin{pmatrix}x_{1}\\\vdots\\x_{n}\end{pmatrix}:\quad x_{i}\in\mathbb{R},i=1,\cdots,n}$ come spazio vettoriale di dimensione $n$, la cui base canonica è: $$e_{1}:=\begin{pmatrix}1\\0\\\vdots\\0\end{pmatrix}\quad e_{2}:=\begin{pmatrix}0\\1\\\vdots\\0\end{pmatrix}\quad\cdots e_{n}:=\begin{pmatrix}0\\0\\\vdots\\1\end{pmatrix}\quad$$

### Operazioni nello spazio n-dimensionale
>[!tip] Prodotto scalare
>Dati $\overrightarrow{x},\overrightarrow{y}\in\mathbb{R}^{n}$ definiamo il loro prodotto scalare come: $$\langle\overrightarrow{x},\overrightarrow{y}\rangle:= \overrightarrow{x}\cdot\overrightarrow{y}\space^{T}=\begin{pmatrix}x_{1}\\\vdots\\x_{n}\end{pmatrix}\cdot\begin{pmatrix}y_{1}&\cdots&y_{n}\end{pmatrix}=x_{1}y_{1}+\cdots+x_{n}y_{n}$$
>Diciamo che: $$\overrightarrow{x}\perp\overrightarrow{y}\iff \langle\overrightarrow{x},\overrightarrow{y}\rangle=0$$

>[!tip] Norma
>Dato $\overrightarrow{x}\in\mathbb{R}^{n}$ definiamo la sua norma come: $$||\overrightarrow{x}||:=\sqrt{\langle\overrightarrow{x},\overrightarrow{x}\rangle}=\sqrt{x_{1}^{2}+\cdots+x_{n}^{2}}$$

>[!tip] Distanza
>Dati $\overrightarrow{x},\overrightarrow{y}\in\mathbb{R}^{n}$ definiamo la loro distanza come: $$\text{dist}(\overrightarrow{x},\overrightarrow{y}):=||\overrightarrow{y}-\overrightarrow{x}||=\sqrt{(y_{1}-x_{1})^{2}+\cdots+(y_{n}-x_{n})^{2}}$$

>[!tip] Palla centrata
>Dato $\overrightarrow{x}_{0}\in\mathbb{R}^{n}$ e un numero $r>0$, definiamo palla centrata in $\overrightarrow{x_{0}}$ di raggio $r$ l'insieme: $$B_{r}(\overrightarrow{x}_{0}):=\set{\overrightarrow{x}\in\mathbb{R}^{n}:\quad\text{dist}(\overrightarrow{x},\overrightarrow{x}_{0})<r}\subseteq\mathbb{R}^{n}$$
### Teoremi importanti dello spazio n-dimensionale
>[!note] Disuguaglianza triangolare
>$$\forall\overrightarrow{x},\overrightarrow{y}\in\mathbb{R}^{n}\qquad ||\overrightarrow{x}+\overrightarrow{y}||\leq ||\overrightarrow{x}||+||\overrightarrow{y}||$$

>[!note] Disuguaglianza di Cauchy-Schwarz
>$$\forall\overrightarrow{x},\overrightarrow{y}\in\mathbb{R}^{n}\qquad |\langle\overrightarrow{x},\overrightarrow{y}\rangle|\leq ||\overrightarrow{x}||\cdot||\overrightarrow{y}||$$
