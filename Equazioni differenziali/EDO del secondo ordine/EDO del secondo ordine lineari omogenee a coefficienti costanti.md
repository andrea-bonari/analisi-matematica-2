Per determinare l'integrale generale dell'equazione omogenea è sufficiente trovare due soluzioni linearmente indipendenti.

Ricordandoci che una funzione della forma $y(t)=e^{\lambda t}$ ha derivata proporzionale alla funzione stessa:
$$\begin{align*}
&y(t)=e^{\lambda t}\\
&y'(t)=\lambda e^{\lambda t}\\
&y''(t)=\lambda^{2} e^{\lambda t} 
\end{align*}$$
Sostituendo all'equazione avremo: $$\begin{align*}
&a\lambda^{2}e^{\lambda t}+b\lambda e^{\lambda t}+e^{\lambda t}=0\\
\Longrightarrow& e^{\lambda t}(a\lambda^{2}+b\lambda+c)=0\\
\end{align*}$$
Sapendo che $e^{\lambda t}\neq0$ per qualsiasi valore otterremo: $$a\lambda^{2}+b\lambda+c=0$$
Questa è detta equazione caratteristica. Le soluzioni dell'equazione $\lambda_{1}$ e $\lambda_{2}$ ci daranno quindi le soluzioni dell'omogenea linearmente indipendenti: $$y_{1}(t)=e^{\lambda_{1}t}\qquad y_{2}(t)=e^{\lambda_{2}t}$$
Siccome la natura delle soluzioni dell'equazione caratteristica è determinata dal $\Delta$ dell'equazione caratteristica si creano diversi casi. 

### Caso $\Delta>0$
>[!note]
>Si creano due soluzioni reali e distinte, e siccome sono indipendenti, per il teorema di struttura avremo come integrale generale: $$y(t)=C_{1}e^{\lambda_{1} t}+C_{2}e^{\lambda_{2}t}$$

### Caso $\Delta <0$
>[!note]
>Si creano due soluzioni complesse coniugate. Ricordando la formula di Eulero: $$e^{\alpha +i\beta}=e^{\alpha}(\cos (\beta)+i\sin(\beta))$$
>Costruiamo due soluzioni reali linearmente indipendenti: $$\begin{align*}
u_{1}(t)&= \frac{y_{1}(t)+y_{2}(t)}{2}=e^{\alpha t}\cos(\beta t)\\
u_{2}(t)&= \frac{y_{1}(t)-y_{2}(t)}{2i}=e^{\alpha t}\sin(\beta t)
\end{align*}$$
>Quindi l'integrale generale sarà: $$y(t)=C_{1}e^{\alpha t}\cos(\beta t)+C_{2}e^{\alpha t}\sin(\beta t)=e^{\alpha t}(C_{1}\cos(\beta t)+C_{2}\sin(\beta t))$$

### Caso $\Delta=0$
>[!note]
>Si creano due soluzioni reali coincidenti. Si può dire che le due soluzioni reali linearmente indipendenti saranno $$\begin{align*}
y_{1}(t)=e^{\lambda_{1}t}\\
y_{2}(t)=te^{\lambda_{1}t}
\end{align*}$$
Quindi l'integrale generale sarà: $$y(t)=C_{1}e^{\lambda_{1}t}+C_{2}te^{\lambda_{1}t}$$
