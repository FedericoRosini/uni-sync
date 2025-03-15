Per quanto riguarda lo studio della statica prendiamo in esame il caso della \textbf{leva}:
![[leva.png|500]]
Prendiamo un asta con lunghezza $L$, massa $M$ e densità omogenea, dati $m_1$ e $m_2$ determinare la posizione di un fulcro opportuno affinché il sistema sia in equilibrio.

Ricordiamo che un sistema è in equilibrio quando:
$$
\begin{gather}
\sum \vec F_{ext} = 0\\

\sum \vec M_{cr\,ext} = 0

\end{gather}
$$
Come sistema considero l'asta e le masse, non considero il fulcro.

Rappresentiamo ora uno schema delle forze:
![[schema forze es leva.png|500]]
La forze in gioco saranno quindi:
$$
\begin{gather}
\vec N = N \hat u_y\\

\vec F_{p1} = m_1 g \hat u_y\\

\vec F_{p2} = m_2 g \hat u_y\\

\vec F_M = -Mg \hat u_y


\end{gather}
$$

Scriviamo ora le cardinali:
$$
\begin{gather}
\text{Prima Cardinale:} \quad N - m_1g - m_2g -Mg = 0\\

\text{Prima Cardinale:} \quad -m_2 g L - M g \frac{L}{2} + Nx = 0

\end{gather}
$$
Isolando la $x$ otterremo che:
$$x = \frac{L(m_2 + \frac{M}{2})}{m_1 + m_2 + M}$$

