>[!note]
>Consideriamo un equazione differenziale della forma: $$ay''+b'+cy=f(t)$$
>Con $a\neq0$. Per determinare l'integrale generale dell'equazione è necessario conoscere l'integrale generale dell'omogenea associata e la soluzione particolare: $$y(t)=C_{1}y_{1}(t)+C_{2}y_{2}(t)+y_{P}(t)\qquad C_{1},C_{2}\in\mathbb{R}$$

Per trovare la soluzione particolare si usa il metodo di somiglianza, di cui adesso analizziamo i casi:
### Forzante esponenziale
>[!note]
>Consideriamo il caso: $$f(t)=Ae^{\alpha t}\qquad A,\alpha\in\mathbb{R}$$
>Per trovare una soluzione particolare, si parte da una funzione: $$y_{P}(t)=Ce^{\alpha t}$$
>Derivandola e sostituendo nell'equazione troveremo un valore $C$. Nel caso $\alpha$ sia radice del polinomio caratteristico, usiamo come soluzione particolare: $$y_{P}(t)=Cte^{\alpha t}$$
>Se $\alpha$ è radice doppia del polinomio caratteristico, usiamo come soluzione particolare: $$y_{P}(t)=Ct^{2}e^{\alpha t}$$
>

### Forzante polinomiale
>[!note]
>Consideriamo il caso in cui $f(t)$ sia polinomiale di grado $n$. Utilizziamo come soluzione particolare il più generale polinomio di grado $n$: $$y_{P}(t)=\beta_{n}t^{n}+\beta_{n-1}t^{n-1}+\cdots+\beta_{1}t+\beta_{0}$$
>Derivando, sostituendo e applicando il principio di identità dei polinomi ricaviamo le costanti $\beta_{n},\beta_{n-1},\cdots,\beta_{1},\beta_{0}$ dal sistema lineare di $n+1$ equazioni e $n+1$ incognite. In caso non sia possibile applicare il principio di identità dei polinomi proviamo usare come soluzione il polinomio generale di grado $n+1$.

### Forzante trigonometrica
>[!note]
>Consideriamo il caso in cui $f(t)$ sia trigonometrica. Utilizziamo come soluzione particolare: $$y_{P}(t)=C_{1}\cos(\nu t)+C_{2}\sin(\nu t)$$
>Derivando, sostituendo e applicando il principio di identità dei polinomi ricaviamo $C_{1}$ e $C_{2}$. Se la forzante è soluzione dell'omogenea associata usiamo come soluzione particolare: $$y_{P}=t(C_{1}\cos(\nu t)+C_{2}\sin(\nu t))$$

