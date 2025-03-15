#uni 
La forza elastica è la forza che un corpo elastico imprime quando viene deformato, compresso o allungato, tendendo a tornare alla forma originale.

Secondo la legge di Hook, la forza elastica è data da:

$$
\vec{F_{el}}=-k \cdot \Delta l
$$
dove, $\Delta l$= deformazione del materiale; $k$= coefficiente elastico del materiale:
$$
 k = \frac{E \cdot s}{L}
$$
dove $E$= modulo di Young, che dipende dal materiale; $L$= lunghezza iniziale; $s$= superficie.
Si può notare andando a sostituire k nella formula originale che $\Delta l$ è:
- proporzionale alla forza $F$ applicata al corpo;
- proporzionale alla lunghezza iniziale $L$;
- inversamente proporzionale alla superficie $s$;
- varia in base al materiale attraverso $E$, al crescere di E il materiale è più rigido.

Se prendiamo in esame una molla posizionata parallelamente all'asse x, bloccata a una estremità, che subirà una deformazione parallela all'asse x, possiamo scrivere la forza elastica come:
$$
 F_{el}=-k(x-L) \cdot \hat{u}_x
$$
dove $x$ è la posizione in cui si trova l'estremità mobile.
![[Molla.png|500]]
## Moto Armonico
Il moto armonico è la legge oraria che descrive la posizione di una massa collegata all'estremità di una molla, sottoposta a un'oscillazione.
![[grafico moto armonico .png|500]]

Prima di andare a determinare le leggi orarie di questo moto dobbiamo introdurre alcuni concetti:
- $T[s]=2 \pi \sqrt{\frac{m}{k}}$: il periodo, il tempo necessario a compiere un oscillazione;
- $f[\frac{1}{s}]=\frac{1}{T}$: la frequenza, quante oscillazioni sono presenti in un secondo.
- $w[\frac{rad}{s}]$: la pulsazione, frequenza angolare
- $A=\Delta l_{max}$: l'ampiezza di oscillazione.

Adesso che abbiamo introdotto questi nuovi concetti possiamo analizzare la legge oraria semplificata del moto armonico:

$$x(t)= Acos(wt+ \phi)$$

Possiamo notare che $-1<cos(wt+ \phi)<1$ e osservando il grafico possiamo notare come questo sia verosimile, la massa oscillerà tra $-A$ e $+A$.

Se analizziamo la legge oraria dell'accelerazione, ricavabile semplicemente derivando due volte la legge oraria della posizione, otterremo:
$$\ddot{x}(t)=-Aw^2cos(wt+\phi)$$
Possiamo notare che $Acos(wt+\phi)=x(t)$ perciò possiamo semplificare questa legge oraria come:

$$\ddot{x}(t)=w^2x(t)$$
  La legge oraria dell'accelerazione può essere ricavata anche attraverso il secondo principio della dinamica:
$$\sum \vec{F} = m \vec{a} \implies \ddot{x}=\frac{-k}{m}x$$Ponendo $L=0$ e $\vec{a}=\ddot{x}$ come nel grafico.
Se adesso andiamo a unire le uguaglianze otterremo che:
$$w=\sqrt{\frac{k}{m}} \implies T=2 \pi \sqrt{\frac{m}{k}}$$
Queste nuove equazioni possono essere utili per ricavare $w$ oppure $k$ negli esercizi.

**Esercizio**
Prendiamo una molla posta parallela all'asse x, \nameref{fig:Molla} e consideriamo la posizione iniziale $x(0)=0m$, $k=10 \frac{N}{m}$ $m=0,1kg$ e che la velocità iniziale $\dot{x}(0)=-3 \frac{m}{s}$

Riscriviamo le leggi orarie del moto armonico:

\begin{equation}

\begin{cases}
$$
\begin{cases}
x(t) = Acos(wt + \phi)\\
\dot{x}(t)=-Awsin(wt+\phi)\\
\ddot{x}(t)=-Aw^2cos(wt+\phi)
\end{cases}
$$

Andiamo a sostituire $t=0$, $x(0)=0$ e $\dot{x}(0)=-3$:
$$x(0)=0 \implies A cos(\phi)=0$$

essendo $A \neq 0 \implies cos(\phi)=0 \implies \phi=\frac{\pi}{2}$ oppure $\phi = \frac{3\pi}{2}$.

Adesso calcoliamo $w$
$$w=\sqrt{\frac{k}{m}}=\sqrt{\frac{10}{0,1}}=10\frac{rad}{s}$$
Ora possiamo andare a sostituire nell'equazione della velocità iniziale:
$$\dot{x}(0)=-3 \implies 10\cdot A \cdot sin(\frac{\pi}{2})=-3\implies A=0,3$$
Da notare che se avessi scelto $\phi=\frac{3\pi}{2}$ il risultato sarebbe stato lo stesso con il segno opposto perché l'oscillazione della molla sarebbe iniziata da una compressione invece che da una trazione.

Adesso che ho ricavato anche $A$ posso scrivere la legge oraria della posizione:
$$x(t)=0,3cos(10t+\frac{\pi}{2})$$
*Fine esercizio.*

Da formulario la legge oraria del moto armonico è:

$$x(t)=(x(0)-\frac{a}{w^2})cos(wt)+ \frac{v(0)}{w}sin(wt)+\frac{a}{w^2}$$
Per quanto possa sembrare molto complessa in realtà è molto simile alla versione semplificata vista in precedenza:
- $a=\frac{F}{m}$ è elemento forzante, dove $F$ è una forza che agisce sulla molla, per esempio la forza peso se la molla fosse posta lungo l'asse y;
- la seconda parte composta da $\frac{v(0)}{w}sin(wt)$ va semplicemente a sostituire quello che era l'angolo di sfasamento $\phi$ e va a considerare quella che è l'oscillazione generata dalla velocità iniziale, la sostituzione viene eseguita considerando $tg(\phi)=-\frac{v(0)}{w\cdot x(0)}$.

Il moto smorzato è un moto che porta alla decelerazione, o accelerazione, del corpo fino a una certa quantità, oltre la quale la velocità rimane costante, per quanto non sia intuitivo, nei capitoli successivi andremo a verificarlo con dei moti specifici.

Nel formulario la legge oraria del moto smorzato è data come:

$$x(t)= \frac{1}{\Gamma}(v(0)-\frac{a}{\Gamma})(a-e^{-\Gamma t})+\frac{a}{\Gamma}t+x(0)$$

Questa legge oraria si è ottenuta seguendo questo procedimento:

$$\vec{F}=m\vec{a} \implies \ddot{x}(t)=-\Gamma \dot{x}+a \implies\ddot{x}=(a-v(0)\Gamma)e^{-\Gamma t}$$
e successivamente derivando.

Come per il moto armonico, questa legge oraria non è complicata come sembra in quanto l'unico termine che non avevamo considerato in precedenza è $a=\frac{F}{m}$ e rappresenta come per il moto armonico il termine forzante.

  

## Moto Armonico + Termine Forzante
Prende il nome di \textbf{termine forzante} una forza che altera il punto di equilibrio della molla.
![[moto armonico smorzato schema.png|300]]

Per andare a determinare le leggi orarie di questo moto, partiamo dall'equazione del moto: $\sum\vec{F}=m\vec{a}$:
$$\sum \vec{F}=F_p+F_e = -mg\hat{u}_y - k(y(t)+L)\hat{u}_y \implies\ddot{y}(t)=-g -\frac{k}{m}(y(t)+L)$$
Si nota che la Forza elastica è data da $\vec{F}_{el}=-k(y(t)+L)$ e non $\vec{F}_{el}=-k(y(t)-L)$ perché con $L$ viene indicato il valore assoluto della lunghezza e pertanto il segno varia in base al verso in cui è disposta la molla.

Semplificando la formula con: $-\frac{kL}{m}-g=a$ denominando $a$ termine forzante, otteniamo:
$$\ddot{y}(t)=-\frac{k}{m}y(t)+a$$

Si definisce **punto di equilibrio** il punto in cui, partendo da fermo, in assenza di forze esterne, il punto rimane fermo:
$$\dot{y}(0)=0, y(0)=y_{eq},\vec{F}_{esterne}=0 \implies \ddot{y}(t)=0$$

Perciò per trovare il nuovo punto di equilibrio posso porre $\ddot{y}(t)=0$

$$\ddot{y}(t)=0 \implies -\frac{k}{m}y_{eq}(t)+a=0\implies y_{eq}(t)=\frac{ma}{k}$$
  
- Con questa precisazione abbiamo definito al meglio le leggi orarie note sul formulario:\label{leggi orarie moto armonico formulario}

$$
\begin{cases}
x(t)=(x(0)-\frac{a}{w^2})cos(wt)+\frac{v(0)}{w}sin(wt)+\frac{a}{w^2}\\
\dot{x}(t)=(\frac{a}{w}-x(0)w)sin(wt)+v(0)cos(wt)\\
\ddot{x}(t)=(a-x(0)w^2)cos(wt)-v(0)wsin(wt)=w^2x(t)+a
\end{cases}
$$

Un altro modo per studiare questo sistema è quello di andare a \textbf{cercare} un nuovo **sistema di riferimento**, per esempio possiamo porre lo $0$ del nostro sistema di riferimento nella posizione di equilibrio:

Essendo in una posizione di equilibrio, $\ddot{y}(t)=0 \implies \sum \vec{F}=0 \implies k(y_{eq}+L)=-mg$ isolando $y_{eq}$ otterremo:

$$y_{eq}=-L+\frac{mg}{k}$$

Da notare ancora che il termine $L$ è cambiato di segno perché la molla è orientata negativamente rispetto al versore $\hat{u}_y$.

Infine otteniamo che la posizione $y'(t)$, la posizione della massa osservata rispetto al punto di equilibrio sarà:

$$y'(t)=y(t)+dist(0-y_{eq})=y(t)-L+\frac{mg}{k}$$

Derivando possiamo notare che le leggi orarie della velocità e dell'accelerazione rimangono le stesse, perciò avremo:
$$\ddot{y'}(t)= -\frac{k}{m}y'(t)$$
Perciò se pongo il mio sistema di riferimento nel punto di equilibrio $y_{eq}$ il sistema avrà le stesse leggi orarie del **moto armonico semplice**.