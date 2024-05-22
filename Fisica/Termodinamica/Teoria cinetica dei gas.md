Consideriamo un modello di gas ideale in un recipiente cubico di lato $a$, dove:
1. il gas è costituito da molecole eguali in moto continuo e disordinato
2. gli urti tra molecole e molecole e contenitore sono elastici
3. non ci sono forze intermolecolari oltre a quelle derivate dagli urti
4. le dimensioni delle molecole sono molto piccole rispetto alla distanza media tra esse

Questo implica che
1. la velocità media del gas è nulla
2. negli urti tra molecole si conservano le [[Quantità di moto|quantità di moto]] ed energia, negli urti tra molecole e pareti si conserva l'energia
3. l'energia potenziale interna è nulla, si ha solo energia cinetica (nota: energia potenziale $\ne$ [[Energia interna di un gas|energia interna]])
4. il volume occupato dalle molecole è trascurabile rispetto a quello del recipiente

Si osservi che nell'urto contro una parete parallela al piano $yz$, solo la componente $x$ cambia, più precisamente il suo segno si inverte, la variazione della [[Quantità di moto|quantità di moto]] vale $-2mv_xu_x$, l'impulso ricevuto dalla parete vale quindi $2mv_xu_x$, l'urto successivo sulla stessa parete avverrà dopo $\Delta t = 2a/v_x$, ovvero il tempo necessario per attraversare il volume del solido due volte, non è detto che la molecola rimanga la stessa per via di urti con altre molecole, tuttavia a causa della prima ipotesi, per ogni molecola che perde la componente $v_x$, ce n'è un'altra che l'acquista in seguito ad un altro urto
Questo porta il numero di urti al secondo sulla parete $yz$ a $1/\Delta t = v_x/2a$, la forza media esercitata da ogni molecola sulla parete vale quindi in modulo:
$$F_x = 2mv_x\frac{v_x}{2a}=\frac{mv_x^2}{a}$$
+ $m$ massa di una molecola
+ $a$ lunghezza lato del cubo
+ $v_x$ componente $x$ della velocità di quella molecola
La forza totale sulla parete è la somma delle forze esercitate in media da ogni molecola:
$$R_x = \frac{m}{a} \sum_iv_{x, i}^2$$
La pressione sulla parete di area $S = a^2$ vale quindi
$$ p = 
\frac{R_x}{S} = 
\frac{m}{a^3} \sum_iv_{x, i}^2 = 
\frac{Nm}{V}\frac{1}{N} \sum_i v_{x, i}^2
$$
+ $N$ numero di molecole nel cubo
+ $V=a^3$ volume del cubo

Ora introduciamo la definizione di velocità media quadratica:
$$\overline{v}^2 = \overline{v}^2_x + \overline{v}^2_y + \overline{v}^2_z = 
\frac{1}{N}\sum_i \overline{v}^2_{x, i} + \overline{v}^2_{y, i} + \overline{v}^2_{z, i}
$$
Per l'ipotesi 1 i valori medi di $\overline{v}^2_x$, $\overline{v}^2_y$ e $\overline{v}^2_z$ sono uguali, quindi:
$$
\overline{v}^2_x = 
\overline{v}^2_y = 
\overline{v}^2_z = 
\frac{\overline{v}^2}{3}
$$
Unendo questo risultato alla formula per la pressione ottenuta precedentemente:
$$p = \frac{Nm}{V} \frac{\overline{v^2}}{3} \Rightarrow 
pV = \frac{1}{3} Nm\overline{v^2}$$
Questo risultato è identico per tutte le pareti e non dipende dalla forma del contenitore
Definendo ora **l'energia cinetica media** $\overline{E_k} = \frac{1}{2} m \overline{v^2}$ si ha che:
$$\begin{gather*}
pV = \frac{2}{3}NE_k \\
nRT = \frac{2}{3}NE_k \\
E_k = \frac{3}{2} \frac{n}{N}RT \\
E_k = \frac{3}{2} \frac{R}{N_a}T \\
E_k = \frac{3}{2} k_BT \\
\end{gather*}$$
nota: $n$ è il numero di moli, $N$ quello di molecole, quindi $\frac{n}{N} = \frac{1}{N_A}$ 

Se questo modello è corretto, possiamo concludere che ***la temperatura è proporzionale all'energia cinetica media***

Nel caso di un gas monoatomico, l'energia meccanica di una molecola è uguale alla sua energia cinetica, essendo l'energia cinetica costituita da tre gradi di liberta ($x$, $y$, e $z$), diremo che il sistema ha tre gradi di libertà, ogni atomo aggiuntivo aggiunge due gradi di libertà alla molecola, quindi l'energia cinetica media per un gas generico vale
$$E_k = \frac{l}{2}k_BT$$
+ $l$ gradi di libertà del gas (3, 5, 7...)
es. in un gas biatomico, i due atomi possono spostarsi in una qualunque delle tre direzioni, possono ruotare come le estremità di un bastone di un samurai, oppure possono ruotare lungo l'asse che li connette

Ad alte temperature entra in gioco anche il moto di vibrazione degli atomi, aggiungendo altri due gradi di libertà