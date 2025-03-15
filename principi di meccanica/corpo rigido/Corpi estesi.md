#uni 
Un corpo esteso è un sistema continuo, ovvero un insieme di punti materiali distribuiti nello spazio.

La massa di un corpo esteso viene calcolata tramite la **densità volumetrica**, la **densità superficiale**, o la **densità lineare** rispettivamente:
$$
\begin{gather}
\rho_v(\vec r) = \frac{\Delta m}{\Delta v}\\

\rho_s(\vec r) = \frac{\Delta m}{\Delta s}\\

\rho_L(\vec r) = \frac{\Delta m}{\Delta L}

\end{gather}
$$
La massa totale ($M$) del corpo esteso è uguale alla somma di tutte le masse dei punti materiali($m_i$):
$$
\begin{gather}
M=\sum \Delta m_i = \int dm = \int \rho_v (\vec r) dv\\

\text{Se} \quad \rho_v(\vec r) = cost \implies M=\rho_vV\\

\rho_v = \frac{M}{V}

\end{gather}
$$
Un altro concetto molto importante da introdurre è il \textbf{centro di massa} che rappresenta il punto in cui possiamo concentrare tutte le forze così da studiare il comportamento di un corpo esteso come se fosse un punto materiale:
$$\vec{r}_{cm} = \frac{\sum_i \vec r_i}{N}$$
dove $N$ rappresenta il numero di punti materiali.

Tuttavia se le masse sono costanti si può usare la seguente formula:
$$\vec r_{cm} = \frac{1}{M}\int \vec r dm$$
Studiamo un caso specifico, prendiamo in esempio un asta omogenea:
![[asta omogenea.png|300]]
Essendo l'asta un corpo omogeneo, possiamo scrivere il centro di massa come:
$$\vec r_{cm} = \frac{\int vec r dm}{M}$$
Ricordiamo l'equazione della densità lineare, $\rho_L = \frac{M}{L}$, con alcuni accorgimenti matematici possiamo ottenere:
$$
\begin{gather}
\rho_L = \frac{dm}{dL} = \frac{dm}{dx}\\

dm = \rho_L dx

\end{gather}
$$
Sostituendo questo accorgimento nell'equazione precedente otterremo che:
$$
\begin{gather}
\vec r_{cm} = \frac{\int_0^L x \hat u_x \rho_L dx}{M} \footnotemark\\

\vec r_{cm} = \frac{\rho_L}{M}\frac{x^2}{2}\hat u_x\Big|_0^L\\

\vec r_{cm} = \frac{\rho_L}{M}\frac{L^2}{2}\hat u_x\\

\rho_L = \frac{M}{L} \implies \vec r_{cm} = \frac{M}{L \cdot M}\frac{L^2}{2}\hat u_x\\

\vec r_{cm} = \frac{L}{2} \hat u_x

\end{gather}
$$
Abbiamo quindi dimostrato matematicamente che il centro di massa di un asta omogenea si trova a metà della sua lunghezza.

## Prima cardinale corpi estesi
La variazione di quantità di moto di un sistema e proporzionale alla risultante delle forze esterne a cui è sottoposto:
$$m\vec a_{cm} = \sum_i \vec F_i = \vec F_{ext}$$
Questo risultato nasce dal terzo principio della dinamica \ref{terzo principio della dinamica}, grazie al quale possiamo stabilire che le forze interne al corpo si annullano poiché l'azione che un punto materiale esegue su un altro punto materiale porterà a una reazione uguale e contraria di quest'ultimo annullandosi.

Adesso grazie alla prima cardinale dimostriamo che \textbf{la posizione del centro di massa di un corpo costituito da due o più corpi estesi è uguale alla media delle posizioni dei centri di massa dei corpi, pesata dilla massa di questi.}

Per dimostrare questa affermazione, analizziamo un caso specifico:

Prendiamo un disco di raggio $R$ e di massa $M$, e saldiamo a una estremità una punto materiale di massa $m$.
![[esercizio prima cardinale.png|300]]
Ricordiamo che:
$$
\begin{gather}
\vec r_{cm} = \frac{\sum_i m_i \vec r_i}{M_{tot}}\\

\vec r_{cm} = \frac{\sum_i m_i \vec r_i + mR \hat u_x}{M_{tot} + m}\\

\vec r_{cm} = \frac{M \vec r_{cm}^{disco} + mR \hat u_x}{M_{tot} + m}\\

\end{gather}
$$
Abbiamo quindi dimostrato l'affermazione precedente.

Analizziamo adesso un altro esempio: consideriamo un auto con un pendolo appeso al tettuccio dell'auto con una massa posta su un estremità.

La macchina accelera con $a>0$
![[esercizio macchina prima cardinale.png|500]]
Lo scopo dell'esercizio è quello di ricavare l'equazione del moto del pendolo.
Analizziamo le forze in gioco:
$$
\begin{gather}
\vec F_p = mgcos(\theta)\hat n - mg sin(\theta)\hat \tau\\

\vec F_T = m|\vec{a_{auto}}|(sin(\theta)\hat n - cos(\theta)\hat \tau)\\

\vec{T} = T \hat n

\end{gather}
$$
studio le forze lungo $\hat \tau$:
$$-mgsin(\theta) - m|\vec a_{auto}|cos(\theta) = m\ddot s = mR\ddot{\theta}$$
Per trovare la posizione di equilibrio pongo $\ddot{\theta} = 0$:
$$
\begin{gather}
-gsin(\theta_{eq})-|\vec a_{auto}|cos(\theta_{eq})=0\\

tg(\theta_{eq}) = - \frac{|\vec a_{auto|}}{g}

\end{gather}
$$
Ricordiamo ora la prima cardinale
$$\sum \vec F_{ext} = M\vec a = \frac{d\vec Q}{dt}$$
Segue che se il sistema è \textbf{isolato} $\frac{d\vec Q}{dt} = 0$ perciò $\vec Q = cost$.

Dobbiamo stare attenti però perché la quantità di moto non ci fornisce informazioni sulla rotazione del corpo, per questa informazione dobbiamo calcolare il \textbf{momento angolare di un corpo esteso}:
$$K_O = \sum_i |P_i-O|\times\vec Q$$
## Seconda cardinale dei corpi estesi
L'enunciato della seconda cardinale dei corpi estesi è il seguente:

**La derivata del momento angolare di un sistema rispetto al tempo, è uguale alla risultante dei momenti esterni rispetto a un punto fisso $C_r$.**
$$\frac{dK_Cr}{dt} = M_{ext}$$
questo vuol dire che se il braccio e/o la forza aumentano, anche il momento esterno aumenta.

Se il sistema è isolato:
$$M_{ext}=0 \implies \frac{dK_Cr}{dt} = 0 \implies K = cost$$
Segue che il momento della forza peso sarà:
$$K = (P_{cm} - C_r) \times (-M_{tot}g \hat u_y)$$
