Sappiamo la prima legge termodinamica
$$\Delta U = Q-W$$
e sappiamo che in un ciclo $\Delta U = 0$, quindi il calore è uguale al lavoro

Questa legge ci suggerirebbe che è possibile trasformare una certa quantità di calore interamente in lavoro, tuttavia ciò non è vero, mentre è possibile convertire tutto il lavoro in calore (e.g. con dell'attrito), fare l'opposto ha sempre effetti collaterali. Questo risultato è ricavato da osservazioni sul mondo reale. Ma viene anche da un'altra osservazione

***"Il calore non fluisce mai spontaneamente da un corpo freddo ad uno caldo"***

Questo si traduce negli enunciati di Kelvin Plank e Clausius
***"è impossibile realizzare una macchina ciclica che converte tutto il calore assorbito da una sorgente omogenea in lavoro"***
***"è impossibile realizzare una trasformazione che abbia come unico risultato il trasferimento di calore da un corpo freddo a uno caldo senza usare lavoro esterno"***
(questi sono principi, ovvero frasi che accettiamo vere, quindi non si dimostrano)
(questi due principi sono equivalenti)

Sono equivalenti perché se prendiamo una macchina C che viola il principio di Clausius che in qualche modo raffredda una sorgente fredda a temperatura $T_1$ scaldando una sorgente calda a temperatura $T_2$. Poi prendiamo una macchina termica normale che produce lavoro spostando calore dalla sorgente calda a quella fredda, in modo che il calore ceduto dalla seconda macchina alla sorgente fredda sia uguale a quello che la prima trasferisce dalla sorgente calda a quella fredda. Questo sistema sta producendo lavoro dal nulla che è impossibile

## Teorema di Carnot
Consideriamo una macchina qualsiasi e una macchina reversibile operanti tra due temperature T1 e T2 con $T_1 < T_2$

Sappiamo che nel ciclo di Carnot, quando non siamo a contatto con nessuna sorgente, la trasformazione è adiabatica, tutti gli altri cicli presuppongono il contatto tra più di due sorgenti

### ipotesi 1: $\eta_x>\eta_R$
se R è reversibile, possiamo girarla al contrario, quindi al posto di produrre lavoro W da calore $Q_2'$ come effetto collaterale $Q_1'$, userà lavoro $W$ per raffreddare la sorgente fredda, facendo quindi $Q_1' - Q_2' = -W'$ 

$$\begin{gather*}
\eta_X > \eta_R \\
\frac{W}{Q_2} > \frac{W}{Q_2'} \\
Q_2' > Q_2 \\
\end{gather*}$$
Da questo possiamo costruire una macchina che viola il principio di Clausius (scaldare una sorgente calda usando una fredda)

???

Teorema di Carnot
***"Il rendimento di una macchina reversibile che lavora tra due temperature è maggiore o uguale al rendimento di una qualsiasi macchina che lavora tra le stesse due temperature"***

## Teorema di Clausius
Il teorema di Clausius generalizza il teorema di Carnot:
Partendo da un ciclo qualsiasi, immaginiamo esso sia divisibili in tanti tratti isotermi e adiabatici di varie lunghezze, possiamo portare questo ragionamento al limite per descrivere qualsiasi ciclo come se fosse composto da isoterme e adiabatiche infinitamente piccole, questo divide ogni ciclo in tanti piccoli cicli di Carnot

???

$$\sum_{j=0}^N\frac{Q_j}{T_j} \le 0$$
+ $N$ numero di sorgenti su cui lavora la macchina

Possiamo riscrivere la formula nella sua forma continua, ovvero un integrale su una curva continua
$$\oint \frac{dQ}{T} \le 0$$
nota: per entrambe $=0$ per cicli reversibili, $<0$ altrimenti