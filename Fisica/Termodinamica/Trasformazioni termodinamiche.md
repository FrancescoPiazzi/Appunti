# Lavoro delle trasformazioni termodinamiche
Ricordando che il lavoro di un corpo che si muove lungo una traiettoria $\gamma$ vale ![[Lavoro#^Lavoro]]
E ricordando che una pressione è una forza su una superficie, se la superficie è costante pressione e forza sono proporzionali. Se mettiamo il gas in un cilindro, anche spostamento e volume sono proporzionali.
Quindi possiamo veder il lavoro di una trasformazione termodinamica in modo simile a come vediamo il lavoro meccanico
$$ W =\int_{V_A}^{V_B} P \ dv$$ ^LavoroTrasformazioniTermodinamiche
# Entropia delle trasformazioni termodinamiche
$$\Delta S= \int_A^B \frac{\delta Q}{T} = \int_A^B \frac{1}{T} \ \delta Q$$
# Trasformazioni isobare
Dall'equazione di stato si ha che in un'isobara
$$\frac{V_A}{T_A} = \frac{V_B}{T_B} \Rightarrow \frac{V_A}{V_B} = \frac{T_A}{T_B}$$
Il gas può scambiare sia calore che lavoro
$$
Q = nc_p(T_B-T_A)
$$

In un'isobara la pressione è costante, quindi abbiamo che il lavoro vale
$$ 
W =\int_{V_A}^{V_B} p\ dv = 
pV \bigg\rvert_{V_A}^{V_B} = 
p(V_B - V_A) = 
p(\frac{nRT_B}{p} - \frac{nRT_A}{p}) = 
nR(T_B-T_A)
$$
Il calore assorbito per passare da uno stato A ad uno stato B
$$ Q_{A\rightarrow B} = n \ c_p \ \Delta T$$
+ $n$ numero moli
+ $c_p$ calore specifico di quel gas a pressione costante
# Trasformazioni isocore
In un'isocora è il volume ad essere costante, essendo gli estremi di integrazione uguali, il lavoro sarà 0
$$ W =\int_{V_A}^{V_A} P \ dv = 0$$
Il calore assorbito per passare da uno stato A ad uno stato B è molto simile a quello delle isocore:

$$ Q_{A\rightarrow B} = n \ c_v \ \Delta T$$
^caloreIsocore
+ $n$ numero moli
+ $c_v$ calore specifico di quel gas a volume costante
# Trasformazioni isoterme
In un'isoterma si ha che
$$dT=0\ \rightarrow \ nc_VdT=0 \ \rightarrow \ dU=0\ \rightarrow \ Q=W$$
Per quanto riguarda il lavoro, nelle isoterme cambiano sia $p$ che $V$ quindi è un casino, dobbiamo riscrivere P come $\frac{nrt}{V}$ usando la [[Legge dei gas perfetti |legge dei gas perfetti]]
$$ Q=W =\int_{V_A}^{V_B} p \ dV = 
\int_{V_A}^{V_B} \frac{nrT}{V} dV = 
nrT \ \bigg\rvert ln(V)\bigg\rvert_{V_A}^{V_B} = 
nrT \ ln(\frac{V_B}{V_A})$$
Essendo la temperatura costante, $1/T$ è costante, quindi la variazione di entropia vale:
$$ \Delta S = \int_A^B \frac{1}{T} \ \delta Q = \frac{Q}{T} $$
# Trasformazioni adiabatiche
Nelle trasformazioni adiabatiche possiamo sfruttare il fatto che, essendo il calore zero, si ha che $\Delta U = -W$
ricordando [[Trasformazioni termodinamiche#^LavoroTrasformazioniTermodinamiche|il lavoro di una trasformazione termodinamica generica]] possiamo scrivere
$$\begin{gather*}
-W = nc_V(T_B-T_A) \\
W = nc_V(T_A-T_B)
\end{gather*}$$
Questo significa che quando il gas esegue un'espansione adiabatica e quindi fa lavoro sull'esterno, quindi $W>0$, la sua temperatura diminuisce, mentre se lo riceve la sua temperatura aumenta
## Trasformazioni adiabatiche reversibili
*Le trasformazioni adiabatiche reversibili sono un caso limite, in quanto per essere reversibile la trasformazione deve avvenire lentamente, ma questo rende le pareti adiabatiche del contenitore non totalmente adiabatiche*

L'espressione infinitesima del primo [[Principi della termodinamica#Primo principio|primo principio della termodinamica]] è:
$$dQ = dU + dW = nc_VdT+pdV=0$$
Essendo la trasformazione reversibile, possiamo esprimere il lavoro in funzione delle coordinate termodinamiche, e poi usare la [[Energia interna di un gas#^RelazioneDiMayer|relazione di Mayer]]
$$\begin{gather*}
n\ c_V\ dT + \frac{nRT}{V} dV = 0 \\
\frac{nRT}{V} dV = - n\ c_V\ dT \\
RT \frac{dV}{V} = - c_V\ dT \\
\frac{R}{c_V} \frac{dV}{V} = -\frac{dT}{T} \\
\frac{R}{c_V}\frac{dV}{V} = -\frac{dT}{T} \\
\frac{c_p-c_V}{c_V}\frac{dV}{V} = -\frac{dT}{T} \\
(\frac{c_p}{c_V}-\frac{c_V}{c_V})\frac{dV}{V} = -\frac{dT}{T} \\
(\gamma-1)\frac{dV}{V} = -\frac{dT}{T} \\
\end{gather*}$$
Integrando dallo stato A allo stato B
$$\begin{gather*}
\int_A^B(\gamma-1)\frac{dV}{V} = \int_A^B-\frac{dT}{T} \\[6pt]
(\gamma-1)\ ln(V)\bigg\rvert_{A}^{B} = -ln(T)\bigg\rvert_{A}^{B} \\[6pt]
(\gamma-1)\ (lnV_B-lnV_A) = -(lnT_B-lnT_A) \\[6pt]
(\gamma-1)\ ln\frac{V_B}{V_A} = ln\frac{T_A}{T_B} \\[6pt]
ln\left(\left(\frac{V_B}{V_A}\right)^{\gamma-1}\right) = ln\frac{T_A}{T_B} \\
\end{gather*}$$
L'uguaglianza tra logaritmi implica l'uguaglianza tra argomenti, quindi
$$\begin{gather*}
ln\left(\left(\frac{V_B}{V_A}\right)^{\gamma-1}\right) = ln\frac{T_A}{T_B} \\[6pt]
\left(\frac{V_B}{V_A}\right)^{\gamma-1} = \frac{T_A}{T_B} \\[6pt]
\frac{V_B^{\gamma-1}}{V_A^{\gamma-1}} = \frac{T_A}{T_B} \\[6pt]
T_A\ V_A^{\gamma-1} = T_B\ V_B^{\gamma-1}
\end{gather*}$$
Possiamo riscrivere questa relazione come relazione tra $p$ e $V$ o tra $p$ e $T$
+ $TV^{\gamma-1}$ = costante
+ $TV^{\gamma-1} = \frac{pV}{nR}V^{\gamma-1} = pV^{\gamma}$ = costante
+ $T\ p^{(1-\gamma)/\gamma}$ = costante
## Trasformazioni adiabatiche irreversibili
Un'esempio di trasformazione adiabatica irreversibile è quella dell'[[Energia interna di un gas#Esperimento di Joule|esperimento di espansione libera di Joule]] 

# Riassunto

|            | Isocore        | Isobare        | Isoterme        | Adiabatiche     |
| ---------- | -------------- | -------------- | --------------- | --------------- |
| $\Delta U$ | $nc_V\Delta T$ | $nc_V\Delta T$ | $0$             | $nc_V\Delta T$  |
| $Q$        | $nc_V\Delta T$ | $nc_p\Delta T$ | $nRln(V_B/V_A)$ | $0$             |
| $W$        | $0$            | $nR\Delta T$   | $nRln(V_B/V_A)$ | $-nc_V\Delta T$ |
