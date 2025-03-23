Una funzione si dice differenziabile se vale:
$$
f(x_0 +  h, y_0 + k) - f(x_0,y_0) = f_x(x_0,y_0)h + f_y(x_0,y_0)k + o(\sqrt{ h^{2} + k^{2} })
$$
dove
- $f_x(x_0,y_0)h + f_y(x_0,y_0)k$ è l'incremento lungo il piano tangente;
- $o(\sqrt{ h^{2} + k^{2} })$ è l'errore di ordine superiore a $||(h,k)||$

Più in generale:
$f$ è differenziabile in $x_0$ se esiste $a \in \mathbb{R}^n$ tale che:
$$
f(x_0 +h) - f(x_0) = a\cdot h +o(||h||)
$$
Se $f$ è differenziabile, questo implica che $f$ è:
- [[Funzione derivabile|derivabile]] e $a = \nabla f(x_0)$
- [[Funzioni Continue|continua]]

Se una funzione $f$ è differenziabile, si dice **differenziale** di $f$ in $(x_0, y_0)$.

La composizione di due funzioni composte differenziabili è ancora differenziabile
