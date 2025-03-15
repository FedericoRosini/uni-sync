Python è un linguaggio di programmazione che utilizziamo per scrivere algoritmi da far compiere alla macchina.

# Tipologia di dati
I dati che forniamo al calcolatore possono essere:
- **int**: si usano per rappresentare numeri naturali con e senza segno. *a = 1*
- **float**: si usano per rappresentare i numeri in virgola mobile. *a = 1.3*
- **chr**: si utilizzano per rappresentare i caratteri. *[tabella ASCII di conversione](https://www.ibm.com/docs/it/aix/7.3?topic=adapters-ascii-decimal-hexadecimal-octal-binary-conversion-table)*
- **str**: si usano per rappresentare sequenze di caratteri. a = 'ciao', oppure a = "ciao"
- <mark style="background: #FFB86CA6;">bool</mark>
# Sintassi
```
<non terminale> := <non terminale> terminale
```
<> si usa per indicare un simbolo che può espandersi.
```
<non terminale>:= terminale1 | terminale2
```
| si usa per indicare un'alternativa
```
<non terminale> := [terminale opzionale] terminale |terminale
```
[] si usa per indicare un simbolo opzionale, sia terminale che non.

## Costanti
Una costante denota un valore che non si può modificare durante l'esecuzione del programma:
- 10 = costante intera
- 10.1 = costante float
- 'c' = costante str
## Variabili
Una variabile dà il nome a una locazione di memoria in cui è memorizzato un valore di un certo tipo:
- a = 10 (variabile con valore int)
- a = 10.1 (variabile con valore float)
- a = 'ciao' (variabile con valore str)

per trovare il valore della classe possiamo scrivere
```python
a = 10
type(a)
<class'int'>
```
Le variabili esistono da quando gli viene assegnato un valore per la prima volta.

Se ho una variabile in $int$ e voglio sommarla con un $float$ devo trasformare $int$ in $float$, sommare tra $float$ e poi riconvertire il valore iniziale in $int$.
## Operatori
### Operatori binari
$$
\begin{array}
\\\text{operatore} & \text{funzione} \\ \hline 
+ & \text{somma} \\
- & \text{sottrazione} \\
* & \text{moltiplicazione} \\
/ & \text{divisione} \\
// &  \text{divisione intera} \\
\%  & \text{resto della divisione intera}
\end{array}
$$
### Operatori binari razionali
$$
\begin{array}{c|c}
\\\text{operatore} & \text{funzione} \\ \hline 
< & \text{minore} \\
<= & \text{minore uguale} \\
== & \text{uguale} \\
> & \text{maggiore} \\
>= &  \text{maggiore uguale} \\
!=  & \text{diverso}
\end{array}
$$
Questi operatori rispondono solo con vero o falso.
### Operatori logici binari: and, or
OR:
$$
\begin{array}{c|c|c} 
\text{a}  & \text{b}& \text{a and b} \\ \hline
False  &  False & False \\ 
False  &  True & True \\
True  &  False & True \\
True  &  True & True \\
\end{array}
$$
AND:
$$
\begin{array}{c|c|c} 
\text{a}  & \text{b}& \text{a and b} \\ \hline
False  &  False & False \\ 
False  &  True & False \\
True  &  False & False \\
True  &  True & True \\
\end{array}
$$
