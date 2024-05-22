Il teorema di Clausius è una conseguenza dell'applicare la [[Principi della termodinamica#Secondo principio|seconda legge della termodinamica]] in ogni punto infinitesimo di un trasferimento di calore, Clausius ci dice che è impossibile costruire un motore che trasferisce calore da una sorgente fredda ad una calda senza usare lavoro dall'esterno, in modo simile.

# Disuguaglianza di Clausius
Ricordando la formula dell'efficienza di un motore termico:
![[Teorema e macchina di Carnot#^RendimentoMacchinaMotrice]]
Il lavoro è dato dalla differenza tra il calore dato e quello assorbito, possiamo quindi riscrivere la parte superiore come
$$
\mu = \frac{Q_a - |Q_c|}{Q_a} = 1 - \frac{|Q_c|}{Q_a}
$$
Studiando il ciclo di Carnot sappiamo che il suo rendimento vale
$$ \begin{gather*}
\mu = 1-\frac{T_1}{T_2}
\end{gather*} $$ Combinando le due sopra
$$ \begin{gather*}
1 - \frac{|Q_c|}{Q_a} = 1 - \frac{T_1}{T_2} \\
\frac{|Q_c|}{Q_a} = \frac{T_1}{T_2} \\
-\frac{Q_c}{Q_a} = \frac{T_1}{T_2} \\
\end{gather*}$$
L'ultimo passaggio si fa perché il calore ceduto da un motore termico è negativo, possiamo poi riscrivere il risultato come:
$$\begin{gather*}
-\frac{Q_1}{Q_2} = \frac{T_1}{T_2} \\
-\frac{Q_1}{T_1} = \frac{Q_2}{T_2} \\
\frac{Q_1}{T_1} + \frac{Q_2}{T_2} = 0\\
\end{gather*}$$
Da questo notiamo che la somma dei calori scambiati diviso le temperature è 0
$$
\sum_{i=1}^n \frac{Q_k}{T_k} = 0
$$
Con un numero infinito di trasformazioni si ha che
$$
\oint{\frac{\delta Q}{T}} = 0
$$
Se le trasformazioni non sono tutte reversibili, la differenza di entropia sarà più piccola, quindi:
$$
\Delta S =\oint{\frac{\delta Q}{T}} \le 0
$$
^DisuguaglianzaClausius

Da questa disuguaglianza possiamo derivare che la variazione di entropia di una trasformazione reversibile è maggiore di quella di una irreversibile
$$\begin{gather*}
\oint{\frac{\delta Q}{T}} \le 0 \\
\int_A^B{\frac{\delta Q_{rev}}{T}} + \int_B^A{\frac{\delta Q_{irr}}{T}} \le 0\\
\int_A^B{\frac{\delta Q_{rev}}{T}} \le -\int_B^A{\frac{\delta Q_{irr}}{T}} \\
\int_A^B{\frac{\delta Q_{rev}}{T}} \le \int_A^B{\frac{\delta Q_{irr}}{T}} \\
\end{gather*}$$

^Corollario1DisuguaglianzaClausius

Il teorema di Clausius dice anche che è possibile vedere qualunque trasformazione termodinamica come una serie infinitesima di cicli di Carnot ma non ho capito come (?)