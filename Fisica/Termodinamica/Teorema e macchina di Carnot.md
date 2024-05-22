Il teorema di Carnot si basa sulla macchina di Carnot, quindi è meglio vedere prima quella
# Macchina di Carnot
Due sorgenti di calore A e B, una calda ed una fredda, vengono messe alternativamente a contatto con un cilindro non ermetico pieno di un gas ideale, questo fa espandere e contrarre il gas all'interno, muovendo il pistone avanti e indietro, che quindi compie lavoro sull'esterno
![Engelbart|600](Carnot-engine.jpg)
Il rendimento di una qualunque macchina che trasforma calore in lavoro, vale:

$$ \eta = \frac{W}{Q_{in}} $$
^RendimentoMacchinaMotrice
+ $\eta$ rendimento ($0\le \eta \le1$)
+ $W = W_{in}+W_{out}$ lavoro (il lavoro in ingresso è già negativo)
+ $Q_{in}$ calore assorbito dalla macchina (quello ceduto dalla macchina è considerato sprecato)
Nel caso della macchina di Carnot, che compie una trasformazione ciclica, si ha che $\Delta U = 0 \Rightarrow Q=W$ (il calore ceduto è già negativo, stessa cosa per il lavoro eseguito sulla macchina dall'esterno)
$$\begin{gather*} 
\eta = \frac{W}{Q_{in}} = 
\frac{Q_{in}+Q_{out}}{Q_{in}} =
1 + \frac{Q_{out}}{Q_{in}} =
1 - \frac{|Q_{out}|}{Q_{in}}
\end{gather*}$$
+ $T_c$ temperatura corpo freddo
+ $T_h$ temperatura corpo caldo
# Ciclo di Carnot
Il ciclo di Carnot è composto da 
1. un'espansione isoterma $AB$ 
2. un' espansione adiabatica $BC$
3. una compressione isoterma $CD$ 
4. una compressione adiabatica $DA$
Il ciclo di Carnot prende calore dalla sorgente calda, e disperde parte di questo calore alla sorgente fredda, producendo lavoro con il resto

|            | AB                  | BC                | CD                  | DA                |
| ---------- | ------------------- | ----------------- | ------------------- | ----------------- |
| $\Delta U$ | 0                   | $nc_V(T_c-T_h))$  | $0$                 | $nc_V(T_h-T_c))$  |
| $Q$        | $nRT_h ln(V_B/V_A)$ | $0$               | $nRT_c ln(V_D/V_C)$ | $0$               |
| $W$        | $nRT_h ln(V_B/V_A)$ | $-nc_V(T_c-T_h))$ | $nRT_c ln(V_D/V_C)$ | $-nc_V(T_h-T_c))$ |

### Rendimento del ciclo
Ricordando il rendimento di un ciclo termico
![[#^RendimentoMacchinaMotrice]]
Sappiamo che i lavori prodotti dalle due trasformazioni isoterme valgono $nRT_h ln(V_B/V_A)$ e $nRT_c ln(V_D/V_C)$ 
Per le adiabatiche, sappiamo che 
$$\begin{gather*}
T_hV_B^{\gamma-1}=T_cV_C^{\gamma-1} \\
T_cV_D^{\gamma-1}=T_hV_A^{\gamma-1}
\end{gather*}$$
si hanno quindi
$$\begin{gather*}
(\frac{V_C}{​V_B}​​)^{\gamma-1}=\frac{Tc}{​Th} \\[6pt]
(\frac{V_A}{​V_D}​​)^{\gamma-1}=\frac{Tc}{​Th} \\
\end{gather*}$$​​(nota: non è  un passaggio algebrico, la prima riga è derivata dalla prima adiabatica, la seconda riga dalla seconda)




$$\begin{gather*}
\eta = 1 + \frac{Q_{out}}{Q_{in}} \\[6pt]
\eta = 1 + \frac{nRT_1ln(V_D/V_C)}{nRT_2ln(V_D/V_A)} \\[6pt]
\eta= 1 - \frac{T_1ln(V_C/V_D)}{T_2ln(V_D/V_A)} \\[6pt]
\eta = 1 - \frac{T_c}{T_h}
\end{gather*}$$
# Teorema di Carnot

Il teorema di Carnot afferma che non può esistere una macchina termica che opera tra due sorgenti di calore che abbia un efficienza maggiore di una macchina di Carnot operante tra le due stesse sorgenti.
Durante la trasformazione da energia termica ad energia meccanica, il rendimento del motore è la percentuale di energia che viene trasformata in lavoro termodinamico, il teorema di Carnot afferma inoltre che il motore non può trasformare tutto il calore della sorgente in energia meccanica, di nuovo, la massima quantità di calore estraibile si estrae con la macchina di Carnot.

Il teorema di Carnot si può esprimere come disuguaglianza che coinvolge solamente i flussi di calore, e le temperature delle sorgenti, per una qualunque macchina che lavora tra le temperature $T_1$ e $T_2$ vale la seguente
$$ \frac{Q_1}{Q_2} + \frac{T_1}{T_2} \le 0$$
Il minore vale per i cicli irreversibili, l'uguale per quelli reversibili.

