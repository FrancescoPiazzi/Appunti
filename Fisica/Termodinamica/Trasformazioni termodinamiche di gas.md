# Lavoro delle trasformazioni termodinamiche
Ricordando che il lavoro di un corpo che si muove lungo una traiettoria $\gamma$ vale ![[Lavoro#^Lavoro]]
E ricordando che una pressione è una forza su una superficie, se la superficie è costante pressione e forza sono proporzionali. Se mettiamo il gas in un cilindro, anche spostamento e volume sono proporzionali.
Quindi possiamo veder il lavoro di una trasformazione termodinamica in modo simile a come vediamo il lavoro meccanico
$$ W =\int_{V_A}^{V_B} P \ dv$$
# Entropia delle trasformazioni termodinamiche
$$\Delta S= \int_A^B \frac{\delta Q}{T} = \int_A^B \frac{1}{T} \ \delta Q$$
# Trasformazioni isobare
In un'isobara la pressione è costante, quindi abbiamo che il lavoro vale
$$ W =\int_{V_A}^{V_B} P\ dv = PV \bigg\rvert_{V_A}^{V_B} = P(V_B - V_A)$$
La variazione di entropia da uno stato A ad uno stato B vale
$$ Q_{A\rightarrow B} = n \ c_p \ \Delta T$$
+ $n$ numero moli
+ $c_p$ calore specifico di quel gas a pressione costante
# Trasformazioni isocore
In un'isocora è il volume ad essere costante, essendo gli estremi di integrazione uguali, il lavoro sarà 0
$$ W =\int_{V_A}^{V_A} P \ dv = 0$$
La variazione di entropia da uno stato A ad uno stato B è molto simile a quella delle isocore:
$$ Q_{A\rightarrow B} = n \ c_v \ \Delta T$$
+ $n$ numero moli
+ $c_v$ calore specifico di quel gas a volume costante
# Trasformazioni isoterme
Nelle isoterme cambiano tutte e due quindi è un casino, dobbiamo riscrivere P come $\frac{nrt}{V}$ usando la [[Legge dei gas perfetti |legge dei gas perfetti]]

$$ W =\int_{V_A}^{V_B} P \ dv = 
\int_{V_A}^{V_B} \frac{nrt}{V} dv = 
nrt \ \bigg\rvert ln(V)\bigg\rvert_{V_A}^{V_B} = 
nrt \ ln(\frac{V_B}{V_A})$$
Essendo la temperatura costante, $1/T$ è costante, quindi la variazione di entropia vale:
$$ \Delta S = \int_A^B \frac{1}{T} \ \delta Q = \frac{Q}{T} $$
# Trasformazioni adiabatiche
## Trasformazioni adiabatiche reversibili
Non essendoci trasferimento di calore, l'entropia non cambia
$$\Delta S = 0$$
## Trasformazioni adiabatiche irreversibili
Non essendoci trasferimento di calore, l'entropia non cambia?