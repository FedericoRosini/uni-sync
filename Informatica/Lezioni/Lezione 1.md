 ## Rappresentazione Dati

- abbiamo dei sistemi che memorizzano uno stato (0 , 1)
- Noi somministriamo delle tensioni e lui ne tira fuori altre in base alle istruzioni
- dobbiamo scegliere come **codificare** dati e istruzioni

### Numeri in Binario

in decimale $42 = 4*10 + 2$ 
$$
\sum_{k=0}^{\infty}a_kB_k
$$
se cambio la base:
$[42]_{10}$ le parentesi quadre indicano che è rappresentato in base 10
$$
[42]_{10} = 2^5 + 2^3 + 2^1 = 32 + 8 + 2 = [101010]_2
$$
### Somme
Il riporto si genera quando si arriva a $B-1$ per esempio in base $10$ si cambia a $B=9$ 


### Prodotto

$$
101*10 = 1010 = 2^3 + 2^1 = 8 + 2 = 10
$$

se moltiplico per $[10]_2$ sposto tutto di un bit come nei decimali avviene con $[10]_{10}$

### Formula cambio di base
$$
a_0 +2\sum_{k=0}^{\infty}a_{k+1} 2^k
$$
massimo resto $a_0 = 1$ 

Procedimento:
- prendo il numero, lo divido per 2

$$
\begin{gather}
[125]_{10} = \frac{125}{2} = 62 \text{ con resto 1}  \\
\frac{62}{2} = 31 \text{ con resto } 1  \\
\frac{31}{2} = 15 \text{ con resto } 1  \\
\frac{15}{2} = 7 \text{ con resto } 1  \\
\frac{7}{2} = 3 \text{ con resto } 1  \\
\frac{3}{2} = 1 \text{ con resto } 1  \\
\frac{1}{2} = 0 \text{ con resto }  1 \\
[111110]_2
\end{gather}
$$

$$
\begin{gather}
\frac{47}{2} = 23 /1 \\
\frac{23}{2} = 11 /1 \\ \\
\frac{12}{2} = 5 /1 \\ \\
\frac{6}{2} = 2 /1 \\ \\
\frac{3}{2} = 1 /0 \\ \\
\frac{1}{2} = 0 /1 \\ \\
  [111011]_1 \\
\end{gather}
$$

- se il numero è dispari finisce sicuramente per 1
- **ricordare di leggere dal basso verso l'alto** 
$$
\begin{gather}
[1101]_2 \\
1*2^0 + 0*2^1 + 1*2^2 + 1*2^3 = 1 + 4 + 8 = 13
\end{gather}
$$
### Tabelle di verità
**XOR** (somma)
$$
\begin{matrix}
0 & 0 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1 \\
1  & 1 & 0
\end{matrix}
$$
**OR**
$$
\begin{matrix}
0 & 0 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1 \\
1  & 1 & 1
\end{matrix}
$$
**END**
$$

\begin{matrix}
0 & 0 & 0 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
1  & 1 & 1
\end{matrix}
$$
# Interi con segno

per rappresentare il segno posso:
- usare un bit per rappresentare il segno

scomodo


Complemento a 2
se il primo numero è 1 l'intero è negativo, mentre se è 0 è positivo
$$
110 \text{ negativo}
$$
$$
\begin{matrix}
100 = -4 \\
101 =-3 \\
110 = -2 \\
111= -1 \\
000 =0 \\
001 = 1 \\
\dots
\end{matrix}
$$
ho interi positivi con un bit in meno


Come trovare il numero negativo:
1. invertire tutti i bit
2. aggiungere 1

$$

\begin{gather}
[23]_{10} = [010111]_2 \\
[101000]_2 + 000001 \\
[101001]_2 = [-23]_{10}
\end{gather}
$$
## overflow
quando i numeri vanno fuori scala e non entrano nei bit (non succede in python perchè ha un interprete)


# Numeri con virgola 
Un numero si divide in 
- mantissa 23 bit
- esponente 8bit
- segno 1 bit


non possiamo avere numeri dopo la virgola maggiori dei numeri prima:

$$
\begin{gather}
0.625 * 2 = 1.250 = a_1\\

\end{gather}
$$


















