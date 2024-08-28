# Esperimento di Joule
La legge che lega le [[Variabili termodinamiche|variabili termodinamiche]] all'energia interna di un gas è data dall'esperimento sull'espansione libera di Joule, dove un gas in un contenitore diatermico viene fatto espandere

![[espansione-libera.jpeg]]

Si osserva sperimentalmente che la temperatura del liquido che lo circonda (e quindi quella del gas) non cambia, quindi **nell'espansione libera l'energia interna di un gas non varia**, inoltre, dato che pressione e volume sono invece ovviamente cambiati, questo significa anche che **l'energia interna $U$ di un gas è funzione solamente della sua temperatura**

Per determinare il valore di $U(T)$ consideriamo due generici stati di equilibrio $A$ e $B$, l'energia associata ad essi $U(A)$ e $U(B)$, e $\Delta U = U(B)-U(A)$, $\Delta U$ deve avere lo stesso valore indipendentemente dalla natura della trasformazione $AB$ essendo funzione di stato, scegliendo $AC$ isocora e $CB$ isoterma:
$$\Delta U = U(B) - U(A) = U(B) -U(C) +U(C) -U(A) = U(C)-U(A)$$
Questo vale perché essendo $CB$ isoterma, $U(B)-U(C)=0$ perché $U$ è funzione solamente della temperatura, che non è cambiata
Ricordando la variazione di energia di una trasformazione isocora:
![[Trasformazioni termodinamiche#^caloreIsocore]]
Essendo una trasformazione isocora il gas non compie [[Lavoro|lavoro]], quindi per il [[Principi della termodinamica#Primo principio|primo principio della termodinamica]] abbiamo che $\Delta U = Q_V$, quindi

$$
\Delta U = n\ c_V\ \Delta T
$$
^DeltaEnergiaInternaGas

da cui si ricava
$$
c_V = \frac{1}{n}\frac{dU}{dT}
$$
Questo ci fa anche capire che il calore specifico rappresenta la quantità di Joule da fornire ad una mole di sostanza perché la sua temperatura aumenti di 1 grado Kelvin

Essendo l'energia interna una funzione di stato, **queste formule sono indipendenti dalle trasformazioni eseguite per ricavarle**, quindi valgono qualunque sia la trasformazione

-----------

Nel caso di una trasformazione isobara invece, abbiamo del lavoro $W=p\Delta V$, positivo perché il gas si espande e quindi compie lavoro positivo con l'aumento della temperatura $$ Q_p = n\ c_p\ \Delta T $$ di nuovo ricordando il primo principio $\Delta U = Q_{in} - W_{out}$

$$ \Delta U = n\ c_p\ \Delta T - p\ \Delta dV$$
^DeltaEnergiaInternaGasIsobara

Dato che l'energia interna è funzione solo della temperatura, e la variazione di temperatura è la stessa, $c_p$ deve essere maggiore di $c_V$ per "bilanciare" il $-p\Delta V$, questo significa che **il calore che bisogna cedere a una certa quantità di gas per farlo aumentare di una certa temperatura è maggiore se manteniamo la pressione costante**. L'idea è che se manteniamo la pressione costante parte del calore trasferito finisce in lavoro per far espandere il gas, cosa che non succede se il volume rimane costante.
Se non consideriamo il calore specifico costante, ma funzione della temperatura:
$$\Delta U = Q = n\int_{T_A}^{T_B}{c_V\ dT}$$
# Relazione di Mayer
## Metodo complicato del libro
Sappiamo che $c_p>c_V$, per dare una relazione quantitativa a questi due valori, consideriamo una trasformazione isobara infinitesima $dQ = n\ c_p\ dT$ e $dW = p\ dV$
$$
n\ c_p\ dT=n\ c_V\ dT + p\ dV
$$
Differenziamo la [[Legge dei gas perfetti|legge dei gas perfetti]]
$$\begin{gather*}
pV = n\ R\ T\\
p\ dV + V\ dp = n\ R\ dT
\end{gather*}$$
Questa è una trasformazione isobara quindi $dP=0$, e di conseguenza:
$$p\ dV = n\ R\ dT$$
Ora che possiamo riscrivere $p\ dV$ in termini di $dT$, lo reinseriamo nell'equazione originale
$$\begin{gather*}
n\ c_p\ dT = n\ c_V\ dT + n\ R\ dT \\
c_p = c_V + R
\end{gather*}$$
In conclusione si ottiene

$$R =c_p-c_V$$
^RelazioneDiMayer

Essendo $c_V$ in funzione della temperatura, questo significa che anche $c_p$ lo è, inoltre per salti di temperatura relativamente piccoli o temperature non basse possiamo approssimarlo a costante

## Metodo semplice
Ricordando le variazioni di energia interna di trasformazioni isocore e isobare:
![[Energia interna di un gas#^DeltaEnergiaInternaGas]]
![[Energia interna di un gas#^DeltaEnergiaInternaGasIsobara]]
$$\begin{gather*}
n\ c_V\ dT = n\ c_p\ dT - p\ dV \\
n\ c_p\ dT - n\ c_V\ dT = p\ dV \\
c_p-c_V = \frac{p\ dV}{n\ dT} \\
\end{gather*}$$
Ricordando che $pV=nRT \rightarrow R = \frac{pV}{nT}$, che in forma infinitesimale diventa uguale alla parte destra dell'equazione, quindi $c_p-c_V = R$

# Rapporto Gamma
Il rapporto tra $c_p$ e $c_V$ può anch'esso essere approssimato a costante, e in particolare dipende dal numero di atomi che formano una molecola del gas, questi risultati sono stati ricavati sperimentalmente

|                          | monoatomici    | biatomici      |
| ------------------------ | -------------- | -------------- |
| $c_V$                    | $\frac{3}{2}R$ | $\frac{5}{2}R$ |
| $c_p$                    | $\frac{5}{2}R$ | $\frac{7}{2}R$ |
| $\gamma=\frac{c_p}{c_V}$ | $\frac{5}{3}$  | $\frac{7}{5}$  |
