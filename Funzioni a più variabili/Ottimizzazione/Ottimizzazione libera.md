>[!note]
>Si parla di ottimizzazione libera quando si cercano i punti estremali di $f$ nel suo dominio.

### Teorema di Fermat
>[!note]
>Sia $A\subseteq\mathbb{R}^{2}$ un insieme aperto e sia $f: A\to\mathbb{R}$ derivabile in $(x_{0},y_{0})\in A$. Se $(x_{0},y_{0})$ è un punto estremale relativo di $f$, allora: $$\nabla f(x_{0},y_{0})=0$$
>Cioè $(x_{0},y_{0})$ è un punto critico di $f$.

### Criterio della matrice Hessiana
>[!note]
>Siano $A\subseteq\mathbb{R}^{n}$ aperto, $f\in c^{2}(A)$ e $\overrightarrow{x}_{0}\in A$ punto critico di $f$. sia $q:\mathbb{R}^{n}\to\mathbb{R}$ la forma quadratica indotta dalla matrice Hessiana $H_{f}(\overrightarrow{x}_{0})$. Abbiamo che:
>- Se $q$ è definita positiva, allora $\overrightarrow{x}_{0}$ è punto di minimo locale.
>- Se $q$ è definita negativa, allora $\overrightarrow{x}_{0}$ è punto di massimo locale.
>- Se $q$ è indefinita, allora $\overrightarrow{x}_{0}$ è punto di sella.

>[!example] Dimostrazione
>Verifichiamo il primo caso (il secondo è analogo).
>La matrice Hessiana $H_{f}(\overrightarrow{x}_{0})$ è:
>- Simmetrica: grazie al teorema di Schwarz siccome $f\in c^{2}(A)$.
>- Ha tutti gli autovalori reali e positivi, siccome $q$ è definita positiva.
>
>Ne deduciamo che: $$\langle\overrightarrow{h}, H_{f}(\overrightarrow{x}_{0})\cdot \overrightarrow{h}\rangle=: q(\overrightarrow{h})\geq\lambda_{\min}||h||^{2}\qquad \forall\overrightarrow{h}\in \mathbb{R}^{n} $$
>Dove $\lambda_{\min}$ è il minimo degli autovalori di $H_{f}(\overrightarrow{x}_{0})$. Inoltre, dato che $\overrightarrow{x}_{0}$ è punto critico di $f$, dalla formula di Taylor al secondo ordine otteniamo che: $$f(\overrightarrow{x}_{0}+h)-f(\overrightarrow{x}_{0})=\frac{1}{2} q(\overrightarrow{h})+ o(||\overrightarrow{h}||^{2})\geq \frac{\lambda_{\min}}{2}||h||^{2}+o(||\overrightarrow{h}||^{2})$$
>Per $||h||\to0$, dove nella disuguaglianza abbiamo applicato la formula precedente. Per la definizione di o piccolo abbiamo che: $$\lim_{\overrightarrow{h}\to\overrightarrow{0}}\frac{o(||\overrightarrow{h}||^{2})}{||\overrightarrow{h}||^{2}}=0$$
>E quindi $\exists\delta>0$ tale che se $||\overrightarrow{h}||<\delta$ e $\overrightarrow{h}\neq\overrightarrow{0}$, allora: $$\frac{|o(||\overrightarrow{h}||^{2})|}{||\overrightarrow{h}||^{2}}< \frac{1}{4}\lambda_{\min}$$
>Dove $\lambda_{\min}>0$ grazie alla seconda ipotesi. Quindi in particolare $\exists\delta>0$ tale che $\forall \overrightarrow{h}\in B_{\delta}(\overrightarrow{0})$ abbiamo che: $$o(||\overrightarrow{h}||^{2})> - \frac{1}{4}\lambda_{\min}||\overrightarrow{h}||^{2}$$
>Pertanto dalle formule precedenti possiamo concludere che $$\begin{align*}
>f(\overrightarrow{x}_{0}+\overrightarrow{h})-f(\overrightarrow{x})&\geq \frac{1}{2}\lambda_{\min}||\overrightarrow{h}||^{2}+o(||\overrightarrow{h}||^{2})\\
>&\geq \frac{1}{2}\lambda_{\min}||\overrightarrow{h}||^{2}- \frac{1}{4}\lambda_{\min}||\overrightarrow{h}||^{2}= \frac{1}{4}\lambda_{\min}||\overrightarrow{h}||^{2}\geq0
>\end{align*}$$
>$\forall \overrightarrow{h}\in B_{\delta}(\overrightarrow{0})$ tale che $\overrightarrow{x}_{0}+\overrightarrow{h}\in A$, che implica che $\overrightarrow{x}_{0}$ è punto di minimo locale di $f$.

>[!tip] Criterio esplicito della matrice Hessiana nel caso $n=2$
>Siano $A\subseteq\mathbb{R}^{2}$ aperto, $f\in c^{2}(A)$ e $(x_{0},y_{0})\in A$ punto critico di $f$. Sia $H_{f}(x_{0},y_{0})$ la matrice Hessiana di $f$ nel punto $(x_{0},y_{0})$. Abbiamo che:
>- Se $\det H_{f}(x_{0},y_{0})>0$ e $\frac{\partial^{2} f}{\partial x^{2}}(x_{0},y_{0})>0$, allora $(x_{0},y_{0})$ è un punto di minimo locale di $f$.
>- Se $\det H_{f}(x_{0},y_{0})>0$ e $\frac{\partial^{2} f}{\partial x^{2}}(x_{0},y_{0})<0$, allora $(x_{0},y_{0})$ è un punto di massimo locale di $f$.
>- Se $\det H_{f}(x_{0},y_{0})<0$, allora $(x_{0},y_{0})$ è punto di sella di $f$.
>- Se $\det H_{f}(x_{0},y_{0})=0$ il criterio non fornisce informazioni, possiamo usare l'indagine diretta o il controllo per convessità/concavità.
>
>Inoltre, se $a:= \frac{\partial^{2} f}{\partial x^{2}}(x_{0},y_{0})=0$, ma $\frac{\partial^{2} f}{\partial y^{2}}(x_{0},y_{0})\neq0$, valgono gli stessi assetti con $c$ al posto $a$.

### Indagine diretta
>[!note]
>Questa strategia consiste nel trovare due curve passanti per il punto critico su cui le restrizioni di $f$ hanno in un caso un massimo e nell'altro un minimo, in maniera tale da concludere che il punto critico è u punto di sella.

### Controllo per convessità/concavità
>[!note]
>Sia $f:\mathbb{R}^{2}\to\mathbb{R}\in c^{2}(\mathbb{R}^{2})$. Diciamo che $f$ è convessa (rispettivamente concava) se $\forall (x,y)\in\mathbb{R}^{2}$ la matrice Hessiana $H_{f}(x,y)$ è definita positiva o semi-definita positiva (rispettivamente definita negativa o semi-definita negativa).
>
>Sia $f\in c^{2}(\mathbb{R}^{2})$ e $(x_{0},y_{0})\in\mathbb{R}^{2}$ un punto critico di $f$, abbiamo che:
>- Se $f$ è convessa su $\mathbb{R}^{2}$, allora $(x_{0},y_{0})$ è un punto di minimo assoluto
>- Se $f$ è concava su $\mathbb{R}^{2}$, allora $(x_{0},y_{0})$ è un punto di massimo assoluto



