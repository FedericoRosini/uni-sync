#uni 
La coordinata intrinseca è una coordinata che misura lo spazio percorso lungo la traiettoria in funzione del tempo, risulta comodo utilizzarla negli esercizi quando la traiettoria è nota e non rettilinea.
Per implementarla è necessario:
1. Scegliere l'origine sulla traiettoria
2. Scegliere un verso positivo
3. Indico con $s$ la distanza, con segno, che devo percorrere dall'origine fino al punto, lungo la traiettoria
![[coordinata intrinseca.png|500]]
## Moto circolare
Il moto circolare uniforme è costituito da una traiettoria circolare:
![[moto circolare.png|500]]

La posizione del punto è definita dalla legge oraria:
$$\vec{r}(t) = x(t)\hat{u}_x + y(t)\hat{u}_y$$
Indichiamo con $O'$ l'origine della coordinata intrinseca, con senso antiorario positivo.

Adesso scriviamo $\vec{r}(t)$ in funzione dell'angolo $\theta$:
$$\vec{r}(t)= Rcos(\theta (t))\hat{u}_x + Rsin(\theta (t))\hat{u}_y$$
L'angolo $\theta$ può essere scritto, grazie alla definizione di radiante come:
$$\theta = \frac{arco}{raggio} = \frac{s(t)}{R}$$
Perciò avremo che:
$$\vec{r}(t)= Rcos(\frac{s(t)}{R})\hat{u}_x + Rsin(\frac{s(t)}{R})\hat{u}_y$$
Analizzando derivando questa legge oraria otterremo la legge oraria della velocità del punto materiale:

$$
\begin{gather}
\vec{v}(t) = \dot{s}(t)\Big(-sin \Big(\frac{s(t)}{R}\Big)\hat{u}_x + cos \Big(\frac{s(t)}{R}\Big)\hat{u}_y \Big)\\
\Big(-sin \Big(\frac{s(t)}{R}\Big)\hat{u}_x + cos \Big(\frac{s(t)}{R}\Big)\hat{u}_y \Big) = \hat{\tau}\\
\vec{v}(t) = \dot{s}(t)\hat{\tau}
\end{gather}
$$**Dimostrazione**: per dimostrare che $\hat{\tau}$ sia un versore tangente alla traiettoria dobbiamo verificare che:
4.  il modulo sai $1$, $|\hat{\tau}| = 1$
5. che sia tangente alla traiettoria, $\vec{r}(t) \cdot \hat{\tau} = 0$

Il punto 1. si dimostra poiché:
$$|\hat{\tau}| = sin^2(k) + cos^2(k) = 1$$
Per il punto 2. dobbiamo eseguire il prodotto scalare:
$$
\begin{gather}
\vec{r}(t) \cdot \hat{\tau} = \Big(Rcos \Big(\frac{s(t)}{R} \Big) \hat{u}_x + Rsin \Big(\frac{s(t)}{R} \Big) \hat{u}_y \Big) \cdot \Big(-sin \Big(\frac{s(t)}{R}\Big) \hat{u}_x + cos \Big(\frac{s(t)}{R}\Big) \hat{u}_y \Big)\\

-Rcos\Big(\frac{s(t)}{R} \Big)sin \Big(\frac{s(t)}{R} \Big) + R sin \Big(\frac{s(t)}{R} \Big) cos \Big(\frac{s(t)}{R} \Big) = 0
\end{gather}
$$
Derivando nuovamente otterremo la legge oraria dell'accelerazione:
$$
\begin{gather}
\ddot{s}(t)\hat{\tau} \dot{s}(t) \Big(-sin \Big(\frac{s(t)}{R} \Big)\hat{u}_x - cos \Big(\frac{s(t)}{R} \Big) \hat{u}\Big)\\

\Big(-sin \Big(\frac{s(t)}{R} \Big)\hat{u}_x - cos \Big(\frac{s(t)}{R} \Big) \hat{u}\Big) = \hat{n} \text{versone perpendicolare alla traiettoria}\\

\vec{a}(t) = \ddot{s}(t)\hat{\tau} + \frac{dot{s}^2(t)}{R}\hat{n}\

\end{gather}
$$

Dove $\ddot{s}(t)\hat{\tau}$ rappresenta l'**accelerazione tangenziale**, e si occupa di variare il modulo della velocità, mentre $\frac{\dot{s}^2(t)}{R}\hat{n}$ rappresenta l'\textbf{accelerazione centripeta}, e si occupa di variare la direzione della velocità.