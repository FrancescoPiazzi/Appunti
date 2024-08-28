 # Principio zero
Quando due sistemi termodinamici sono in equilibrio termico condividono alcune proprietà, che possono essere misurate con un valore numerico, la temperatura

Se metti tre cose attaccate assieme tipo così
$$
A|B|C
$$
Dove le "|" sono pareti non ermetiche, e A, B, e C sono alla stessa temperatura. Allora i tre sistemi sono in equilibrio termico (waw).
# Primo principio
Il primo principio della termodinamica identifica il calore come una forma di energia che, come tutte le forme di energia, può essere trasformata in lavoro ed essere immagazzinata.
Questo significa che il calore, originariamente misurato in calorie, ed il lavoro, misurato in Joule, sono equivalenti, una caloria vale circa 4.186 Joule.
Il primo principio quindi parla della conservazione dell'energia: in ogni macchina termica una certa quantità di calore viene trasformata in lavoro, di nuovo, entrambe sono forme di [energia](Lavoro%20e%20calore.md), ed entrambe si misurano in Joule:
$$ \Delta U = Q_{in} - W_{out}$$
+ $\Delta U$ Variazione di energia interna
+ $Q_{in}$ Calore fornito al sistema
+ $W_{out}$ Lavoro effettuato dal sistema (negativo perché il lavoro viene assorbito)
Con variazione di energia interna si intende la somma delle energie cinetiche delle particelle del sistema.

Questa formula ci comunica alcune cose:
+ ***Se un sistema compie una trasformazione da uno stato A ad uno stato B, scambiando calore e lavoro con l'ambiente, Q e W dipendono dalla trasformazione, ma Q-W è indipendente da essa***
+ Esiste una funzione delle coordinate termodinamiche del sistema chiamata **energia interna** U, le cui variazioni dipendono dagli scambi energetici del sistema
+ Dati due stati A e B è fissata $\Delta U$, questo significa che in diverse trasformazioni dallo stato A allo stato B possono scambiare quantità diverse di calore e lavoro, ma la loro differenza sarà sempre la stessa, se U resta costante durante una trasformazione, allora sicuramente si ha che $Q=W$, queste trasformazioni vengono dette **cicliche**
+ Quando si fornisce energia ad un sistema, questa rimane immagazzinata in esso, e può essere interamente riutilizzata (nella realtà non è il caso, per via del secondo principio della termodinamica)

Nel caso di un sistema aperto, il primo principio diventa il seguente
$$ \Delta E  = \Delta U + \Delta E_k + \Delta E_{pot}= Q_{in} - W_{out} $$
+ $\Delta U$ Variazione di energia interna (stessa di prima)
+ $\Delta E_k$ Variazione energia cinetica
+ $\Delta E_{pot}$ Variazione di energia potenziale

Nel caso di un ciclo termodinamico come quello della [[Teorema e macchina di Carnot#Macchina di Carnot|macchina di Carnot]] invece, al termine del ciclo dobbiamo tornare alle condizioni di partenza, quindi si ha che
$$ Q = W$$
# Secondo principio
## Chiacchere
Osservazioni sul mondo reale, che consideriamo veri
+ Clausius: è impossibile realizzare una trasformazione che abbia come unico risultato il trasferimento di calore da un corpo freddo a uno caldo senza usare lavoro esterno ([[Teorema di Clausius|altro]])
+ Kelvin-Planck: è impossibile realizzare una macchina ciclica che converte tutto il calore assorbito da una sorgente omogenea in lavoro
### Kelvin Plank implica Clausius
I primi due punti sono equivalenti, questo perché, assumendo di poter costruire una macchina che violi la formulazione di Kelvin-Plank KP, possiamo costruirne una che violi anche l'enunciato di Clausius:
![Engelbart|600](macchina-impossibile.png)
Il motore KP sta violando il principio di Kelvin Plank, convertendo in lavoro tutto il calore assorbito dalla sorgente T1, senza effetti collaterali, il lavoro di questa macchina viene poi immesso in una macchina di Carnot che funziona al contrario (un frigorifero) F, che sposta calore da una sorgente fredda ad una calda. Avendo spostato calore da una sorgente fredda ad una calda senza aver usato lavoro esterno al sistema, abbiamo costruito una macchina che viola il principio di Clausius
### Clausius implica Kelvin Plank
Consideriamo ora un motore C che viola il principio di Clausius, che quindi in qualche modo sposta calore da un corpo freddo ad uno caldo senza usare lavoro esterno, assumendo che questa macchina sposti una quantità di calore $Q$, possiamo collegare una macchina di Carnot che crea lavoro spostando calore dalla sorgente calda a quella fredda, in modo che la quantità di calore trasferito alla sorgente fredda sia uguale a $Q$, questo sistema sta producendo lavoro dal nulla, che è impossibile

## Trasformazioni reversibili e non
Quando viene compiuta una trasformazione reversibile sull'ambiente, è sempre possibile tornare indietro, ripercorrendo la trasformazione in senso inverso, invertendo quindi quantità di calore e lavoro scambiati.
Questo si estende ai cicli reversibili, nei quali è sempre possibile ripercorrerli al contrario per riportare sia il sistema che l'ambiente nello stato iniziale (il sistema torna allo stato iniziale dopo ogni ciclo, l'ambiente non necessariamente)
In generale potremmo dire che ***Una trasformazione reversibile non comporta alterazioni permanenti***
Questo non vale in presenza di trasformazioni irreversibili, come tutte le trasformazioni nelle quali sono presenti:
+ Forze di attrito
+ Espansioni libere di gas
+ Passaggi di calore tra due corpi a contatto termico 
*(quindi qualunque trasformazione vera)*
![[Teorema e macchina di Carnot#Teorema di Carnot]]

----------

La formulazione più usata nella fisica moderna però si basa sul concetto di entropia:
***In un sistema isolato, l'entropia è una funzione non decrescente nel tempo***
$$\frac{dS}{dt} \ge 0$$
Più precisamente, l'entropia di un sistema rimane invariata quando si esegue una trasformazione reversibile, e aumenta quando si esegue una trasformazione irreversibile.


## Formulazione matematica
Ricordando una conseguenza del teorema di Clausius
![[Teorema di Clausius#^Corollario1DisuguaglianzaClausius]]
$$ \begin{gather*}
dS = \frac{\delta Q_{rev}}{T} \gt\frac{\delta Q_{irr}}{T}  \\
\int^B_A dS = \int^B_A \frac{\delta Q_{rev}}{T} dS \gt \int^B_A \frac{\delta Q_{irr}}{T} dS \\
S = \int^B_A \frac{\delta Q_{rev}}{T} dS \gt \int^B_A \frac{\delta Q_{irr}}{T} dS 
\end{gather*} $$

# Terzo principio
Il terzo principio afferma che è impossibile raggiungere lo zero assoluto con un numero finito di trasformazioni.
Questo principio dà anche una definizione precisa di 0 entropico, ovvero l'entropia che ha un solido cristallino alla temperatura di 0 Kelvin. L'entropia di questo solido è uguale a 0 per via della legge di Boltzmann $S = K ln(1) = 0$ dove l'1 nel logaritmo è il numero di modi diversi di disporre le molecole, dato che stiamo parlando di un cristallo le molecole sono tutte uguali