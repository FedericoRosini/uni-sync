[[Informatica]] [[Iterazioni]] [[Lezione 4 Informatica]]

Voglio sapere se in una sequenza di numeri almeno uno deve essere negativo

**devo guardarli uno ad uno**
quando pensiamo questo usiamo il **for**

Il for si usa per le **liste chiuse** mentre il [[While]] per le liste aperte.

Esempio:
```python
valori = [18, 22, 29, 30]
media = 0

for v in valori:
    media =  media + v
    
media/=len(valori) # \= è un operatore che vuol dire: media = media / len(valori)
print(f'media: {media}')
```
[[Len]] 

```python
valori = [20, 10, 30, 78]
somma = 0
c = 0

print(f'c \tsomma\tN') #intestazione tabella
while c<len(valori):
    somma = somma + valori[c]
    print(f'{c}\t{somma}\t{len(valori)}') #tabella
    c = c + 1
   
media = somma / len(valori)

print(media)

```
[[Tabella in Python]]




