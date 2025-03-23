Le derivate parziali si usano per calcolare l'incremento di una funzione in più variabili.

Per calcolarla andiamo a derivare rispetto a una sola variabile, mentre le altre le consideriamo costanti.

Esempio:
$$
\begin{gather}
\frac{\partial f}{\partial x} = \lim_{ h \to 0 } \frac{f(x_0+h,y_0)- f(x_0,y_0)}{h} \\
\frac{\partial f}{\partial y} = \lim_{ k \to 0 } \frac{f(x_0,y_0+k)- f(x_0,y_0)}{k} \\
\end{gather}
$$
Il vettore che ha come coordinate le derivate parziali è detto [[Gradiente|gradiente]]$\nabla$ 
$$
\nabla = (\partial x , \partial y)
$$
nel caso di $f(x,y)$.

Per calcolare le derivate si possono sfruttare anche le proprietà del calcolo della derivata.