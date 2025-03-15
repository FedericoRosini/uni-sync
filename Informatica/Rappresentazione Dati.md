[[Lezione 1]] [[Informatica]]
Noi vogliamo rappresentare i dati in forma binaria perché siamo in grado di costruire dei dispositivi, i transistor, che sono in grado di "ricordare il proprio stato", però può essere solo:
- acceso (1)
- spento (0)
Dobbiamo quindi codificare le informazioni che conosciamo e che vogliamo che il calcolatore elabori in **codice binario**.

# Codice Binario
Per capire il codice binario, analizziamo prima il codice decimale a cui siamo abituati:
$$
[42]_{10} = 4*10 + 2
$$
La posizione delle cifre indica quindi il suo ordine di grandezza.

Un numero $n$ si scrive quindi come:
$$
n = \sum_{k=0}^{\infty}a_kB_k
$$
dove $B_k$ rappresenta la base in cui vogliamo esprimere il valore, mentre $a_k$ indica la cifra che moltiplica la base, mentre $a_k$ è il coefficiente che moltiplica la potenza e, $a_k \in [0, B-1]$.

Osservazione:
- nel codice binario $a_k$ può essere '0' oppure '1'.

Proviamo ora a scrivere $[42]_{10}$ in base 2:
$$
42 = 1*2^5 + 0*2^4 + 1*2^3 + 0*2^2+ 1*2^1 + 0*2^0
$$
Possiamo quindi scrivere:
$$
[42]_{10} = [101010]_2
$$




<mark style="background: #FFB86CA6;">Possiamo rappresentare i numeri lunghi in esadecimale organizzando i bit a gruppi di 4, la somma dei 4 bit sarà il valore da dare alla rispettiva potenza di 16</mark>
## Operazioni
### Somme
Le somme tra numeri in codice binario si fanno nello stesso del codice decimale, con l'unico accorgimento che i riporti ci sono per $B-1$ quindi nel caso dei decimali, per cifre $>9$, mentre nel caso del codice binario per cifre $>1$ , quindi:
$$
1 + 1 = 10
$$
### Prodotto
Per fare i prodotti in base 2 si eseguono semplicemente i prodotti in colonna come nella base decimale, per esempio:
$$
\begin{gather}
101 \cdot 10 =  \\
101 \cdot 0 = 000 \\
101 \cdot 1 = 101 \\
\end{gather}
$$
$$
\begin{align}
00 & 0  + \\
101 & /  = \\ \hline
1010
\end{align}
$$
Osservazione:
- moltiplicare per 2 (10) trasla di un bit il valore.
## Formula di Cambio Base
L'algoritmo per il cambio base è:
$$
a_0 + 2\sum_{k=0}^{\infty}a_{k+1}2^k
$$
*Nel codice binario, per generalizzare la formula è sufficiente scambiare i '2' nella formula con 'B' generica* 

Questo algoritmo, che prende il nome di "regola dei resti successivi" consiste nel dividere la cifra per il valore della base fino a quando non otteniamo uno $0$, tenendo conto dei resti, alla fine delle divisioni dobbiamo scrivere **partendo dall'ultima divisione fino alla prima** i resti delle divisioni, ed otterremo il numero scritto in codice binario.

Facciamo un esempio pratico di questo algoritmo:
$$
\begin{gather}
[125]_{10} : \\
\frac{125}{2} = 62 \text{ con resto 1}  \\
\frac{62}{2} = 31 \text{ con resto } 1  \\
\frac{31}{2} = 15 \text{ con resto } 1  \\
\frac{15}{2} = 7 \text{ con resto } 1  \\
\frac{7}{2} = 3 \text{ con resto } 1  \\
\frac{3}{2} = 1 \text{ con resto } 1  \\
\frac{1}{2} = 0 \text{ con resto }  1 \\
[111110]_2
\end{gather}
$$
Osservazione:
- se il numero è dispari finisce sicuramente pre 1
## Rappresentazione Interi senza Segno
Possiamo, dato un numero limitato $N$ di bit rappresentare $2^{N-1}$ valori:
$$
\sum_{k=0}^{N-1}a_k{2}^k
$$
Osservazione:
- con 8 bit (1 byte) posso rappresentare interi da 0 a 255.
## Rappresentazione Interi con Segno
Per rappresentare i numeri negativi si utilizza il **complemento a 2**. Una rappresentazione secondo la quale il bit più significativo (quello più a sinistra che rappresenta la potenza massima di 2) è un termine negativo.
Definizione:
Il complemento a $B$ per un numero $r$ a $N$ cifre è dato da $[v]_{CA_{2}} = B^N -r$ 
$$
-a_{N-1}2^{N-1}+\sum_{k=0}^{N-2}a_k 2^k
$$
Il primo numero è negativo, mentre tutti gli altri sono positivi.

Osservazione:
- se il primo numero è '1' $\implies$ il numero è negativo
$$
\begin{matrix}
CA2  & [x]_{10} \\ \hline
100  & -4 \\
101  & -3 \\
110 & -2 \\
111  & -1 \\
000 & 0 \\
001 & 1 \\
010 & 2 \\
011 & 3
\end{matrix}
$$
### Algoritmo di Conversione
L'algoritmo di conversione da un numero positivo a uno negativo è il seguente:
1. invertire tutti i bit (dove ci sono 0 metto 1 e viceversa)
2. sommo 1

Vediamo un esempio pratico:
$$
\begin{gather}
[23]_{10} = [010111]_2 \\
[101000]_2 + 000001 \\
[101001]_2 = [-23]_{10} \\
\end{gather}
$$
## Numeri con la Virgola mobile
Per rappresentare i numeri con la virgola l'idea è di rappresentare i numeri nella seguente forma:
$$
(segno) \times mantissa\cdot B^c
$$
prendendo in esempio una rappresentazione a 32 bit, avremo quindi il primo bit dedicato al segno, i seguenti 8 dedicati all'esponente e gli ultimi 23 alla mantissa:
$$
\begin{array}{c|c|c}
s & e & m \\ \hline
1 & \quad8\quad  & \qquad 23\qquad
\end{array}
$$
Segno:
- 0 $\implies$ positivi
- 1 $\implies$ negativi

Mantissa:
rappresenta il valore del numero, viene scritta sempre in forma **normalizzata**, per esempio:
$$
1011 = 1,011 \cdot 2^3
$$

La mantissa deve rispettare il vincolo $1 \leq m <B$

Per rappresentare i numeri frazionari usiamo un esponente negativo.

Esponente:
l'esponente si rappresenta codificandolo in 8 bit, aggiungendo un *bias* di $(B^{N-1}-1)$, con $B$ base e $N$ numero di bit dedicati all'esponente, la formula dell'esponente diventa quindi:
$$
e = c + (2^7 -1)
$$
con $c$, l'esponente che abbiamo usato per normalizzare la mantissa, concludendo l'esempio di prima avevamo che $c=3$, quindi:
$$
e=3+(128-1)
$$
**In sintesi:**
$$
(-1)^s \cdot 1.m \cdot 2^{e-127}
$$
I numeri in virgola mobile non rappresentano tutti i numeri razionali, per esempio:
$$
[0.1]_{10} = 0.\overline{00011}
$$
è quindi un numero periodico, non rappresentabile con il codice binario.

**Il codice binario é più preciso con i numeri piccoli**
![[Pasted image 20250228090744.png|600]]
Infatti nelle reti neurali si comprimono in dati tra $-1<n<1$ così da avere una maggior precisione.
![[Rappresentazione Dati 2025-02-28 09.16.36.excalidraw]]










