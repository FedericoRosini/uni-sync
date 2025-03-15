#uni 
## Forze Dissipative
Prendono il nome di **forze dissipative** quelle forze che vanno a "dissipare, diminuire, l'energia cinetica.

In altre parole si tratta delle forze che si oppongono al moto, come per esempio le forze di attrito, rappresentate quindi con il verso opposto alla forza che agisce sul punto materiale.

## Forze Posizionali
Prendono il nome di **forze posizionali** quelle forze che dipendono esclusivamente dalla posizione del punto materiale, queste forze possono essere scritte mediante la relazione:
$$\vec{F}=F(\vec{r})$$
Le forze posizionali hanno un importante proprietà:
$$L_{A\rightarrow B} = -L_{B \rightarrow A}$$
## Forze conservative
Prendono il nome di **forze conservative** quelle forze il cui lavoro non dipende dal percorso che ha eseguito ma unicamente dal punto iniziale e finale, per esempio la **forza peso** e la **forza elastica** sono due forze conservative. 

Per capire al meglio questa tipologie di forze analizziamo un esercizio:
![[esercizio forze conservative.png|300]]
In questo schema troviamo un punto materiale di massa $m$ che viene lasciato cadere partendo da un punto iniziale $A$ lungo una traiettoria rettilinea $\gamma_1$ fino a un punto $B$, oppure lungo una traiettoria semicircolare $\gamma_2$.

Ricordiamo che come visto in precedenza la forza peso $F_p$ è una forza posizionale e pertanto non dipende dalla traiettoria del punto materiale:
$$L_{AB}=\int_A^B{\vec{F}_p d\vec{s}}$$

Il lavoro compiuto dal punto materiale lungo la traiettoria $\gamma_1$ è lo stesso che avevamo analizzato in precedenza \ref{fig:esercizio teorema delle forze vive}:
$$L_{AB}=mg2R$$
Andiamo adesso ad analizzare il lavoro compiuto dal punto materiale nella traiettoria $\gamma_2$:

Avendo una traiettoria nota, possiamo utilizzare le coordinate intrinseche, attraverso le quali possiamo riscrivere la forza peso come:
$$\vec{F}_p = mg(cos(\theta)\hat{n} + sin(\theta)\hat{s})$$
possiamo scrivere il vettore $d\vec{r}$, che rappresenta la lo spostamento circolare, come il vettore spostamento lungo l'asse y, vincolato alla traiettoria:
$$
\begin{gather}
d\vec{r} = d\vec{s}\hat{\tau}\\

\vec{s} = R\theta \implies d\vec{r}=Rd\theta \hat{\tau}

\end{gather}
$$
Adesso possiamo riscrivere il lavoro come:
$$
\begin{gather}
L_{AB\gamma_2} = \int_{\theta_A}^{\theta_B}{mg(cos(\theta))\hat{n} + sin(\theta)Rd\theta \hat{\tau}} \\

L_{AB\gamma_2} = \int_{0}^{2\pi}{mgsin(\theta)Rd\theta} \\

L_{AB\gamma_2} = mgR(-cos(\theta))\big|_0^{\pi}\\

L_{AB\gamma_2} = mgR[1+1] = 2mgR

\end{gather}
$$
  
Nel passaggio 2 è stato separato l'integrale; l'integrale con dentro il coseno non è stato considerato perché integrandolo sarebbe diventato $sin(\theta)$ e calcolato tra $0$ e $\pi$ si sarebbe annullato}

Abbiamo quindi definito che il lavoro impiegato dalla forza peso è lo stesso indipendentemente dalla traiettoria, dipenderà unicamente il punto di partenza e il punto di arrivo.
## Teorema delle forze conservative
Una forza si dice conservativa $\iff$ esiste una funzione scalare $U(\vec{r})$ della posizione $\vec{r}$ t.c.:
$$L_{AB} = U(\vec{r}_A) - U(\vec{r}_B)$$
**Dimostrazione:**
$\impliedby$ è dimostrato dalla definizione, non essendo rilevante la traiettoria;
$\implies$ Assumiamo che $\vec{F}$ sia conservativa, avremo che:

$$U(\vec{r})=-\int_0^{\vec{r}}{\vec{F}d\vec{s}}$$
Questa funzione è ben definita anche senza specificare la traiettoria poiché la forza è conservativa, possiamo scrivere quindi:
$$
\begin{gather}
L_{AB} = \int_A^B{\vec{F}d\vec{s}}\\

L_{AB} = \int_A^0{\vec{F}d\vec{s}}+\int_0^B{\vec{F}d\vec{s}}\\

L_{AB} = -\int_0^A{\vec{F}d\vec{s}}+\int_0^B{\vec{F}d\vec{s}}\\

L_{AB} = -\int_0^A{\vec{F}d\vec{s}}- \Big(-\int_0^B{\vec{F}d\vec{s}}\Big)\\

U(\vec{r}_A) = -\int_0^A{\vec{F}d\vec{s}} ;\quad U(\vec{r}_B)=-\int_0^B{\vec{F}d\vec{s}}

\end{gather}
$$
Abbiamo quindi ottenuto che:
$$L_{AB}=U(\vec{r}_A)-U(\vec{r}_B)$$

*Fine dimostrazione*

Questa nuova equazione ci può essere utile per esempio nell'esercizio \ref{fig:esercizio forze conservative} in cui abbiamo verificato che il lavoro svolto è: $L_{AB} = 2mgR$, generalizzando possiamo ottenere che:
$$U(\vec{r}) = mgy$$
e prende il nome di \textbf{energia potenziale}.

N.B. L'energia potenziale dipende dal sistema di riferimento, ma la sua differenza no.
## Teorema della conservazione dell'energia meccanica
Assumiamo che il solo lavoro delle forze sai eseguito da forze conservative, considerando che le forze vincolari non compiono mai lavoro poiché sono perpendicolari, avremo che:
$$
\begin{gather}
L_{AB} = U_A - U_B

L_{AB} = T_B - T_A

U_A + T_A = U_B + T_B

\end{gather}
$$
Consideriamo quindi $T+U = cost$ e prende il nome di \textbf{energia meccanica}.