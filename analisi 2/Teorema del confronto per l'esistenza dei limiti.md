[[Calcolo dei limiti]]
Con questo metodo andiamo a confrontare la funzione in analisi con altre note:
$$
0 \leq |f (x,y) | \leq g (x,y) \to 0
$$

Alcune funzioni che prendiamo spesso come riferimento sono:
$$
\begin{gather}
e^z \geq 1 + z \\
\log z \leq z -1  \\
|\sin t| \leq|t| \\
1 - \cos t \leq \frac{t^{2}}{2} \\
\arcsin(t) \leq t \\
\text{con $a,b > 0$ } ab \leq \frac{1}{2}(a^{2} + b^{2}) \\
ab \leq \frac{a^p}{p} + \frac{b^q}{q} \text{  con $p,q > 1$ e $\frac{1}{p} + \frac{1}{q} = 1$}\\
\frac{a ^{2}}{a^{2} + b^{2}} \leq 1
\end{gather}
$$
Esempio:
$$
\begin{gather}
\lim_{ (x,y) \to (0,0) } \frac{xy^{3} - 2\sin(x^{2}y)\cos(x + 2y)}{x^{2} + y^{2}} = L? \\
L = \lim_{ (x,y) \to (0,0) } \frac{xy^{3}}{x^{2} + y^{2}}  - \lim_{ (x,y) \to (0,0) } \frac{2\sin(x^{2}y)\cos(x + sy)}{x^{2} + y^{2}}
\end{gather}
$$
consideriamo:
$$
\begin{gather}
\lim_{ (x,y) \to (0,0) } \frac{xy^{3}}{x^{2} + y^{2}} = L_1 \\
\lim_{ (x,y) \to (0,0) } \frac{2\sin(x^{2}y)\cos(x + sy)}{x^{2} + y^{2}} = L_2
\end{gather}
$$
purché $L_1, L_2$ esistano e non diano luogo a forme indeterminate.

Studiamo $L_1$:
$$
\begin{gather}
0 \leq \left|\frac{xy^{3}}{x^{2} + y^{2}}\right| = \left|\frac{yxy^{2}}{x^{2} + y^{2}}\right|\\
\leq y^{2} \frac{ |x| |y|}{x^{2} + y^{2}} \leq y^{2} \frac{\frac{1}{2}(x^{2} + y^{2})}{x^{2} + y^{2}}
\end{gather}
$$
In questo passaggio abbiamo usato  la disuguaglianza nota citata all'inizio: $ab \leq \frac{1}{2}(a^{2} + b^{2})$
La funzione diventa ora:
$$
\begin{gather}
2y^{2} = g(x,y) \to 0 \\
L_1 = 0
\end{gather}
$$
Studiamo $L_2$
$$
\begin{gather}
\lim_{ (x,y) \to (0,0) } \frac{2\sin(x^{2}y)\cos(x + 2y)}{x^{2} + y^{2}} \\
|\cos(x + 2y)| \leq 1 \implies f_2(x,y) \leq \frac{2|\sin(x^{2}y)|}{x^{2} + y^{2}} \\
|\sin(t)| \leq |t| \implies f_2(x,y) \leq \frac{2 x^{2}|y|}{x^{2} + y^{2}} \\
= 2 |x|\frac{|x||y|}{x^{2} + y^{2}} \leq s|x| \frac{1}{2} \frac{x^{2} + y^{2}}{x^{2} + y^{2}} = |x| = 0 \\
L_2 = 0
\end{gather}
$$
Siamo arrivati quindi al risultato che:
$$
\begin{gather}
L_1 = 0 \\
L_2 = 0 \\
L = L_1 + L_2 = 0 + 0 = 0
\end{gather}
$$
