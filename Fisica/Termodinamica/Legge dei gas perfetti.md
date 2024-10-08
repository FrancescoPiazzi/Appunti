# Prologo
## Legge di Boyle
Si consideri un gas in equilibrio termodinamico ad una certa pressione $p$ e volume $V$ a una certa temperatura $T$, se si fa variare la pressione o il volume, mantenendo la temperatura uguale, si ha che
$$ p V = costante$$
^leggeDiBoyle
Una trasformazione di questo tipo si può fare comprimendo un gas che è in contatto con una sorgente a temperatura costante
Questo significa che comunque il gas passi da una pressione e volume $p_1$ e $V_1$ ad una pressione e volume $p_2$ e $V_2$, se la temperatura dello stato iniziale e finale è la stessa (può variare durante la trasformazione), si ha che:
$$p_1 V_1 = p_2 V_2$$
Riassumendo, possiamo dire che
***In una trasformazione isoterma, pressione e volume sono inversamente proporzionali***
## Leggi di Volta-Gay Lussac
Se invece il gas non cambia di pressione durante una trasformazione (i.e. lo mettiamo in un cilindro), si ha che il volume varia linearmente con la temperatura
$$ V = V_0(1+\alpha t)$$
+ $V$ volume
+ $V_0$ volume occupato dal gas quando t=0 °C
+ $\alpha$ costante che varia (poco) al variare del gas
+ $t$ (C°) temperatura

Se si mantiene il volume costante, si ha un risultato simile
$$ p = p_0(1+\beta t)$$
+ $p$ pressione
+ $p_0$ pressione occupata dal gas quando t=0 °C
+ $\beta$ costante che varia (poco) al variare del gas
+ $t$ (°C) temperatura

Da questi ultimi due esperimenti si nota che, quando il gas si avvicina alla condizioni di un gas ideale (bassa pressione e alta temperatura), si osserva che $\alpha$ e $\beta$ assumono lo stesso valore per tutti i gas
$$\alpha = \beta = \frac{1}{273.15}°C^{-1}$$
Le formule precedenti possono essere quindi riscritte come:
$$ V = V_0(1+\alpha t) = V_0\ \alpha\ (\frac{1}{\alpha}+t) = V_0 \ \alpha \ T$$
$$ p = p_0(1+\alpha t) = p_0\ \alpha\ (\frac{1}{\alpha}+t) = p_0 \ \alpha \ T$$
+ $T = \frac{1}{\alpha} + t = 273.15 + t$, ovvero la temperatura convertita da Celsius in Kelvin

Da questa formulazione notiamo che alla temperatura di 0 Kelvin si hanno $p=0$ e $V=0$, questo rappresenta uno stato limite, e, oltre ad essere di per sé irragginugibile, temperature inferiori a 0 Kelvin non hanno senso
## Legge di Avogadro
***Una mole di gas a una data temperatura e pressione occupa sempre lo stesso volume***
Questo indipendentemente da cosa sia composto il gas, a pressione atmosferica e 0°C si ha che $V_m = 0.022 m^3$, dove $V_m$ indica il volume molare

# Legge dei gas perfetti
Sappiamo dalla legge di Avogadro che, se consideriamo n moli di un gas a 0°C e a pressione atmosferica, il suo volume sarà $V_0 = nV_m$
Ora portiamo questo gas a uno stato qualsiasi C, ciò può essere fatto in molti modi, uno può essere quello di fare una trasformazione isocora dallo stato A allo stato B, seguita da una isoterma dallo stato B allo stato C
Sappiamo dalle leggi di Gay-Lussac che la pressione dopo la trasformazione isocora sarà 
$p_b = p_a\ \alpha\ T$, sappiamo dalla legge di Boyle che il prodotto pressione volume rimane costante in una trasformazione isoterma, quindi abbiamo che
$$pV = p_BV_A = p_A \alpha T V_A = np_AV_m\alpha T$$
$p_0$ e $V_m$, e $\alpha$ sono costanti, possiamo quindi racchiuderli in un'unica costante $R$, e ottenere:
$$
pV = nRT
$$
^GasPerfetti1
+ $p$ pressione ($pascal$)
+ $V$ volume ($m^3$)
+ $n$ numero molecole
+ $R$ costante gas ($\frac{J}{mol*K}$)
+ $T$ temperatura ($K$)

La costante $R$ rappresenta il lavoro che $1$ mole di gas compie quando si espande in seguito all'aumento della temperatura di $1$ Kelvin a pressione costante.
In termini pratici, si ha che
$$ \begin{aligned}
R = N_a\ k_b \\
k_b = \frac{R}{N_a}
\end{aligned} $$
^CostanteBoltzmann
+ $N_a$ Numero di Avogadro ($\frac{molecole}{moli}$) $\approx 6.26 \times 10^{23}$
+ $k_b$ Costante di Boltzmann ($\frac{J}{K}$) $\approx 1.38 \times 10^{-23} JK^{-1}$

Quindi $R \approx 8.31 \frac{J}{mol\cdot K}$
Potevamo ricavare $R$ anche dal prodotto $p_0 \ V_m \alpha$: $R = 101325 * 0.0224 * \frac{1}{273.15} = 8.309\frac{J}{mol\cdot K}$

******

Possiamo riscrivere la formula originale in modo diverso in dividendo per il volume
$$ p = n_m\ R\ T $$
+ $n_m$ densità molare ($\frac{mol}{m^{3}}$)
Ora introduciamo $n = n_m N_a$ dove $n$ è il numero di molecole per metro cubo e osserviamo che compare la costante di Boltzmann
$$ \begin{gather*}
p = n_m\ \frac{R}{N_a}\ T \\
p = n_m\ k_b\ T
\end{gather*} $$
^GasPerfetti2