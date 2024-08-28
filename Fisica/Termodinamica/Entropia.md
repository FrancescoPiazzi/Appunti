Siano A e B due stati qualunque di un sistema termodinamico che passa dallo stato $A$ allo stato $B$ usando trasformazioni reversibili $1$ e $2$, se percorriamo in senso inverso la trasformazione $2$, abbiamo composto un ciclo reversibile, si ha quindi che
$$ \oint\frac{dQ}{T} = 
\int_A^B(\frac{dQ}{T})_1 + \int_B^A(\frac{dQ}{T})_2 =
\int_A^B(\frac{dQ}{T})_1 - \int_A^B(\frac{dQ}{T})_2 = 0 $$
Questo per via della proprietà delle trasformazioni reversibili dove invertire di senso un processo comporta solo l'inversione di senso dei segni di calore e lavoro, questo significa che
$$\int_A^B(\frac{dQ}{T})_1 = \int_A^B(\frac{dQ}{T})_2$$
Il che significa che, fissati il punto iniziale e finale della trasformazione, l'integrale $\int_A^B(\frac{dQ}{T})$ ha sempre lo stesso valore, indipendentemente dalla trasformazione scelta

Definiamo quindi una funzione $S$
$$S_B-S_A=\Delta S=\int_A^B(\frac{dQ}{T})_{rev}$$
Questa funzione di stato è detta **entropia**
L'entropia è una quantità additiva, quindi dati due sistemi, l'entropia complessiva è la somma delle entropie dei sistemi singoli


---------

L'entropia è una funzione di stato che misura il grado di probabilità che un sistema si trovi in un particolare stato.
Una funzione di stato è una funzione la cui variazione non dipende dal percorso seguito, ma solo dagli estremi della trasformazione.
Il fatto che l'entropia sia una funzione di stato significa anche che se in una funzione lo stato iniziale e quello finale coincidono allora la funzione varrà 0, in modo simile a come il lavoro di forze conservative che costituiscono un ciclo chiuso vale 0 ([[Forze conservative e non]])
