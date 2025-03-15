[[E.M. L.1.pdf]]
**L'elettrostatica studia i sistemi dove le cariche sono ferme.**
I primi a parlare di elettrostatica sono stati i greci che avevano scoperto che se strofinate due bacchette di ambra queste poi attraevano oggetti. La parola elettricità deriva infatti a *electron* (ambra in greco).

Abbiamo imparato dal corso di fisica che la massa è il ponte che collega la causa con l'effetto:
$$
\vec{F} = m \vec{a} 
$$
- $\vec{F} =$ causa
- $\vec{a} =$ effetto

Oltre alla massa un'altra interazione tra punti materiali è data dalla **carica** '$q$', misurata secondo il sistema internazionale il Coulomb $[C]$. 

Questa carica la possiamo vedere a livello atomico, un atomo è composto infatti da  un nucleo, dove troviamo i **protoni** di carica positiva e intorno al nucleo si trova una nuvola di **elettroni** di carica negativa.

Rappresentando l'atomo come una sfera, il nucleo avrà un diametro di $10^{-12}m$, mentre la nuvola di elettroni è grande $10^{-10}m = 1Å$ 
$$
\begin{array}{c|c|c} 
 & p^+ & e^- \\ \hline
m & 1,7\cdot 10^{-27}kg & \frac{m_p}{1800}kg \\ \hline
q & 1,6\cdot 10^{-19}C & -1,6\cdot 10^{-19}C
\end{array}
$$
# Induzione elettrostatica
![[Elettrostatica 2025-02-28 18.11.21.excalidraw]]
[[Induzione elettrostatica]]
L'induzione elettrostatica è il fenomeno per cui la distribuzione di carica di un conduttore viene modificata dalla presenza di un corpo carico nelle vicinanze.

Per avere un induzione elettrostatica necessiteremo di due tipologie di materiali:
- materiale **dielettrico**, o isolante, le cui cariche stanno ferme;
- materiale **conduttore**, le cui cariche sono libere di muoversi.

La presenza del materiale dielettrico carico positivamente, porta le cariche del materiale conduttore a spostarsi asimmetricamente, questo deriva dal fatto che le cariche opposte si attraggono, mentre quelle uguali si respingono.
![[Elettrostatica 2025-02-28 21.45.25.excalidraw]]
Possiamo vedere come la forza che il materiale conduttore farà verso sinistra sia maggiore della forza che il materiale compie verso destra.

Per giustificare matematicamente questa osservazione dobbiamo introdurre la **forza di Coulomb:** 
![[Elettrostatica 2025-02-28 22.10.25.excalidraw]]
$$
\begin{gather}
\vec{F}_{12} = k \frac{q_1q_2}{r^{2}}\hat{r} \\
K=\frac{1}{4 \pi \epsilon_0} \\
\epsilon_0 = 8,85 \cdot 10^{-12}\left[ \frac{C^{2}}{Nm^{2}} \right]
\end{gather}
$$
*$\epsilon_0 =$ costante delle cariche elettrostatiche*

Questa formula ci dimostra anche perché cariche opposte si attraggono, mentre cariche uguali si respingono, si può notare dal segno del prodotto, che modifica il verso della forza.

Analizziamo ora cosa avviene all'interno del nucleo
![[Elettrostatica 2025-03-01 10.37.54.excalidraw]]

Possiamo calcolare la forza di Coulomb visto che tutti i dati sono noti:
$$
\vec{F}_p = \frac{1}{4 \pi \epsilon_0} \frac{q_p^{2}}{d^{2}}
$$
Dal corso di fisica conosciamo una forza di attrazione che agisce su tutti i corpi, la forza di gravità:
$$
F_g = G \frac{m_p^{2}}{d^{2}}
$$
Adesso andiamo a calcolare quanto questa forza incide nella forza elettrostatica calcolando il rapporto:
$$
\frac{|\vec{F}_{el}|}{|\vec{F}_g|} \approx 10^{36} 
$$
Siamo arrivati quindi alla conclusione che **la forza elettrica domina la forza di gravità** nella scala atomica.
# Campo elettrostatico
[[Campo elettrostatico]]
Quando abbiamo una carica sola nello spazio, quest'ultimo si deforma preparandosi a interagire con questa.

Prendiamo in esame una carica positiva $Q$ (per convenzione) nello spazio, per valutare lo stato del sistema dobbiamo introdurre una carica sonda $q$  positiva (per convenzione) che ha lo scopo di sviluppare la carica potenziale del sistema.
![[Elettrostatica 2025-03-01 10.44.44.excalidraw]]
La forza di interazione tra le due cariche sarà:
$$
\vec{F}_{el} = \frac{1}{4 \pi \epsilon_0} \frac{Q \cdot q}{r^{2}}\hat{r}
$$
Per studiare lo spazio in presenza di una sola carica non voglio avere $q$ all'interno della mia equazione, perciò introduco il concetto di **campo elettrico** $\vec{E}$:
$$
\begin{gather}
\vec{E} = \frac{\vec{F}}{q} \\
\vec{E} = \frac{1}{4 \pi \epsilon_0} \frac{Q}{r^{2}}\hat{r}
\end{gather}
$$
Da questa equazione possiamo ricavare l'inversa:
$$
\vec{F}=q \cdot \vec{E}
$$
Dato un campo elettrico posso trovare la forza che agisce sul corpo.

Generalizziamo ora il concetto di carica sonda, la carica possiamo posizionarla in qualsiasi punto nello spazio, avremo quindi che il campo elettrico è una sfera intorno alla carica con verso entrante o uscente in base al segno della carica.
![[Elettrostatica 2025-03-01 10.36.36.excalidraw]]
Queste forze che compongono il campo elettrico sono dette **linee di campo** e sono diverse dalla traiettoria del punto materiale, infatti un punto segue le traiettorie tangenti a queste linee, spostandosi da una a un'altra.
![[Elettrostatica 2025-03-01 10.45.25.excalidraw]]
Adesso scriviamo il campo elettrico $E$ in forma cartesiana:
Per prima cosa trasformiamo il versore $r\cdot\hat{r} \to \vec{r}$ :
$$
\vec{E} = \frac{1}{4 \pi \epsilon_0} \frac{Q \vec{r}}{r^{3}}
$$
consideriamo ora un punto materiale posto in $P:(x,y,z)$ e poniamo che la carica si trovi nell'origine $Q = (x_0,y_0,z_0)$
$$
\vec{E} = \frac{Q}{4 \pi \epsilon_0} \frac{(x-x_0)\hat{i}+ (y-y_0)\hat{j} + (z-z_0)\hat{k}}{([x-x_0]^{2} + [y-y_0]^{2} + [z-z_0]^{2})^{\frac{3}{2}}}
$$
dove:
- $\vec{r} = (x-x_0)\hat{i}+ (y-y_0)\hat{j} + (z-z_0)\hat{k}$
- $|\vec{r}|^3=([x-x_0]^{2} + [y-y_0]^{2} + [z-z_0]^{2})^{\frac{3}{2}}$
## Campo elettrico con più cariche
Suppongo di avere più cariche disposte nello spazio, posso subito stabilire che vicino alle sorgenti questi si comporteranno come nel caso di sorgenti isolate.\!![[Elettrostatica 2025-03-01 10.53.03.excalidraw]]
Tutte e tre le sorgenti andranno a interagire con la carica sonda
$$
\vec{E} = \frac{\sum_{i=0}^{3}\vec{F}_i}{q}=\sum_{i=0}^{3}\vec{E}_i
$$
La composizione dei campi elettrici sarà quindi data dalla **somma vettoriale** di questi, seguendo il principio di sovrapposizione.
# Dipolo Elettrico
**Un dipolo elettrico è un sistema costituito da due cariche elettriche di segno opposto, con lo stesso modulo e con una distanza finita l'una dall'altra.**
![[Elettrostatica 2025-03-01 11.52.34.excalidraw]]
Adesso vogliamo stabilire il campo elettrico in funzione di $x$

Scomponendo i vettori e sommandoli, possiamo notare che  le componenti lungo l'asse x si annullano e che quelle lungo l'asse y sono uguali:
$$
\begin{gather}
E_{tot} = 2 E^+ \sin(\theta) = 2\left[ \frac{1}{4 \pi \epsilon_0} \frac{q}{x^{2} + \left( \frac{d}{2} \right)^{2}} \right]\sin(\theta) \\
\sin(\theta) = \frac{\frac{d}{2}}{\sqrt{ x^{2} + \left( \frac{d}{2} \right)^{2} }} \\
E_{tot} = - \frac{1}{4 \pi \epsilon_0} \frac{qd}{\left[ x^{2} + \left( \frac{d}{2} \right)^{2} \right]^{\frac{3}{2}}} \hat{j}
\end{gather}
$$
Introduciamo ora il concetto **momento di dipolo** $\vec{p}$ , un vettore che va dalla carica negativa a quella positiva e con modulo $\vec{p} = d \cdot q \hat{j}$. 

Sostituendo questo nuovo elemento nell'equazione che abbiamo appena trovato:
$$
E_{tot} = - \frac{1}{4 \pi \epsilon_0} \frac{\vec{p}}{\left( x^{2}+ \left( \frac{d}{2} \right)^{2}\right)^{\frac{3}{2}}}
$$
avremo che $-\frac{\vec{p}}{4 \pi \epsilon_0}=\alpha$ che consideriamo costante;

Studiando ora l'andamento del campo elettrico rispetto all'asse x possiamo notare che per $x$ molto maggiori di $d$, la componente $d$ diventa trascurabile, pertanto:
$$
E_{tot} = \alpha\frac{1}{x^3}
$$
![[Elettrostatica 2025-03-01 11.59.43.excalidraw]]
[[Lezione 2.pdf]]
# Densità di carica
Studiamo come si sovrappongono i campi elettrici in dei sistemi con **densità di carica** uniforme.
## Volume
![[Elettrostatica 2025-03-07 11.48.58.excalidraw]]
Quando abbiamo un sistema tridimensionale avremo che:
$$
\rho  = \frac{dq}{dV}\left[\frac{C}{m^{3}}\right]
$$
Per la sovrapposizione delle cariche studiata in precedenza possiamo dire che:
$$
\vec{E}_p = \int_V d\vec{E} = \int_V \frac{1}{4 \pi \epsilon_0} \frac{dq}{r^{2}}\hat{r}
$$
Sostituendo $\rho_v$:
$$
\int_V \frac{1}{4 \pi \epsilon_0} \frac{\rho dV}{r^{2}}\hat{r}
$$
## Superficie
![[Elettrostatica 2025-03-07 11.58.14.excalidraw]]

In questo caso dobbiamo considerare la densità di carica rispetto alla superficie $\sigma$
Per la sovrapposizione delle cariche avremo che:
$$
\vec{E}_P = \int_S d \vec{E} = \int_S \frac{1}{4 \pi \epsilon_0} \frac{\sigma dS}{r^{2}} \hat{r}
$$
## Unidimensionale
![[Elettrostatica 2025-03-13 16.12.40.excalidraw]]
In questo caso dobbiamo considerare la densità di carica rispetto alla linea $\lambda$
Per la sovrapposizione delle cariche avremo che:
$$
\vec{E}_P = \int_L d \vec{E} = \int_L \frac{1}{4 \pi \epsilon_0} \frac{\lambda dL}{r^{2}} \hat{r}
$$
# Sovrapposizione dei campi
## Unidimensionale


**scrivere esempio del filo infinito**


Studiamo ora un esempio di un sistema unidimensionale, un **anello** di spessore infinitesimo.
![[Elettrostatica 2025-03-08 11.43.24.excalidraw|200]]
Sappiamo grazie al principio di sovrapposizione che:
$$
E_{tot} = \oint d\vec{E} = 0 \text{  (rispetto al centro)}
$$
dove $\oint$ rappresenta l'area di un percorso chiuso, l'annullarsi dell'integrale è dato dalla **simmetria** del sistema, infatti per ogni campo generato da un punto sull'anello, ne esiste un altro opposto che lo annulla.
![[Elettrostatica 2025-03-08 11.13.04.excalidraw|200]]
Studiamo ora di questo sistema un punto che esce dal piano su cui poggia l'anello con una distanza $x$ dal centro.
![[Pasted image 20250308112004.png]]
Poiché le componenti del campo lungo l'asse $y$ si annullano possiamo calcolare il campo con un integrale semplice che calcola la somma dei moduli delle componenti orizzontali del campo:
$$
\begin{gather}
\vec{E}_{tot} = \oint \frac{1}{4 \pi \epsilon_0} \frac{\lambda dl}{r^{2}}\cos\theta \\
= \frac{1}{4 \pi \epsilon_0}\oint  \frac{\lambda dl}{r^{2}}\cos\theta \\
=\frac{\lambda}{4 \pi \epsilon_0r^{2}} \oint dl\cos\theta \\
\cos\theta = \frac{x}{\sqrt{R^{2} + x^{2}}}  \implies \frac{1}{4\pi\epsilon_0} \frac{\lambda x}{(R^{2}+x^{2})^{\frac{3}{2}}} \oint dl\\
\oint dl = 2 \pi R \implies \frac{1}{2\epsilon_0} \frac{\lambda R x}{(R^{2}+x^{2})^{\frac{3}{2}}}
\end{gather}
$$
Facciamo ora un esempio di un possibile esercizio:

Scrivere l'equazione del moto di un elettrone in funzione della distanza dal centro di un anello unidimensionale, e calcolare il tempo $\tau$ che impiega partendo da una posizione x ad arrivare al centro del cerchio:
![[Pasted image 20250308120108.png]]
Sappiamo che la forza di Coulomb applicata sulla carica è:
$$
\vec{F} = q_e \vec{E} = -|q_e|\vec{E}
$$
Ricordando l'esempio fatto in precedenza sappiamo che:
$$
\vec{E} = \frac{1}{2\epsilon_0} \frac{\lambda Rx}{(x^{2} + R^{2})^{\frac{3}{2}}}
$$
Possiamo quindi riscrivere la forza applicata all'elettrone come:
$$
\vec{F} = \frac{-|q_e|}{2\epsilon_0} \frac{\lambda Rx}{(x^{2} + R^{2})^{\frac{3}{2}}}
$$
Per il secondo principio della dinamica, $\vec{F} = m \vec{a}$.
$$
m\ddot{x} = \frac{-|q_e|}{2\epsilon_0} \frac{\lambda Rx}{(x^{2} + R^{2})^{\frac{3}{2}}} 
$$
studiando il sistema per $x\ll R$ nel denominatore del secondo componente $x$ diventa trascurabile
$$
\ddot{x} = -\frac{|q_e|\lambda Rx}{2\epsilon_0(R^{2})^{\frac{3}{2}}}
$$
Possiamo riconoscere in questa equazione del moto una somiglianza con il **moto armonico** considerando $w^{2} = \frac{|q_e|\lambda Rx}{2\epsilon_0(R^{2})^{\frac{3}{2}}}$
Ricordando le caratteristiche del moto armonico, il tempo impiegato per percorrere la distanza sarà uguale a $\frac{T}{4}$ dove $T$ rappresenta un periodo:
$$
\tau = \frac{2\pi}{4w}
$$
## Superficie
Ricordando il risultato ottenuto con l'anello unidimensionale, adesso vogliamo calcolare il campo elettrico generato da un disco pieno.
![[Pasted image 20250308124318.png]]
ricordiamo che $\sigma > 0$ e che $dq = \sigma dS$, possiamo quindi scrivere:
$$
\vec{E}_{tot} = \int_S d\vec{E} = \int_S \frac{1}{4 \pi \epsilon_0} \frac{\sigma dS}{r^{2}}\hat{r}
$$
dove $r$ è la distanza tra il centro del disco e $dS$.

Il problema di questo integrale è che è un integrale di superficie, quindi andrebbero considerate tutte le possibili direzioni dei vettori e svolgere un integrale doppio, per superare questo ostacolo cerchiamo ora di sfruttare la **simmetria** del sistema, infatti $dS$ non deve avere per forza una forma quadrata, bensì possiamo raffigurarla come un anello di spessore $dS$, così che la somma di tutti gli anelli formi il disco:
![[Pasted image 20250308124807.png]]
Ricordiamo ora che il campo prodotto da un anello spinge lungo il suo asse, così abbiamo unificato tutte le direzioni dei diversi campi.

Consideriamo $\rho \in [0 ,R]$ il raggio dei diversi anelli.

Adesso cerchiamo di far comparire $\rho$ all'interno dell'integrale, per fare questo manipoliamo la geometria dell'anello:
Sappiamo che $dS$ è l'area dell'anello con spessore infinitesimo, immaginiamo ora di tagliare l'anello e stenderlo, trasformandolo in un rettangolo di spessore $d\rho$ come in figura:
![[Pasted image 20250308125704.png]]
possiamo calcolare l'area del rettangolo come:
$$
dS = 2 \pi \rho \cdot d\rho \implies dq = \sigma \cdot 2 \pi \rho \cdot d\rho
$$
$$
\begin{gather}
E_{tot} = \int_0^R \frac{1}{4 \pi \epsilon_0} \frac{\sigma 2 \pi \rho \cdot d\rho x}{(x^{2} + \rho^{2})^{\frac{3}{2}}}\hat{r} \\
= \frac{\sigma}{2 \epsilon_0}x \int_0^R \frac{\rho \cdot d\rho}{(x^{2} + \rho^{2})^{\frac{3}{2}}} \\
= \frac{\sigma}{2 \epsilon_0}x \left( -\frac{1}{\sqrt{ x^2 + \rho^{2}}} \Big|_0^R\right) \\
=\frac{\sigma}{2 \epsilon_0} \cdot \left\{ 1 - \frac{x}{\sqrt{ x^{2} + R^{2} }} \right\} \hat{u}
\end{gather}
$$
dove $\hat{u}$ rappresenta un versore nella direzione dell'asse.

Adesso grazie a questo risultato siamo in grado di calcolare il campo generato da un disco a una distanza $x$.

Provo a valutare il campo generato nel caso in cui $R \to \infty$:
$$
\vec{E}_P = \lim_{ R \to \infty } \frac{\sigma}{2 \epsilon_0} \cdot \left\{ 1 - \frac{x}{\sqrt{ x^{2} + R^{2} }} \right\} \hat{u} = \frac{\sigma}{2 \epsilon_0} \hat{n}
$$
Siamo arrivati quindi al risultato che il campo generato da un piano infinito è costante e indipendente dalla posizione in cui ci troviamo.
# Prima legge di Maxwell
## Flusso
Adesso vogliamo cercare una soluzione alternativa per calcolare la sovrapposizione dei campi anche per forme non simmetriche.

Distinguiamo ora le superfici in:
- superfici chiuse (come una sfera): racchiude un volume al suo interno.
- superfici aperte (come un piano)

Inoltre sarà importante il concetto di **flusso**:
$$
\Phi = \vec{E} \cdot\hat{n} \cdot dS
$$
dove $\hat{n}$ rappresenta il versore con direzione normale al piano e verso, nel caso delle superfici chiuse, che va da dentro verso l'esterno.
![[Elettrostatica 2025-03-13 14.43.03.excalidraw|300]]
Possiamo riscrivere il flusso come:
$$
\Phi = E \cdot \cos \theta dS
$$
Possiamo immaginare che il flusso sia la quantità di carica assorbita da un piano immaginario radiale a n.
Quindi, come descrive la formula, se l'angolo compreso tra il campo elettrico e la forza normale è piccolo avremo un flusso maggiore.
### Flusso in una sfera
In una superficie chiusa il flusso sarà:
$$
d \Phi = \vec{E} \cdot \hat{n} \cdot dS
$$
possiamo calcolare quindi il flusso totale andando a sommare l'intera superficie:
$$
\Phi = \oint_S \vec{E} \cdot \hat{n} \cdot dS
$$
Studiamo il caso di una carica $q$ che vive all'interno di una sfera:
![[Elettrostatica 2025-03-13 15.04.53.excalidraw|300]]
Il flusso sarà:
$$
\begin{gather}
 \Phi = \oint_S \vec{E} \cdot \hat{n} \cdot dS \\
= E \oint dS \\
E = \frac{1}{4 \pi \epsilon_0} \frac{q}{R^2}, \: \oint dS = 4\pi R \\
\Phi = \frac{q}{\epsilon_0}
\end{gather}
$$
## Angolo solido
Per andare a dimostrare la prima legge di Maxwell dobbiamo prima introdurre il concetto di angolo solido.

Si definisce angolo solido l'ampiezza di una porzione di  spazio tridimensionale vista da un punto.![[Elettrostatica 2025-03-13 15.23.27.excalidraw]]
L'angolo solido viene rappresentato da $\Omega$, è importante notare che il rapporto tra superficie e distanza rimane costante:
$$
d\Omega = \frac{dS}{r^{2}} = \frac{dS'}{r'^{2}}
$$
e si misura in steradianti.

Possiamo misurare ora l'angolo solido di una sfera:
$$
\begin{gather}
\Omega = \oint d\Omega \\
\oint \frac{dS}{R^2} = \frac{1}{R^{2}} \oint dS = \frac{1}{R^{2}} \cdot 4\pi R^{2} = 4\pi
\end{gather}
$$

## Generalizzazione calcolo del Flusso
Vogliamo ora generalizzare il  risultato ottenuto per la sfera a tutte le superfici chiuse:
$$
d\Phi = \vec{E} \cdot \hat{n} \cdot dS = E \cos\theta dS
$$
il $\cos\theta$ trasforma $dS$ in $dS'$, una superficie sferica associata alla superficie originale.

Così facendo otterremo che $\vec{E}$ ha la stessa direzione di $\hat{n}$ 
![[Elettrostatica 2025-03-13 15.43.27.excalidraw|200]]
Possiamo quindi scrivere che:
$$
\begin{gather}
d \Phi = E r^{2} d \Omega \\
= \frac{1}{4 \pi \epsilon_0} \frac{q}{r^{2}}r^{2} d\Omega \\
= \frac{q}{4\pi \epsilon_0}d\Omega
\end{gather}
$$
possiamo ora somare tutte le $dS$ con un integrale per calcolare il flusso totale:
$$
\begin{gather}
\Phi = \oint \frac{q}{4\pi \epsilon_0}d\Omega \\
= \frac{q}{4\pi \epsilon_0} \oint d \Omega \\
= \frac{q}{4\pi \epsilon_0}4\pi = \frac{q}{\epsilon_0}
\end{gather}
$$
abbiamo così generalizzato quanto detto per una superficie sferica per una generica superficie chiusa con una carica interna alla superficie, e inoltre abbiamo dimostrato che il flusso non dipende dalla distanza.

La specifica richiesta che la carica si trovi all'interno della superficie deriva dal fatto che se fosse esterna il campo attraverserebbe due volte la superficie con stesso modulo ma con verso opposto e si annullerebbe.
## Sovrapposizione di cariche
Nel caso in cui abbia tante cariche all'interno della superficie:
![[Elettrostatica 2025-03-13 16.05.24.excalidraw]]
I campi elettrici delle diverse cariche si sommeranno tra loro vettorialmente:
$$
\begin{gather}
\vec{E}_{tot} = \sum_{i = 0}^{n} \vec{E}_i \\
\Phi = \oint \sum_{i = 0}^{n} \vec{E}_i \hat{n} dS \\
\sum_{i = 0}^{n} \oint \vec{E}_i \hat{n} dS \\
\end{gather}
$$
utilizzando il risultato che abbiamo ottenuto poco fa possiamo dire che:
$$
\begin{gather}
\Phi = \frac{\sum_{i=0}^{n}q_i}{\epsilon_0} = \frac{Q^{int}}{\epsilon_0}
\end{gather}
$$
Nel caso in cui io abbia una distribuzione continua delle cariche avrò:
$$
\begin{gather}
Q = \int dq = \int_V \rho dV \\
\Phi = \frac{1}{\epsilon_0} \int_V \rho dV
\end{gather}
$$
Quest'ultimo risultato è la **Prima legge di Maxwell**.











