#uni 
L'attrito viscoso si presenta quando siamo all'interno di un **fluido**, ogni particella del fluido trasferirà al nostro corpo una certa quantità di moto $\vec{q}$, nel caso in cui l'impatto sia completamente elastico, la particella rimbalzerà, trasferendo quindi un totale di quantità di moto pari a $2q$ per collisione.

Quando la velocità del corpo rispetto alla velocità del fluido è nulla, allora il numero di particelle che colpiscono il corpo da sinistra sarà bilanciato dal numero di particelle che impatteranno da destra, pertanto la quantità di moto trasferita dal fluido al corpo sarà nulla.

$$(v_{corpo}-v_{fluido})=0 \implies \sum q=0$$
![[attrito viscoso.png|500]]
Poniamo per ipotesi di avere questo corpo immerso in un fluido e che $v_{corpo} \ne v_{fluido}$, in un intervallo di tempo $\Delta t$ il corpo sposta un volume di fluido pari a $V=s(v_{corpo}-v_{fluido})\Delta t$, il numero di collisioni che il nostro corpo avrà con le particelle del fluido sarà uguale a $n \cdot V$ dove $n$ rappresenta la densità di particelle all'interno del fluido.

Sostituendo la formula otterremo che:
$$n \cdot V=ns(v_{corpo}-v_{fluido})\Delta t$$
Perciò, ricordando che la quantità di moto trasferita da una particella è di circa $2q$, possiamo dire che la quantità di moto trasferita dal fluido al corpo sarà uguale a:
$$\Delta \vec{Q}=ns(v_{corpo}-v_{fluido})\Delta t\cdot2q$$
Adesso ricordando la proprietà vista nel capitolo precedente \ref{quantità di moto} possiamo dire che:
$$|\vec{F}|=\frac{ns(v_{corpo}-v_{fluido})\Delta t\cdot2q}{\Delta t}=ns(v_{corpo}-v_{fluido})\cdot2q$$
Ponendo $ns\cdot2q=\Gamma$ che rappresenta il coefficiente di attrito viscoso, otteniamo che:
$$|\vec{F}|=\Gamma(v_{corpo}-v_{fluido})$$
Il verso del vettore sarà dato dal verso delle due velocità.

## Moto smorzato
Il moto smorzato è un moto che porta alla decelerazione o accelerazione del corpo fino a una certa quantità, oltre la quale la velocità rimane costante, per quanto non sembri intuitivo, nei capitoli successivi andremo a verificarlo con dei moti specifici.

Nel formulario la legge oraria del moto smorzato è data come:
$$x(t)= \frac{1}{\Gamma}(v(0)-\frac{a}{\Gamma})(a-e^{-\Gamma t})+\frac{a}{\Gamma}t+x(0)$$
Questa legge oraria si è ottenuta seguendo questo procedimento:
$$\vec{F}=m\vec{a} \implies \ddot{x}(t)=-\Gamma \dot{x}+a \implies\ddot{x}=(a-v(0)\Gamma)e^{-\Gamma t}$$
e successivamente derivando.

Come per il moto armonico questa legge oraria non è complicata come sembra in quanto l'unico termine che non avevamo considerato in precedenza è $a=\frac{F}{m}$ e rappresenta, come per il moto armonico, il termine forzante.

## Moto smorzato + Elemento forzante
Per analizzare questa tipologia di moto, analizziamo un esempio, consideriamo un paracadutista che cade da un aereo.
![[moto smorzato con elemento forzante schema.png]]

Il paracadutista sarà sottoposto alla sua forza peso e a una forza di attrito viscoso, dovuta dell'aria.

Ricordiamo che $F_v=-\Gamma(v-v_f)=-\Gamma \dot{y}(t)\hat{u}_y$\footnote{da notare il segno negativo dalla discordanza con il versore $\hat{u}_y$},considerando l'assenza di vento ($v_f=0$) mentre che $F_p=-mg$.

Perciò scrivendo l'equazione del moto otterremo:
$$\ddot{y}(t)=-\frac{\Gamma}{m}\dot{y}(t)+g$$
Dove $g$ rappresenta il termine forzante.

Dai dati dell'esercizio possiamo definire che $x(0)=0$ e che $\dot{y}(0)=0$, perciò sostituendo nella legge oraria della velocità otterremo che:
$$\ddot{y}(o)=-\frac{\Gamma}{m} \cdot 0 + g \implies\ddot{y}(0)=-g$$

Adesso vado a studiare il sistema in un tempo $t_1 \ne t_0$, avrò che $\ddot{y}(o)=\frac{\Gamma}{m} \cdot \dot{y}(t_1) - g$ con $\dot{y}(t_1)\ne 0$.
  
Infine vado a studiare il tempo $t_2$ t.c. $\dot{y}(t_2)=g\frac{m}{\Gamma}$ ne segue che $\ddot{y}(t)=0$ e perciò dopo un tempo $t_2$ la velocità sarà costante.