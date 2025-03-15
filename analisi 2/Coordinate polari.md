[[Calcolo dei limiti]]
- rappresentare la funzione secondo le coordinate polari:
$$
\begin{cases}
x = \rho \cos \theta \\
y = \rho \sin \theta
\end{cases}
$$
ricordando che:
$$
\begin{gather}
\rho = \sqrt{ x^{2} + y^{2} } \\
\tan \theta = \frac{y}{x}
\end{gather}
$$
Se esiste $L \in \mathbb{R}$ e  $\phi(\rho)$ **indipendente da $\theta$** con $\rho \to 0$

Esempio:
$$
\begin{gather}
\lim_{ (x,y) \to (0,0) } \frac{2x^{2}y}{x^{2} + y^{2}} \\
y = mx \quad \frac{2x^{2}(mx)}{x^{2} + m^{2}x^{2}} \to 0 \text{ per $\rho\to 0$}\\
\lim_{ x \to 0 } f(x,mx) = 0 = L \text{ } \forall m\in \mathbb{R}\\
f(\rho \cos\theta, \rho \sin\theta) = \frac{2\rho^{2}\cos ^{2}\theta \rho \sin\theta}{\rho^{2}(\cos ^{2}\theta + \sin ^{2}\theta)}\\
|f(\rho \cos\theta, \rho \sin\theta) - L| = \frac{2\rho^{3}|\cos ^{2}\theta \sin\theta|}{\rho^{2}}\\
|f(\rho \cos\theta, \rho \sin\theta) - L| = 2\rho|\cos ^{2}\theta \sin\theta| \text{ con $\rho \to 0$}\\
|\cos ^{2}\theta \sin\theta|\leq 1\\
2 \rho = 0 \\
2\rho|\cos ^{2}\theta \sin\theta| = 0\\
\end{gather}
$$
ricordando che se $\rho \to 0 \implies (x,y) \to (0,0)$ possiamo dedurre che:
$$
\lim_{ (x,y) \to (0,0) } = 0 
$$
**Se $\phi$ dipende da $\theta$ è dimostrato che il limite non esiste**