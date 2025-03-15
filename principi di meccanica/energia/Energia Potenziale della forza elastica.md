#uni 
Come detto in precedenza anche la forza elastica è una forza conservativa, e pertanto anch'essa genererà un'energia potenziale, per determinarne l'equazione andiamo a studiare un caso specifico:
![[energia potenziale forza elastica.png|300]]
Abbiamo imparato in precedenza che:
$$
\begin{gather}

\vec{F}_{el} = -kx \hat{u_x}\\

d\vec{s} = dx\hat{u}_x

\end{gather}
$$
Possiamo quindi dire che:
$$
\begin{gather}
L_{AB} = \int_A^B{-kxdx}\\

L_{AB} = -k \int_A^B{xdx}\\

L_{AB} = -\frac{kx^2}{2}\Big|_A^B\\

L_{AB} = -\frac{kx_B^2}{2}+ \frac{kx_A^2}{2}\\

\end{gather}
$$
Definiamo l'energia potenziale elastica come:
$$U=-\frac{kx^2}{2}$$

Possiamo ora aggiungere un osservazione alla definizione delle forze conservative \label{definizione forze conservative}:

$\vec{F}$ è una forza conservativa $\iff \exists$ una funzione $U(\vec{r})$ t.c. $\vec{F}=-\nabla U(\vec{r})$, dove $\nabla$ rappresenta il **gradiente**, il gradiente per definizione "mangia" uno scalare e restituisce un vettore:

$$\nabla U(\vec{r})=\Big( \frac{\partial U}{\partial x}, \frac{\partial U}{\partial y}, \frac{\partial U}{\partial z} \Big)$$

Dove $\partial$ rappresenta una derivata parziale, in pratica si derivano solamente le variabili che stiamo considerando, mentre le altre vengono considerate costanti, per esempio:
$$
\begin{gather}
\vec{F}_p =- \Big( \frac{\partial mgy}{\partial x}, \frac{\partial mgy}{\partial y}, \frac{\partial mgy}{\partial z} \Big)\\

\vec{F}_p=- \Big(0, \frac{\partial mgy}{\partial y}, 0 \Big)\\

\vec{F}_p = (0, mg, 0)

\end{gather}
$$
Questo è un breve resoconto di quanto detto fino a ora:
$$
\begin{array}{c|c}
Forze conservative & Energia Potenziale \\\hline

Forza peso & $mgy$\\

Forza elastica & $-\frac{kx^2}{2}$
\end{array}
$$
