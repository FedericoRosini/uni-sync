Le derivate direzionali descrivono la velocità di crescita lungo un asse.

**Definizione:**
Sia $v$ il versore della direzione della quale vogliamo conoscere la crescita; si dice **derivata direzionale di $f$ rispetto a $v$ nel punto $x_0$**:
$$
D_vf(x_0) = \frac{\partial f(x_0)}{\partial v} = \lim_{ t \to 0 } \frac{f(x_0 + tv) - f(x_0)}{t}
$$
purché esista finito.

Se studiamo il caso di due dimensioni ($n=2$), avremo che $v = (\cos\theta, \sin\theta)$:
$$
D_vf(x_0,y_0) = \lim_{ t \to 0 } \frac{f(x_0 + t\cos\theta, y_0 + t\sin\theta) - f(x_0,y_0)}{t}
$$
possiamo quindi arrivare al risultato che:
$$
g(t) = f(x_0 + t\cos\theta, y_0 + t\sin\theta)
$$
perciò
$$
D_vf(x_0, y_0) = g'(0)
$$

**Esempio:**
$f(x,y) = \sqrt[3]{ x^{2}y }$, $D_vf(0,0)$  con $v = (\cos\theta, \sin\theta)$
$$
\begin{gather}
g(t) = f(t\cos\theta, t\sin\theta) = \sqrt[3]{ t^{2}\cos ^{2}\theta t\sin\theta } = t (\cos\theta)^{\frac{2}{3}} (\sin\theta)^{\frac{1}{3}} \\
g'(t) = (\cos\theta)^{\frac{2}{3}} (\sin\theta)^{\frac{1}{3}}
\end{gather}
$$
**COMPLETARE**


