#uni 
Lo scopo della cinematica del punto è quello di descrivere la posizione di un punto materiale in funzione del tempo, ossia determinare le sue **leggi orarie**, analizziamo un caso:
![[posizione punto materiale.png|300]]
In questo caso la posizione di $P$ è data da:
$$P=(x(t), y(t), z(t))$$
Dove $x(t), y(t), z(t)$ sono funzioni che descrivono l'andamento delle componenti cartesiane nel tempo.

Segue che la legge oraria della posizione di P sarà:
$$\vec{r}_P = x(t)\hat{u}_x + y(t)\hat{u}_y + z(t)\hat{u}_z$$
## Traiettoria
La traiettoria è l'insieme delle posizioni in cui passa il punto materiale.

Per definire una traiettoria nello spazio sono necessarie due funzioni $f(x, y, z)$ e $g(x,y ,z)$ le quali andranno a tracciare una curva geometrica.
## Velocità
La velocità è una grandezza vettoriale che misura quanto spazio il punto materiale ha percorso in un determinato intervallo di tempo:
$$\vec{v} = \frac{\Delta \vec{r}}{\Delta t}$$
La velocità istantanea, non è altro che la velocità vista in precedenza ma per un intervallo di tempo infinitesimo:
$$\vec{v}_i = \lim_{\Delta t \to 0}\frac{\Delta \vec{r}}{\Delta t} = \dot{x}$$
## Moto rettilineo uniforme
Il moto rettilineo uniforme è costituito da una traiettoria rettilinea e da velocità costante, le leggi orarie di questo moto sono:
$$
\begin{cases}
\dot{x}(t) = \dot{x}(t_0)\\
x(t) = \dot{x}(t_0)t + x(t_0)
\end{cases}
$$
è possibile risalire alla legge oraria della posizione semplicemente integrando la legge oraria dell'accelerazione, ricordando che:
$$\dot{x}= \frac{dx(t)}{dt}$$
## Accelerazione
L'accelerazione misura quanto varia la velocità del punto materiale in un intervallo di tempo:
$$\vec{a} = \frac{\Delta v}{\Delta t}$$
L'accelerazione istantanea, sfrutta lo stesso principio della velocità istantanea, andando quindi a considerare l'intervallo di tempo $\Delta t \to 0$:
$$\lim_{\Delta t \to 0}\frac{\Delta v}{\Delta t} = \frac{dv}{dt} = \frac{d^2 x}{dt} = \ddot{x}(t)$$
## Moto rettilineo uniformemente accelerato
Il moto rettilineo uniformemente accelerato è costituito da una traiettoria rettilineo e da un'accelerazione costante, le sue leggi orarie sono:
$$
\begin{cases}
\ddot{x}(t)=\ddot{x}(t_0)\\
\dot{x}(t)= \ddot{x}(t_0)t + \dot{x}(t_0)\\
x(t) = \frac{ddot{x}(t_0)}{2}t^2 + \dot{x}(t_0)t + x(t_0)\\
\end{cases}
$$
