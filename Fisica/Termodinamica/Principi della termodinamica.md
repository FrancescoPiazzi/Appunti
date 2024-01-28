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
+ $W_{out}$ Lavoro effettuato dal sistema

Con variazione di energia interna si intende la somma delle energie cinetiche delle particelle del sistema.
Nel caso di un sistema aperto, il primo principio diventa il seguente
$$ \Delta E  = \Delta U + \Delta E_k + \Delta E_{pot}= Q_{in} - W_{out} $$
+ $\Delta U$ Variazione di energia interna (stessa di prima)
+ $\Delta E_k$ Variazione energia cinetica
+ $\Delta E_{pot}$ Variazione di energia potenziale

Nel caso di un ciclo termodinamico invece, al termine del ciclo dobbiamo tornare alle condizioni di partenza, quindi si ha che
$$ Q = W$$
# Secondo principio
## Chiacchere
Il secondo principio è stato formulato più volte in forme diverse:
+ Clausius: è impossibile realizzare una trasformazione che abbia come unico risultato il trasferimento di calore da un corpo freddo ad uno caldo senza usare lavoro esterno
+ Kelvin-Planck: è impossibile realizzare una macchina ciclica che converte in lavoro tutto il calore assorbito da una sorgente omogenea
+ Non si sa chi: è impossibile realizzare una macchina termica con rendimento 1
La più usata nella fisica moderna però si basa sul concetto di entropia:
	$\textit{"In un sistema isolato, l'entropia è una funzione non decrescente nel tempo"}$	$$\frac{dS}{dt} \ge 0$$
Più precisamente, l'entropia di un sistema rimane invariata quando si esegue una trasformazione reversibile, e aumenta quando si esegue una trasformazione irreversibile.

## Formulazione matematica
$$ \begin{gather*}
dS = \frac{\delta Q_{rev}}{T} \gt\frac{\delta Q_{irr}}{T}  \\
\int^B_A dS = \int^B_A \frac{\delta Q_{rev}}{T} dS \gt \int^B_A \frac{\delta Q_{irr}}{T} dS \\
S = \int^B_A \frac{\delta Q_{rev}}{T} dS \gt \int^B_A \frac{\delta Q_{irr}}{T} dS 
\end{gather*} $$

# Terzo principio
Il terzo principio afferma che è impossibile raggiungere lo zero assoluto con un numero finito di trasformazioni.
Questo principio dà anche una definizione precisa di 0 entropico, ovvero l'entropia che ha un solido cristallino alla temperatura di 0 Kelvin. L'entropia di questo solido è uguale a 0 per via della legge di Boltzmann $S = K ln(1) = 0$ dove l'1 nel logaritmo è il numero di modi diversi di disporre le molecole, dato che stiamo parlando di un cristallo le molecole sono tutte uguali