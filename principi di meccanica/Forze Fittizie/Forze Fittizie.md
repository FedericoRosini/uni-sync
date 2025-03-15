#uni 
Le forze fittizie sono forze osservabili in sistemi di riferimento non inerziali e che non sono dovute dall'interazione con altri corpi. Per comprenderle al meglio analizziamo un caso specifico:
![[forze fittizie.png|300]]
In questo caso possiamo notare due sistemi di riferimento $(\hat u_x, \hat u_y, \hat u_z)$ e $(\hat u_x', \hat u_y', \hat u_z')$.

Le leggi orarie di questi due sistema di riferimento saranno rispettivamente:
$$
\begin{gather}
\vec r (t) = x(t)\hat u_x + y(t)\hat u_y + z(t)\hat uz \\

\vec {r'} (t) = x'(t)\hat u_x' + y'(t)\hat u_y' + z'(t)\hat u_z'

\end{gather}
$$
Se il sistema di riferimento $O'_{\hat{u}x', \hat{u}y', \hat{u}z'}$ compie un moto puramente traslatorio rispetto al sistema di riferimento $O_{\hat{u}x, \hat{u}y, \hat{u}z}$, i versori $\hat u_x', \hat u_y', \hat u_z'$ non varieranno; ma se il sistema di riferimento $O'_{\hat{u}x', \hat{u}y', \hat{u}z'}$ compie un moto di rotazione, allora questi cambieranno rispetto al sistema di riferimento principale $O_{\hat{u}x, \hat{u}y, \hat{u}z}$.

Per studiare la relazione tra questi sistemi di riferimento vado a studiare il vettore $\vec r_{O'}(t)$ che determina la posizione in funzione del tempo del sistema di riferimento $O'_{\hat{u}x', \hat{u}y', \hat{u}z'}$ rispetto a $O_{\hat{u}x, \hat{u}y, \hat{u}z}$.

Ricordando quanto detto nel capitolo precedente, possiamo constatare che:
$$\vec r (t) = \vec r_{O'}(t) + \vec{r'}(t)$$
Vorrei porre l'attenzione nel caso in cui il sistema di riferimento $O'_{\hat{u}x', \hat{u}y', \hat{u}z'}$ ruoti rispetto al sistema di riferimento principale, in questo caso i versori, come detto in precedenza, varieranno nel tempo, diventando quindi anch'essi funzioni:
$$\vec {r'} = x' (t) \hat u_x'(t) + y' (t) \hat u_y'(t) + z(t)' \hat u_z'(t)$$
Se adesso vogliamo andare a determinare la velocità oppure l'accelerazione, dovremo derivare anche i versori, poiché questi, non essendo costanti, non si annullano come succede normalmente in un sistema inerziale.

Per derivare un versore si sfrutta la \textbf{Formula di Poisson}, la quale ci dice che:
$$\frac{d\hat u(t)}{dt} = \omega \times \hat u (t)$$
dove $\omega$ è il vettore della velocità angolare del sistema di riferimento $O'$ rispetto a $O$, con direzione lungo l'asse di rotazione.

Dimostriamo ora questo passaggio:
![[formula di poisson.png|300]]
Avremo quindi:
$$
\begin{gather}
\hat u_x' (t)= 1 \cdot cos(\theta(t)) \hat u_x + 1 \cdot sin(\theta(t))\hat u_y\\

\frac{d\hat u_x'(t)}{dt} = -sin(\dot{\theta}(t))\hat u_x + cos(\dot{\theta}(t))\hat u_y
\end{gather}
$$
Adesso dimostriamo che $\vec \omega = \dot \theta (t) \hat u_z$:
$$
\begin{gather}
\frac{d\hat u_x'(t)}{dt} = \vec \omega \times \hat u_x\\

\vec \omega \times \hat u_x = \dot \theta (t) \hat u_z \times (cos(\theta(t))\hat u_x + sin(\theta(t))\hat u_y)\\

\implies \dot \theta (t) cos(\theta(t))(\hat u_x \times \hat u_z) + \dot \theta (t) sin(\theta (t))(\hat u_z \times \hat u_y)\\

\implies -sin(\theta(t))\dot \theta (t) \hat u_x + cos(\theta (t))\dot \theta (t) \hat u_y

\end{gather}
$$

Abbiamo quindi dimostrato che $\vec \omega$ è il vettore velocità angolare, diretto lungo l'asse di rotazione, il cui modulo è $\dot \theta(t)$ e il cui verso è ottenibile mediante la regola della mano destra:
$$
\begin{gather}
\text{Se} \quad \dot \theta (t) > 0 \implies \vec{\omega}>0\\

\text{Se} \quad \dot \theta (t) < 0 \implies \vec{\omega}<0

\end{gather}
$$
Adesso possiamo procedere nel derivare la legge oraria della posizione per ottenere la velocità:
$$\vec{v} = \vec{v}_{O'}(t) + \vec{v'}(t) + \vec{\omega} \times \vec{r'}(t)$$
Deriviamo nuovamente così da trovare l'accelerazione:
$$\vec{a}(t) = \vec{a'}(t) + \vec{a}_{O'}(t) + \vec{\dot \omega} \times (\vec \omega \times \vec{r'}) + 2\vec \omega \times \vec v$$
Analizzando la formula avremo che:
$$
\begin{gather}
\vec{a}_{O'}(t) + \vec{\dot \omega} \times (\vec \omega \times \vec{r'}) \quad = \quad \text{accelerazione di trascinamento}\\

2\vec \omega \times \vec v \quad = \quad \text{accelerazione di Coriolis}
\end{gather}
$$
Adesso andiamo a studiare l'equazione del moto:
$$
\begin{gather}
F_{vere} = m\vec a\\

m\vec{a'} = m(\vec a - vec a_T - vec a_C) \implies m\vec{a'} = F_{vere} - m\vec a_T -m\vec a_C 
\end{gather}
$$
Siamo arrivati quindi al risultato che se osserviamo il sistema da un punto di riferimento non inerziale allora oltre alle forze vere avremo anche la **forza di trascinamento** e la **forza di Coriolis**.

Andiamo ora a studiare un caso specifico di quando queste forze entrano in gioco: Consideriamo un pacco che si trova sopra il sedile di un auto, l'auto frena con un accelerazione $\vec a = -3[\frac{m}{s^2}]$. L'esercizio chiede di trovare il coefficiente di attrito statico affinché il pacco non cada.
![[esercizio 1 forze fittizie.png|300]]
Analizziamo le forze in gioco:
$$
\begin{gather}
\vec{N} = N \hat u_y'\\

\vec F_p = -mg \hat u_y'\\

\vec F_T = m \vec a_m \hat u_x'\\

\vec F_{as} = - F_{as} \hat u_x'

\end{gather}
$$
Possiamo notare che il sistema di riferimento è non inerziale perchè anche se il pacco è fermo rispetto all'auto, l'auto sta frenando, quindi il pacco si muove rispetto al sistema di riferimento dell'auto, sarà presente quindi la forza di trascinamento.

Adesso studiamo in caso in cui il sistema sia in equilibrio:
$$
\begin{gather}
m\vec a' = 0 F_{vere} + F_{fittizie} \\

(N-mg)\hat u_y' + (m\vec a_m - F_{as})\hat u_x =0\\

\text{Ricordiamo che} \quad F_{as} \leq \mu_s N\\

\begin{cases}

N=mg\\

F_{as}=m\vec{a}_m

\end{cases} \\

F_{as}=m\vec{a}_m \implies \mu_s N \geq m\vec{a}_m\\

\mu_s \geq \frac{\vec a_m}{g}

\end{gather}
$$

Se sostituiamo i dati otterremo che:
$$\mu_s \geq \frac{3}{g} = 0,3$$
**Quando il punto materiale non si muove rispetto al sistema di riferimento non inerziale l'unica forza fittizia è la forza di trascinamento**.

Adesso studiamo un altro caso specifico, un bambino seduto sul girello:
![[esercizio 2 forze fittizie.png|300]]
Possiamo notare che essendo il bambino seduto, la sua velocità rispetto al sistema di riferimento sarà nulla: $\vec{v'}=0$ perciò avremo soltanto la forza di trascinamento.  

Il vettore $\omega$ è costante e uguale a $\dot{\theta}(t)\hat u_z$, sappiamo infine che il girello è fisso, quindi $\vec a_{O'}=0$.

Analizziamo ora le forze in gioco:

Ruotando con velocità angolare costante, il girello visto da un sistema inerziale non sarà soggetto a forze vere, se però osserviamo il girello da un sistema di riferimento non inerziale noteremo che sarà presente la forza centrifuga, poiché è presente una velocità angolare:
$$\vec{F}_centrifuca = -m(\vec \omega \times (\vec \omega \times \vec{r'}))$$
Analizzando il sistema possiamo dedurre che:
$$
\begin{gather}
\vec{r'}=R \hat u_x'\\

\vec \omega = \dot \theta \hat u_z'

\end{gather}
$$
Adesso procediamo con i calcoli:
$$
\begin{gather}
\vec \omega \times \vec{r'} = \vec{\dot \theta}R \hat u_y'\\

\vec \omega \times (\omega \times\vec{r'}) = -\vec{\dot \theta}^2 R \hat u_x'

\end{gather}
$$
Abbiamo quindi definito che:
$$\vec{F}_{centrifuga} = -\vec{\dot \theta}^2 R \hat u_x'$$