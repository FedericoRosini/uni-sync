[[Informatica]] [[Lezione 4 Informatica]]
While è un'[[Iterazioni]] 

- Si usa tipicamente quando non è noto il numero di iterazioni

# Passaggi da eseguire
1. Scegliere la variabile che conta
2. Assegnarle un valore iniziale
3. Definire il test per terminare l'iterazione
4. Scrivere il blocco da eseguire
	1. Modificare la variabile di conteggio
5. Eseguire il codice al termine dell'iterazione

**Esempio:**
```python
error = 0.000001
x = 10000 
z = x #starting value z_0 #1. (z è la variabile che conta) #2. 

while abs(z*z - x) > error: #3.
    z = 0.5 * (z + x/z) #4.
print(z) # 5. 
```
- come valore iniziale possiamo prendere il valore che vogliamo calcolare almeno siamo sicuri che vada bene




