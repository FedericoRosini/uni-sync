#uni 
Un corpo rigido è un particolare sistema dinamico in cui le distanze tra i punti rimangono invariate durante il moto.

Per determinare la posizione di un corpo rigido nello spazio sono necessarie sei informazioni, infatti si dice che un corpo rigido ha sei gradi di libertà:
- tre gradi di traslazione $(x, y, z)$
- tre gradi di rotazione $(\phi, \theta, \psi)$

Per studiare il moto di un corpo rigido andiamo a utilizzare un sistema di riferimento non inerziale solidale al corpo, prendiamo questa scelta perché un corpo rigido può sia traslare che ruotare, se scegliessimo un sistema di riferimento inerziale dovremo descrivere sia il moto traslatorio che rotatorio, in questo modo invece possiamo separare i due moti, in quanto il sistema di riferimento non inerziale andrà a considerare unicamente le rotazioni del corpo.

Posta l'attenzione su un generico punto $P$ del corpo, stabilirò che la velocità di $P$ rispetto al sistema di riferimento inerziale sarà data dalle coordinate della velocità del sistema di riferimento non inerziale rispetto a quello inerziale e alla rotazione del sistema di riferimento non inerziale, calcolata da $\omega$ (3 + 3 = 6 parametri), segue la **formula fondamentale dei corpi rigidi**:
$$
\vec v_p(t) = \vec v_{O'}(t) + \vec \omega (t) \times \vec r(t)
$$

## Traslazione di un corpo rigido
![[traslazione corpo rigido.png|300]]
Un corpo rigido esegue un moto traslatorio se tutti i punti hanno stessa velocità e stessa accelerazione:
$$
\vec v_A = \vec v_O + \omega \times (A-O) = \vec v_O
$$
## Rotazione di un Corpo rigido
![[rotazione corpo rigido.png|300]]
Un corpo rigido esegue un moto rotatorio se tutti i punti ruotano attorno a un asse fisso e con raggio pari alla distanza del punto dall'asse:
$$
\vec{P} = \dot \theta R
$$
## Rototraslazione di un corpo rigido
![[rototraslazione corpo rigido.png|500]]
Studiamo il caso del **moto di rotolamento puro** per un disco posto su una superficie orizzontale rettilinea, in cui $\vec v_c = 0$, nel punto di contatto.

Utilizzo la condizione $\vec v_c =0$ per determinare $\vec \omega$, svolgendo tutti i calcoli otterremo che:
$$
\begin{align}
 \vec v_B   &  =   2 |\vec v_O| \hat u_x  \\
\vec v_A   &   = |\vec v_O| \hat u_x + |\vec v_O| \hat u_y
\end{align}
$$
## Seconda cardinale di un corpo rigido
Ricordiamo la seconda cardinale:
$$
\frac{dK_{cr}}{dt} = \sum \vec M_{cr}^{ext}
$$
Se il corpo ruota intorno a un asse fisso allora il momento si può scrivere come:
$$
K = I \omega
$$
La seconda cardinale diventa quindi:
$$
I\alpha = \sum \vec M_{cr}^{ext}
$$
dove $I$ rappresenta il momento d'inerzia rispetto all'asse di riduzione, $\omega$ rappresenta il vettore velocità angolare, mentre $\alpha$ rappresenta il vettore accelerazione angolare.