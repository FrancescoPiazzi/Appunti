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
\end{gather*}$$​​*(nota: non è  un passaggio algebrico, la prima riga è derivata dalla prima adiabatica, la seconda riga dalla seconda)*




$$\begin{gather*}
\eta = 1 + \frac{Q_{out}}{Q_{in}} \\[6pt]
\eta = 1 + \frac{nRT_1ln(V_D/V_C)}{nRT_2ln(V_D/V_A)} \\[6pt]
\eta= 1 - \frac{T_1ln(V_C/V_D)}{T_2ln(V_D/V_A)} \\[6pt]
\eta = 1 - \frac{T_c}{T_h}
\end{gather*}$$
# Teorema di Carnot
Consideriamo due macchine termiche, X ed R; che lavorano tra due sorgenti di calore alle temperature $T_1$ e $T_2$, con $T_1<T_2$, dimensionate in modo da assorbire lo stesso calore $Q_2$, la prima potrebbe essere reversibile oppure no, mentre la seconda è sicuramente reversibile $R$
I rendimenti delle due macchine saranno $\eta_X = W_X/Q_2$ e $\eta_R = W_R/Q_2$, essendo $R$ reversibile, possiamo farla funzionare al contrario come macchina frigorifera, scambiando di segno calore e lavoro scambiati da essa.
Dato che $R$ è reversibile, ha rendimento 1, quindi tutto il calore ($=Q_2$) assorbito da $T_1$ verrà trasferito a $T_2$, questo significa che $T_2$ non scambia complessivamente calore.
Per l'[[Principi della termodinamica#Secondo principio#Chiacchere|enunciato di Kelvin plank]], questa macchina non può produrre lavoro (se lo facesse staremmo prendendo calore da $T_1$ e convertendolo tutto in lavoro senza risultati esterni), questo significa che il lavoro prodotto dalla macchina $X$ deve essere minore o uguale di quello prodotto dalla macchina $R$
$$\begin{gather*}
W_X \le W_R \\
\frac{W_X}{Q_2} \le \frac{W_R}{Q_2} \\
\eta_X \le \eta_R
\end{gather*}$$
In particolare, se $X$ è reversibile possiamo rifare tutto il ragionamento dove però facciamo diventare $X$ un frigorifero, ottenendo $\eta_X \ge \eta_R$, e quindi $\eta_X = \eta_R$, mentre se $X$ è irreversibile si ha che $\eta_X \lt \eta_R$

-------------
(old stuff)
Il teorema di Carnot afferma che non può esistere una macchina termica che opera tra due sorgenti di calore che abbia un efficienza maggiore di una macchina di Carnot operante tra le due stesse sorgenti.
Durante la trasformazione da energia termica ad energia meccanica, il rendimento del motore è la percentuale di energia che viene trasformata in lavoro termodinamico, il teorema di Carnot afferma inoltre che il motore non può trasformare tutto il calore della sorgente in energia meccanica, di nuovo, la massima quantità di calore estraibile si estrae con la macchina di Carnot.

Il teorema di Carnot si può esprimere come disuguaglianza che coinvolge solamente i flussi di calore, e le temperature delle sorgenti, per una qualunque macchina che lavora tra le temperature $T_1$ e $T_2$ vale la seguente
$$ \frac{Q_1}{Q_2} + \frac{T_1}{T_2} \le 0$$
Il minore vale per i cicli irreversibili, l'uguale per quelli reversibili.

