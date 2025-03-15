#uni 
Si definisce **vincolo** qualcosa che ridice la libertà di movimento di un corpo attraverso delle forze.

Il termine **reazioni** sta a indicare che questi vincoli agiscono (imprimono forze) solo se sollecitate in modo opposto.

N.B. le reazioni vincolai sono incognite a priori, dipendono dallo sforzo a cui è sottoposto il vincolo.

Sono considerati \textbf{vincolo ideali} dei vincolo lisci che applicano forze perpendicolari al vincolo.

![[reazioni vincolari ideali piano inclinato.png|500]]
Quegli rappresentati in figura sono due casi di vincoli ideali, la massa $m_1$ subirà una reazione vincolare dal piano inclinato, mentre $m_2$ subirà una reazione vincolare dal piano orizzontale, ipotizziamo che la reazione vincolare in entrambi i casi sia sufficiente per sorreggere la massa.

Analizziamo per primo il caso di $m_2$, in questo caso la reazione vincolare:
$$N=F_p$$
Adesso analizziamo il caso di $m_1$ in cui andiamo a scomporre la forza peso in una componente parallela e una perpendicolare al piano, la reazione vincolare:
$$N=F_psin(\theta)$$
La $m_2$ non si troverà quindi in una posizione di equilibrio, sarà soggetta a una forza lungo l'asse $\hat{u}_x$ pari a $\sum F_x = F_p cos(\theta)$.
## Pendolo semplice
Per studiare il moto del pendolo semplice osserviamo un caso specifico:
![[pendolo semplice.png|300]]
Consideriamo $L$ come un filo ideale, inestensibile e di massa trascurabile, possiamo notare che la traiettoria del pendolo è nota, perciò interpelliamo le coordinate intrinseche.

Per la definizione di radiante osserviamo che:
$$s(t)=L\theta(t)$$Scomponendo la forza peso lungo la direzione del filo otterremo che:
$$F_p=-mg\cdot sin(\theta)\hat{\tau}-mg\cdot cos(\theta)\hat{n}$$La reazione vincolare del filo si troverà lungo la sua direzione: $\vec{T}=T\hat{n}$, con $T \geq 0$.

Adesso analizziamo l'equazione del moto $\vec{F}=m\vec{a}$:
$$\sum\vec{F}=-mgsin(\theta)\hat{\tau}-mgcos(\theta)\hat{n}+T\hat{n}$$
Possiamo inoltre definire $\vec{a}=\ddot{s}(t)\hat{\tau}+\frac{\dot{s}(t)}{L}\hat{n}$.

Unendo le formule otterremo che $\vec{a}$:
$$
\vec{a}=\begin{cases}
-gsin(\theta(t))\hat{\tau}=\ddot{s}(t)\hat{\tau}\\
-mgcos(\theta(t))\hat{n} + T\hat{n} = \frac{m\dot{s}(t)}{L}\hat{n}
\end{cases}
$$
In precedenza avevamo definito $s(t)=L\theta(t)$ possiamo quindi derivando ottenere che $\ddot{s}(t)=\ddot{\theta}(t)L$ sostituendo questa uguaglianza nel sistema precedente otterremo:
$$
\vec{a}=\begin{cases}
L\ddot{\theta}(t)=-gsin(\theta)\\
\frac{m(L\dot{\theta}(t))^2}{L}=-mgcos(\theta(t))+T
\end{cases}
$$
Sostituendo possiamo isolare $T=\frac{m(L\dot{\theta}(t))^2}{L}+mgcos(\theta(t))$.

Conoscendo l'accelerazione tangenziale: $\ddot{s}(t)=L\theta(t)$ e conoscendo la $\sum\vec{F}_t=-mgsin(\theta)$, tramite l'equazione del moto lungo le forze tangenziali possiamo ricavare che:
$$\ddot{\theta}(t)=-\frac{g}{L}sin(\theta(t)) \implies \theta(t)=\frac{g}{L}sin(\theta(t))$$
Grazie allo sviluppo di Taylor abbiamo imparato che $sin(\theta)\approx \theta$, segue che per $\theta$ molto piccoli la legge oraria del moto del pendolo sarà:
$$\ddot{\theta}(t)=\frac{-g}{L}\theta(t)$$
Con un po' di attenzione questa legge oraria ci ricorda quella del moto armonico con elemento forzante, dove $w=\sqrt{\frac{g}{l}}$.

Possiamo quindi calcolare il periodo di oscillazione:
$$T_{periodo}=\frac{2\pi}{w}=2\pi \sqrt{\frac{L}{g}}$$mentre la tensione del filo sarà:
$$T=m\dot{\theta}^2(t)+mgcos(\theta(t))$$
Essendo dipendente da $cos(\theta(t))$ la tensione sarà massima per $\theta=0$.
## Vincoli non ideali: attrito
Nei vincoli non ideali, denominati anche **vincoli reali** possiamo trovare anche una componente parallela al vincolo, come nel caso della **forza di attrito radente**.

La forza di attrito radente è una forza che si oppone al movimento e può essere di due tipologie:
- **attrito statico**, quando il punto materiale non si muove rispetto al vincolo;
- **attrito dinamico** quando il punto materiale è in movimento rispetto al vincolo.
- 
La forza di attrito statico è una forza incognita a priori e può assumere valori limitati:
$$\vec{F}_s \leq \mu_s|\vec{N}|$$
dove $\mu_s$ rappresenta il coefficiente di attrito statico\footnote{i coefficienti di attrito dipendono dai materiali a contatto}.

Il coefficiente di attrito dinamico invece sarà:
$$\vec{F}_d=\mu_d|\vec{N}|$$
dove $\mu_d$ rappresenta il coefficiente di attrito dinamico.

Per studiare quello che è il contributo dell'attrito, analizziamo un esempio:

Prendiamo un corpo di massa $m$ sopra un superficie scabra\footnote{Con attrito}, con $\mu_s$ e $\mu_d$ note, e applico una forza $F$
![[attrito.png|300]]
Le forze in gioco sono: $\vec{F}=F\hat{u}_x$, $\vec{F}_{as}=-F_{as}\hat{u}_x$ con $|\vec{F}_{as}|\leq \mu_s|\vec{N}|$, oppure $\vec{F_{ad}}=\mu_d|\vec{N}|\hat{u}y$; $\vec{N}=N\hat{u}_y$, $\vec{F_p}=-mg\hat{u}_y$.

Ipotizziamo che il corpo sia fermo, $\ddot{y}(t)=\ddot{x}=0$, avremo quindi che:
$$
\begin{cases}
F-F_a=0\\
N-mg=0
\end{cases}
$$
$$N=mg$$
considerando che $F_{as} \leq \mu_sN$ avremo che:
$$F_{as} \leq \mu_smg$$
Sostituendo questa uguaglianza nel sistema iniziale otteniamo che il corpo sarà fermo solamente se:
$$F \leq \mu_smg$$
Nel caso in cui la forza fosse maggiore dovremmo considerare la presenza dell'attrito dinamico e quindi:
$$\vec{F}-\vec{\mu_dmg}=m\ddot{x}(t)\hat{u}_x$$
### Attrito nel piano inclinato
Adesso studiamo il comportamento dell'attrito in piano inclinato scabro, analizzando un caso specifico:
![[Attrito piano inclinato.png|300]]
le forze in gioco:
$$
\begin{gather}
\sum F_y = N-mgcos(\theta)\\
\sum F_x = mgsin(\theta)-F_a
\end{gather}
$$
quindi segue che per ottenere l'equilibrio:
$$
\begin{gather}
N=mgcos(\theta)\\
F_a=mgsin(\theta)
\end{gather}
$$
Perciò ricordando che $F_{as} \leq \mu_s N$, il corpo sarà in equilibrio solamente se:
$$mgsin(\theta) \leq \mu_s(mgcos(\theta)) \implies \mu_s \geq \frac{sin(\theta)}{cos(\theta)}$$