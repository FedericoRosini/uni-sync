#uni 
Prima d'introdurre il concetto di lavoro è importante introdurre il concetto di spostamento.

Lo  **spostamento** è una grandezza vettoriale che misura la variazione della posizione di un punto materiale $P$ nello spazio, per esempio, se $P$ si muove da $A$ a $B$, lo spostamento sarà:

$$\vec{s}=(B-A)$$
Adesso possiamo introdurre il concetto di \textbf{lavoro}:
$$\Delta L = \vec{F} \cdot \vec{s}$$
Notare che il lavoro è una grandezza scalare, infatti viene calcolato tramite il prodotto scalare.

La potenza invece misura quanto lavoro è stato effettuato in un unità di tempo:
$$W=\frac{\Delta L}{\Delta t} = \vec{F} \cdot \vec{v}$$
## Teorema delle Forze vive
Il teorema delle forze vive ci garantisce che il lavoro è uguale alla variazione di energia presente nel sistema, adesso vedremo la dimostrazione:
![[teorema delle forze vive.png|300]]
La curva rappresentata in figura è lo spostamento totale eseguito dal corpo, per la nostra dimostrazione dobbiamo scomporre la curva dello spostamento totali in tanti piccoli spostamenti che chiameremo $\Delta \vec{s}_i$ ogni piccolo spostamento subirà una determinata forza $F_i$, il lavoro totale eseguito dal corpo sarà dato dalla somma di tutti i lavori compiuti nei piccoli spostamenti:
$$L_{tot}=\sum_i \vec{F}_i \cdot \vec{s}_i$$
Ricordando la teoria di analisi possiamo osservare che questo calcolo ci porterà a trovare l'area sottostante alla nostra curva, pertanto:
$$L_{tot}=\int_A^B{\vec{F}d\vec{s}}$$
adesso moltiplichiamo l'integrale per $\frac{dt}{dt}$ e in seguito eseguiamo degli accorgimenti matematici:
$$
\begin{gather}
L_{tot}=\int_A^B{\vec{F}\frac{d\vec{s}}{dt}dt}\\

\frac{d\vec{s}}{dt}=\vec{v} \implies L_{tot}=\int_A^B{\vec{F}\vec{v}}dt\\

\vec{F}=m\vec{a} \implies L_{tot}=\int_A^B{(m\vec{a})\vec{v}}dt\\

\vec{a}=\frac{d\vec{v}}{dt} \implies L_{tot}=\int_A^B{m\frac{d\vec{v}}{dt}\vec{v}}dt\\

\end{gather}
$$

Adesso dobbiamo fare un'altra considerazione:
$$
\begin{gather}
\frac{d(v \cdot v)}{dt} = \frac{dv}{dt} \vec{v}+ \vec{v} \frac{dv}{dt}\\

\frac{d(v \cdot v)}{dt} = 2\frac{dv}{dt} \vec{v}\\

\end{gather}
$$
Tornando all'integrale precedente:
$$
\begin{gather}
  L_{tot} = \frac{1}{2}m \int_A^B{\frac{d(v \cdot v)}{dt}dt}\\

L_{tot} = \frac{1}{2}m \int_A^B{\frac dv \cdot v}\\

L_{tot} = \frac{1}{2}m (v)^2 \big|_A^B\\

L_{tot} = \frac{1}{2}m (v_A)^2 - \frac{1}{2}m (v_B)^2

\end{gather}
$$
Denominiamo:
$$T=\frac{1}{2}m (v)^2$$
con $T$ che rappresenta l'\textbf{energia cinetica}. Vediamo ora un esempio pratico in cui questo teorema semplifica i calcoli:

Prendiamo in esempio un corpo di massa $m$ in caduta libera, partendo da una determinata altezza $h$ vogliamo sapere la velocità $v_f$ con cui tocca il suolo.
![[esercizio teorema delle forze vive.png|300]]
Osservando i dati dell'esercizio avremo:
$$
\begin{gather}
\vec{Fp}=-mg\hat{u}_y\\

\Delta\vec{s}=-l\hat{u}_y

\end{gather}
$$
Abbiamo perciò tutti i dati per calcolare il lavoro $L$ che è stato compiuto dal corpo nella sua discesa libera:
$$
\begin{gather}
L_{AB}= \vec{F} \cdot \Delta\vec{s}\\

L_{AB}= mgl

\end{gather}
$$
Sappiamo grazie al teorema delle forze vive che $L_{AB}=T_B-T_A$ perciò:
$$L_{AB} = \frac{1}{2}mv_B^2 - \frac{1}{2}mv_A^2$$
essendo $V_A=0$ perché il corpo parte da fermo:
$$
\begin{gather}
L_{AB} = \frac{1}{2}mv_B^2\\

mgl = \frac{1}{2}mv_B^2\\

|v_B|=\sqrt{2gl}

\end{gather}
$$
**N.B. Quando un esercizio non richiede, e non è indicato, il tempo in cui un punto materiale raggiunge una determinata configurazione, ci conviene sempre usare il teorema delle forze vive.**
