>[!note]
>Una EDO del primo ordine è autonoma se è nella forma: $$y'(x)=g(y(x))$$
>Dove $g: B\to\mathbb{R}$ è una funzione continua nell'insieme $B\subseteq\mathbb{R}$ (cioè la EDO è in forma normale e a variabili separabili).

>[!tip]
>Se $y$ è soluzione di $y'(x)=g(y(x))$ in un certo intervallo $(\lambda,\beta)$, allora anche $$z_{c}:=y(x+c)$$
>È soluzione in $(\lambda-c,\beta+c)\quad\forall c\in\mathbb{R}$.

>[!tip]
>Se $g$ è positiva (rispettivamente negativa) in un certo punto $\overline{y}\in B$, allora una soluzione $y:J\to B$ è passante per $\overline{y}$, cioè tale che $\exists \overrightarrow{x}$ con $y(\overrightarrow{x})=\overrightarrow{y}$, sarà crescente (rispettivamente decrescente) in $\overrightarrow{x}$.

### Punti di equilibrio
>[!note]
>Sia: $$y'(x)=g(y(x))$$
Gli zeri della funzione $g$ si dicono punti di equilibrio.

### Costruzione del diagramma di fase
>[!note]
>Partiamo dal grafico di $g$:
>![[Pasted image 20241216173848.png]]
>E disegniamo il diagramma in questo modo:
>- Disegno una linea
>- Indichiamo i punti di equilibrio
>- Indichiamo con una freccia gli intervalli dove $g$ è positiva o negativa, rispettivamente.
>
>![[Pasted image 20241216174026.png]]
>
>Infine diciamo che un punto di equilibrio $\overline{y}$ è:
>- stabile se entrambe le frecce puntano a $\overline{y}$
>- instabile in caso contrario

### Esempio di studio qualitativo di un EDO autonoma
>[!note]
>1. Verifichiamo che esiste unicamente e localmente soluzione per tutti i problemi di Cauchy associati alla EDO.
>2. Troviamo i punti di equilibrio.
>3. Verifichiamo la prolungabilità delle soluzioni
>4. Disegniamo il diagramma di fase e deduciamo la monotonia delle soluzioni e la stabilità dei punti di equilibrio.
>5. Studio del limite delle soluzioni agli estremi di definizione
>6. Studio convessità/concavità soluzioni
