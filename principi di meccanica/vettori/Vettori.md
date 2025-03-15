#uni 
Un vettore è un'entità matematica dotata di:
- direzione
- verso
- modulo

Si indica con $\vec{u}$ il vettore e con $u$, $|u|$ il suo modulo.
![[Vettore.png]]
Si definisce **versore** un vettore che ha stessa direzione e verso del vettore, ma $\vec{|u|}=1$:
$$
\hat{u}=\frac{\vec{u}}{|u|}
$$Alcuni esempi di grandezze vettoriali sono:
$$
\begin{array}{c|c|c}
Vettoriali & Scalari \\
\hline
Spostamento & Lunghezza \\
Velocità & massa \\
Accelerazione & Intervallo di tempo \\
Forza & Lavoro \\
Quantità di moto & Energia\\
Momento di forze & \\
Momento angolare & \\
Impulso\\
\end{array}
$$

Con **angolo** tra due vettori si intende l'angolo convesso generato dalle direzioni su cui giacciono i vettori.

  

Il **modulo della proiezione** di un vettore $\vec{v}$ sulla direzione del vettore $\vec{u}$ si calcola:

$$v_u=v\cdot cos(\alpha)$$
dove $\alpha$ è l'angolo compreso tra $u$ e $v$.

## Operazioni tra vettori

### Prodotto Scalare

Il **prodotto scalare** è un'operazione tra due vettori $v$ e $w$ che dà come risultato uno scalare:
$$\vec{v}\cdot\vec{w}=|v||w|cos(\alpha)$$
dove $\alpha$ è l'angolo compreso tra $\vec{v}$ e $\vec{w}$.

Si nota che se:
-  $\alpha$=0, $\vec{v}\cdot\vec{w}=|v||w|$;
- $\alpha=\frac{\pi}{2}$, $\vec{v}\cdot\vec{w}=0$.

Viene identificata come **norma** di un vettore $u$, il suo modulo, e viene calcolato attraverso il prodotto scalare: $|u|=\sqrt{\vec{u}\cdot \vec{u}}$.

Mentre la norma della somma di due vettori si calcola:
$$|\vec{u}+\vec{v}|=\sqrt{(\vec{u}+\vec{u}) \cdot (\vec{u}+\vec{u})}$$
### Prodotto Vettoriale

Il **prodotto vettoriale** è un'operazione vettoriale che, partendo da due vettori $\vec{v}$ w $\vec{w}$ restituisce un vettore $\vec{u}$ con le seguenti proprietà:
- $\vec{u}$ ortogonale sia a $\vec{v}$ che a $\vec{w}$;
- il verso di $\vec{u}$ viene determinato dalla regola della mano destra;
- $|\vec{u}|=|v||w|sin(\alpha)$

Si nota da quest'ultima proprietà che se $\vec{v} \times \vec{w}=0 \implies \vec{v} \parallel \vec{w}$.
### Prodotto misto
Il **prodotto misto** è un' operazione vettoriale che partendo da tre vettori ci restituisce uno scalare:
$$(\vec{v} \times \vec{w}) \cdot \vec{u} =k$$
Dando come risultato uno scalare, dovremo prima eseguire il prodotto vettoriale e in seguito il prodotto scalare.