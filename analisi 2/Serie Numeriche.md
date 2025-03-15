![[Serie Numeriche 2025-03-02 14.16.59.excalidraw]]
**Definizione**:
Una serie numerica è la somma formale degli elementi di una successione numerica $a_k$:
$$
s_n = \sum_{k=0}^\infty a_k = a_0 + a_1 + a_2 + \cdots + a_n, \quad n \in \mathbb{N}
$$
$a_k$ prende il nome di **termine** della serie

**Serie ridotte:** sono dette serie ridotte, delle serie "parziali", in cui la somma non avviene all'infinito:
$$
s_n = \sum_{k=0}^{n}
$$
**Carattere della serie:** Il carattere della serie (la convergenza o divergenza di questa) dipende dall'andamento della successione $s_n$.
- Se $s_n$ per $n \to \infty$ tende a un numero finito, si dice che la serie è \textbf{convergente}
- Se $s_n$ per $n \to \infty$ tende a $\pm \infty$, si dice che la serie è \textbf{divergente}
- Se $\not \exists \lim_{n \to \infty} s_n$, si dice che la serie è \textbf{irregolare}
## Serie Geometrica
**Definizione:**
Dato un generico $x \in \mathbb{R}$ si dice serie geometrica di ragione $x$ la serie:
$$
\sum_{k=0}^{\infty} x^k = 1 + x + x^2 + \cdots
$$
**Carattere della Serie Geometrica:**
- **convergente** e $\sum_{k=0}^{\infty} x^k = \frac{1}{1 - x}$ se $-1 < x < 1$;
- **divergente** a $\infty$ se $x \geq 1$
- **irregolare** se $x \leq -1$
![[Serie Numeriche 2025-03-01 12.31.48.excalidraw]]
# Serie di Potenze
Data $(\alpha_k)_{k \in \mathbb{N}}$, una serie di potenze di centro $x_0$ è una funzione:

$$
x \longrightarrow \sum_{k=0}^{\infty} \alpha_k (x-x_0)^k = \alpha_0 + \alpha_1 (x-x_0) + \alpha_2 (x-x_0)^2 + \cdots
$$
Dove $(x-x_0)$ può convergere o meno.

La funzione è quindi un polinomio con termini infiniti.

Il nostro intento è trovare per quali valori di $x$ la serie numerica converge, vogliamo trovare quindi l'**insieme di convergenza**.
**Osservazione:**
-  $\alpha_k$ può essere $\geq 0 $ o $<0$
- $(x-x_0)$ può essere $\geq 0 $ o $<0$, se $x=x_0 \implies \sum \alpha_k = \alpha_0 \implies$ \textbf{la serie converge sempre nel suo centro.}

Per rendere vero il secondo punto $\forall \mathbb{R}$ si usa la convenzione che $0^0 = 1$
### Convergenza Assoluta
**Definizione:**
Data $\sum_{k=0}^{\infty} a_k$, converge assolutamente se $\sum_{k=0}^{\infty} |a_k| < +\infty$

**N.B. la convergenza assoluta è SUFFICIENTE ma NON NECESSARIA per la convergenza semplice:**
$$

\begin{gathered}

\sum_{k=0}^{\infty} |\alpha_k| \text{converge} \Rightarrow \sum_{k=0}^{\infty} \alpha_k \text{converge} \\

\sum_{k=0}^{\infty} \alpha_k \text{converge} \not\Rightarrow \sum_{k=0}^{\infty} |\alpha_k| \text{converge} \\

\end{gathered}

$$

Per esempio $\sum_{k=0}^{\infty} \frac{(-1)}{k}$ non converge assolutamente ma converge semplicemente.

### Intervallo di Convergenza
Nelle serie di potenze, l'insieme di convergenza è un \textbf{intervallo simmetrico rispetto al centro di serie}.

*Consideriamo da ora in poi $x_0 = 0$ per semplicità, ma nel caso in cui $x_0 \neq 0, \: (x-x_0) = y$ e consideriamo $\alpha_k y^k$ quello che succede è quindi una semplice traslazione della funzione.*

In una serie di potenze:
Se $\sum_{k=0}^{\infty} \alpha_k x^k$ converge per $x = \xi \implies \text{coverge almeno} \: \forall x \leq |\xi|$
**Intervalli di Convergenza:**
- $(-R,R)$: converge almeno per $x \in (-R , R)$ e può non convergere per $x \in [-R , R]$
- - $(-\infty , +\infty)$: convergente $\forall x \in \mathbb{R}$, per convenzione si dice che $R = \infty$ \\
- ${0}$: convergente solo nel centro di convergenza
$R$ rappresenta il \**raggio di convergenza**, per $x = R$ dobbiamo verificare la convergenza caso per caso.
**Esempi di Serie di funzioni che si riconducono a serie di potenze:}**
$$

\sum_{k=0}^{\infty} e^{kx}

$$
Fissato $x$ è una serie geometrica di ragione $e^{kx}$ e converge per:

$$

|e^x < 1 \implies x<0|

$$
Intervallo non simmetrico $(/\infty , 0)$

$$

\sum_{k=0}^{\infty}

$$
Converge per $|cosx| < 1 \implies \forall x \not {n\pi}$, quindi in infiniti intervalli periodici (non è un intervallo).
## Criterio della radice
Se $\exists M>0 : |\alpha_k | \leq M^k \implies |\alpha_k x^k|\leq|Mx|^k$ converge se $|Mx|^k < 1, \: |x|< \frac{1}{M}$.

Da ciò deriva il teorema:
Se $\exists \lim_{k \to \infty} \sqrt[k]{\alpha_k}$ allora:
$$

R = \frac{1}{\lim_{k \to \infty} \sqrt[k]{\alpha_k}}

$$
Si scrive per convenzione: $\frac{1}{\infty} = 0$ e $\frac{1}{0} = \infty$
## Criterio del rapporto
Sia $\alpha_k > 0 \; \forall k$ , se $\exists \lim_{k \to \infty} \frac{\alpha_{k+1}}{\alpha_k}$, allora $\exists \lim_{k \to \infty} \sqrt[k]{\alpha_k}$ e sono uguali:
$$
R = \frac{1}{\lim\limits_{ k \to \infty } \frac{\alpha_{k+1}}{\alpha_{k}}}
$$
**Esempio 1:**
$$
s_{n} = \sum_{k=0}^{\infty} \alpha_k
$$
Usiamo il criterio del rapporto:
$$
\begin{gather}
\alpha_{k} = \frac{1}{k^2} \\
R = \lim\limits_{ k \to \infty } \frac{k^2}{(k +1)^2} \to 1  \\
R = 1 \\
\end{gather}
$$
La serie converge **almeno** per $x \in (-1 , 1)$; applichiamo ora il criterio del confronto:
$\sum_{k=0}^{\infty}\frac{1}{k^2}$ converge $\forall k \in \mathbb{N}$, $x^k$ converge $\iff |x| \leq 1$ *(per serie goemetrica)*. 

Unendo le soluzioni otteniamo che $x \in [-1,1]$.
**Esempio 2:**
$$
s_{n} = \sum_{k=0}^{\infty} \frac{x^k}{k}
$$
converge in $[-1 ,1)$:

$\alpha_{k} = \frac{1}{k}$, per il criterio del rapporto:
$$
\frac{k}{k+1}\to 1 \implies R=1
$$
La serie converge almeno per $x \in (-1 ,1)$

Adesso controllo gli estremi:
$$
\begin{gather}
x=1 \to \sum_{k=0}^{\infty} \frac{1}{k} = \infty \implies \text{diverge} \\
x=-1 \to \sum_{k=0}^{\infty} \frac{(-1)^k}{k} \implies\text{segni alterni}
\end{gather}
$$
## Criterio di Leibniz
**Teorema**
Sia $\sum_{k=0}^{\infty}(-1)^ka_k$ una serie numerica;
Se:
- $a_k \geq 0$;
- $a_k \geq a_{k+1} \; \forall k$
- $a_k \to 0$
Allora $\sum_{k=0}^{\infty}(-1)^ka_k$ converge.

Esempio
$$
\sum_{k=0}^{\infty} \frac{(-1)^k}{k}
$$
- $a_k = \frac{1}{k}>0$;
- $a_k > a_{k+1}$
- $a_k \to 0$
Questo implica che la serie converge.
## Serie di funzioni
Consideriamo una serie di funzioni:
$$
\sum_{k=0}^{\infty}f_{k}(x)
$$
con $f_{x}:I \subseteq \mathbb{R} \to \mathbb{R}$ , un esempio di serie di funzione è proprio la serie potenziale.
### Convergenza Puntuale 
Si definisce convergenza puntuale se $\forall x \in I \: \exists f_{k}(x) = f(x)$ dove $I$ rappresenta il nostro insieme di convergenza.
**Osservazione:**
$f(x)$ può non essere continua anche se le funzioni $f_{k}(x)$ sono continue,
**Esempio:**
$$
f(x) = \sum_{k=0}^{\infty}(1-x) x^k  = (1 - x) \sum_{k=0}^{\infty} x^k
$$La serie sarà:
- $1$ se $|x|<1$;
- $0$ se $|x|\geq 1$ 
possiamo notare come nonostante $x^k$ sia continua, $f(x)$ non lo sia.
### Convergenza Totale
**Definizione:**
$\sum_{k=0}^{\infty}f(x)$ converge **totalmente** in $I$ se $\exists c_{k} \geq 0: \: |f_{k}(x)|\leq c_{k} \: \forall x \in I, \: \forall k$ e $c_{k}$ converge.

Osservazione:
il $\leq$ si dice **uniforme in $x$** in quanto $c_{k}$ non dipende da $x$

**Teorema:**
Supponiamo che $\sum_{k=0}^{\infty}f_{k}(x)$ converga totalmente in $I$, allora:
1) $\sum_{k=0}^{\infty}f_{k}(x)$ converge anche puntualmente;
2) Se $f_{k}(x)$ sono continue $\implies f(x)$ è continua.
**Dimostrazione:**
1) Fissato $x \in I$, vogliamo vedere che la serie numerica $\sum_{k=0}^{\infty}$ converge:

Si ha che $|f_k(x)|\leq c_k$ con $\sum_{k=0}^{\infty} c_k < \infty$, quindi per confronto:
$$
\sum_{k=0}^{\infty}f-k(x) \;\text{converge assolutamente}
$$
Sia $f(x) = \sum_{k=0}^{\infty}f_k(x)$ si avrà che $\forall x \; |f(x)|\leq \sum_{k=0}^{\infty}c_k =M$.
Essendo $\sum_{k=0}^{\infty}c_k$ indipendente da $x \implies f(x)$ è limitata.

2) vogliamo dimostrare adesso che $f(x)$ è continua se $f_k(x)$ sono continue:

Vogliamo vedere quindi che $\forall x \in I, \forall \epsilon>0, \; \exists \delta>0 : |x-x_0<\delta \implies|f(x)-f(x_0)|<\epsilon$
$$
\begin{gather}
|f(x) - f(x_0)|= \left|\sum_{k=0}^{\infty}f_k(x) - \sum_{k=0}^{\infty}f_k(x_0)\right| \\
= \sum_{k=0}^{\infty}f_k(x) - \sum_{k=0}^{m}f_k(x) \\
+\sum_{k=0}^{m}f_k(x) - \sum_{k=0}^{m}f_k(x_0) \\
+\sum_{k=0}^{m}f_k(x_0) - \sum_{k=0}^{\infty}f_k(x_0)
\end{gather}
$$
Si ha che
$$
\sum_{k=0}^{\infty}f_k(x) - \sum_{k=0}^{m}f_k(x_) = \sum_{k=m+1}^{\infty}f_k(x)
$$
e che:
$$
\sum_{k=m+1}^{\infty}|f_k(x)| \leq \sum_{k=m+1}^{\infty}c_k \to 0 \text{  per } m \to \infty
$$
!!! negli appunti è scritto che questo è il resto di una serie convergente, cosa si intende?

Quindi $\forall x \in I$ (anche $x_{0}$) in corrispondenza di $\frac{\epsilon}{3}>0, \; \exists \;\overline{m}$ tale che: 
$$
\left|\sum_{k=0}^{\infty}f_k(x) - \sum_{k=0}^{m}f_k(x)\right|< \frac{\epsilon}{3}, \; \forall m \geq \overline{m} 
$$
Osservazione:
- $\overline{m}$ dipende da $\epsilon$ ma non da $x$

Per dimostrare la seconda riga uso la differenza di continuità.

Per l'indice $\bar{m}$ trovato ora  uso la definizione di continuità$\sum_{k=0}^{\bar{m}}f_k(x) - \sum_{k=0}^{\bar{m}}f_k(x_0)$ è continua, quindi in corrispondenza di $\frac{2E}{3} > 0, \; \exists \delta >0$:
$$
|x-x_0|< \delta \implies \left|\sum_{k=0}^{\bar{m}}f_k(x) - \sum_{k=0}^{\bar{m}}f_k(x_0)\right|< \frac{\epsilon}{3}
$$
avremo quindi che:
$$
|f(x) - f(x_0)| \leq \frac{\epsilon}{3} + \frac{\epsilon}{3} + \frac{\epsilon}{3} = \epsilon \implies f \text{ è continua}
$$
**Esempio:**
$\sum_{k=0}^{\infty}a_{k}x^k$ serie di potenze, $f_{k}(x) = a_{k}x^k$, essendo una serie di potenze, questa converge assolutamente in un intervallo $(-R , R)$; 

Sia $\xi \in (0,R)$, allora $\sum_{k=0}^{\infty} |a_{k}|\xi \leq \infty$ 
Se $|x| \leq \xi \implies \sum_{k=0}^{\infty}|a_{k} x^k| \leq \sum_{k=0}^{\infty} |a_{k}\xi^k|$ con $\leq$ uniforme in $\xi$; 
$|f_{k}(x)| \leq a_{k}\xi^k \implies$ le **potenze convergono totalmente** negli intervalli $(-\xi , \xi)$.
*In generale non convergono totalmente in $(-R , R)$, dipende se gli estremi sono inclusi o meno, per esempio $\sum_{k=0}^{\infty}x^k$ non converge totalmente in $(-1 ,1)$.* 
**Teorema:**
Sia $f(x) = \sum_{k=0}^{\infty}a_{k}(x - x_{0})^k$, con $x \in (x_{0} - R, x_{0} +R)$, con $R$ raggio di convergenza, allora **$f(x)$ è derivabile** e:
$$
f'(x) = \sum_{k=0}^{\infty}ka_{k}(x -x_{0})^{k-1}; \quad \text{per} \: x \in (x_{0} - R, x_{0} +R)
$$
Osservazione:
**La serie derivata ha lo stesso raggio di convergenza**. 

**Dimostrazione:**
Sia $f(x) =\sum_{k=0}^{\infty}a_{k}x^k$ e $g(x) = \sum_{k=1}^{\infty} ka_{k}x^{k-1}$ per $x \in (-R , R)$.

Vogliamo dimostrare che $f'(x) = g(x)$:

Si ha che $\frac{d}{dx}\sum_{k=0}^{m}a_{k}x^k = \sum_{k=1}^{m}ka_{k}x^{k-1}$ , possiamo definire per il teorema del calcolo integrale che:
$$
\begin{gather}
\sum_{k=0}^{m}a_{k}x^k - a_{0} = \int_{0}^x \sum_{k=1}^{m}ka_{k}t^{k-1}dt \\
= \left|\int_{0}^x \sum_{k=1}^{\infty}ka_{k}t^{k-1} - \sum_{k=1}^{m}ka_{k}t^{k-1}dt\right|  \\
=\left|\int_{0}^x \sum_{k=m+1}^{\infty}ka_{k}t^{k-1}dt\right| \leq c_{m} \to 0
\end{gather}
$$
## Serie di Taylor
Data $\sum_{k=0}^{\infty}a_{k}(x -x_{0})^k$ con raggio di convergenza $R>0$ in $(x_{0} - R, x_{0}+R)$ definiamo $f(x) = \sum_{k=0}^{\infty}a_{k}(x-x_{0})^k$; 

Allora la funzione $f(x)$ è:
- continua
- derivabile
- è $C^\infty$
- ha derivate continue
Abbiamo già visto in precedenza che $f(x_{0}) = a_{0}$, adesso calcoliamo:
$$
f'(x_{0}) = \sum_{k=1}^{\infty} ka_k(x-x_{0})^{k-1} \to f'(x_0) = a_1
$$
$$
\implies a_k = \frac{f^{k}(x_0)}{k!} \implies f(x) = \sum_{k=0}^{\infty} \frac{f^{k}(x_0)}{k!}(x-x_0)^k
$$
Se calcolo le serie ridotte con la precisione dettata da $k$.

Viceversa, data $f \in C^\infty(I), \: I \subseteq \mathbb{R}$ non è garantito che $f(x)$ sia **sviluppabile** in serie Taylor.
Si considera una serie sviluppabile se:
$$
f(x) = \frac{\sum_{k=0}^{\infty}f^{(k)}(x_)}{k!}(x-x_0)^k
$$
Esempio di una funzione non sviluppabile:
$$
f(x) = \begin{cases}
e^{ - \frac{1}{x^{2}}} \; &\text{se }x \neq 0 \\
0 \; &\text{se }x = 0
\end{cases}
$$
In questo caso la funzione è continua perché $\lim\limits_{ x \to 0 }f(x) = 0$, però la funzione non è sviluppabile secondo la serie Taylor perché $f^{(k)}(0)=0,$ perciò la serie Taylor centrata in $x_0$ sarà nulla.

Per vedere se $f(x)$ è sviluppabile occorre stimare il resto della serie:
$$
f(x) = \sum_{k=0}^{m} \frac{f^{(k)}(x_0)}{k!}(x-x_0)^k + R_m(x)
$$
Dove $R_m(x)$ rappresenta il resto della serie in forma di Lagrange
$$
R_m(x) = \frac{f^{(m+1)}(\xi)}{(m+1)!}(x-x_0)^{m+1}
$$
con $\xi \in (x_0,x)$;

Esempio:
Sia $|f^{(m+1)}(\xi)\leq M|; \forall \xi \in I \;\forall m$,
*quindi la derivata è limitata dalla stessa costante*
Allora:
$$
|R_m(x)| \leq \frac{M}{(m+1)!}(x-x_0)^{m+1} \to 0 \; \text{per } m\to \infty
$$
quindi $f(x)$ è sviluppabile.

























