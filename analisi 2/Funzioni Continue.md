$f$ è definita **continua** in $x_0 \in A \iff$:
$$
\forall\epsilon > 0, \;\exists \delta >0, \; t.c. \; |f(x) - f(x_0)| < \epsilon, \; \forall x \in A, \; t.c \; ||x - x_0|| < \delta
$$
## Come stabilire se una funzione in più variabili è continua
Per determinare se una funzione è continua dobbiamo per prima cosa calcolarne il dominio, successivamente analizziamo la funzione ricordando che:
se $f(x,y)$ e $g(x,y)$ sono continue allora anche:
- $g \cdot f$ è continua
- $\frac{g}{f}$ è continua
- $g \pm f$ è continua

Esempio:
$$
\begin{gather}
\frac{xy + 1}{x^{2} - y} \\
D = y \neq x^{2} \\
f(x,y) = x \\
g(x,y) = y \\
f \cdot g = xy \text{ continua} \\
f \cdot g + 1 \text{ continua} \\
f \cdot f = x^{2} \text{ continua} \\
f^{2} - g \text{ continua} \\
\end{gather}
$$
essendo tutte le componenti continue, la funzione è continua.

Nel caso in cui ci troviamo davanti una funzione a tratti:
$$
f(x,y =)\begin{cases}
\frac{x^{2} -y^{2}}{x^{2} + y^{2}} \quad  & (x,y) \neq (0,0) \\
0  & (x,y) = (0,0)
\end{cases}
$$
dobbiamo calcolare se la funzione è continua nel punto $(x,y) = (0,0)$. 
Per farlo calcoliamo il limite nel punto e verifichiamo che corrisponda a $f(x,y)$ calcolata per $(x,y) = (0,0)$ 
Quindi in questo caso la funzione sarà continua in $(0,0)$ se il $\lim_{ x,y \to (0,0) } = 0$ 

Dimostro la non esistenza del limite con il metodo della [[Restrizione|restrizione]]:
$$
\begin{gather}
y = mx \\
\frac{x^{2}(1 - m^{2})}{x^{2}(1 + m^{2})} = \frac{(1 - m^{2})}{(1 + m^{2})}
\end{gather}
$$
abbiamo dimostrato che il limite non esiste perché dipende solo da $m$, perciò la funzione sarà continua solo per $(x,y) \neq (0,0)$
