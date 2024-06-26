Il calore è una forma di energia, quindi si misura in Joule, il calore ceduto (o ricevuto) da un corpo durante una trasformazione termodinamica è:

$$ Q = c\ m \ \Delta T $$^CaloreSensibile

+ $c$ calore specifico
+ $m$ massa corpo
+ $\Delta T$ differenza tra la temperatura del corpo e l'esterno
Il $\Delta T$ nella formula del calore ci comunica qualcosa di molto importante: il calore corrisponde allo scambio di energia fra due sistemi dovuto ad una differenza di temperatura, è definibile come energia in transito, e quindi non come energia posseduta da un corpo, non ha senso dire che un corpo più caldo ha "più calore", perché il calore esiste solo quando esiste un trasferimento di energia (termica) tra due corpi.
Questa quantità di calore scambiata viene detta calore sensibile.
Durante la transizione da uno stato della materia ad un altro di un corpo, il calore ricevuto  da quel corpo non modifica la sua temperatura, ma viene usato per rompere i suoi legami molecolari, questo calore si chiama calore latente:
$$ Q = \lambda m$$
$\lambda$ è un parametro che varia in base al materiale, e si misura in $J/Kg$ ogni materiale ha due calori latenti: uno di fusione e uno di ebollizione.

Il prodotto $C=mc$ è detto **capacità termica** e rappresenta il calore necessario da fornire o sottrarre ad un corpo con un certo calore specifico c e una certa massa m per far variare la sua temperatura di 1K.

Se due corpi a temperature diverse vengono messi in contatto in un recipiente adiabatico quello con la temperatura maggiore cederà calore a quello con la temperatura minore fino a quando entrambe i corpi non avranno la stessa temperatura $T_e$, essendo il recipiente adiabatico, non c'è stata dispersione di calore all'esterno (nè ne è stato aggiunto) questo significa che il calore ceduto dal corpo più caldo $Q_1$ è uguale in modulo e opposto in segno a quello ceduto da quello più freddo $Q_2$, quindi $Q_1=-Q_2$. Utilizzando la [[#^CaloreSensibile|definizione di calore sensibile]]:
$$ \begin{gather*}
m_1 c_1 (T_e-T_1) = -m_2 c_2 (T_e-T_2) \\[8pt]
m_1 c_1 T_e - m_1 c_1 T_1 = -m_2 c_2 T_e + m_2 c_2 T_2 \\[8pt]
m_1 c_1 T_e + m_2 c_2 T_e = m_1 c_1 T_1 + m_2 c_2 T_2 \\[8pt]
T_e = \frac{m_1 c_1 T_1 + m_2 c_2 T_2}{m_1 c_1 + m_2 c_2} \\[8pt]
T_e = \frac{C_1 T_1 + C_2 T_2}{C_1 + C_2} \\
\end{gather*}$$
Notiamo che questa è semplicemente la media pesata delle temperature dei due corpi, con la loro capacità termica come peso
Nel caso di gas a contatto, la formula è la stessa, tuttavia i calori specifici sono diversi a seconda delle condizioni in cui avviene lo scambio di calore, ovvero se avviene a pressione o a volume costante. In teoria questa distinzione andrebbe fatta anche per i solidi e i liquidi, tuttavia la variazione di pressione o volume di questi ultimi è spesso abbastanza piccola da poter essere trascurata.
In molte situazioni torna utile avere il calore trasferito da un certo numero di moli $n$, in questo caso si parla di calore specifico molare che può essere calcolato come
$$ c = \frac{dQ}{n \ dT}$$
Il numero di moli in una massa di una certa sostanza è:
$$n = \frac{M}{N_A \ m}$$
+ $n$ numero di moli
+ $M$ massa del corpo
+ $N_A$ numero di Avogadro
+ $m$ massa di una molecola

In realtà il calore specifico di un corpo dipende dalla sua temperatura, tuttavia, a temperature lontane dallo zero assoluto, cambia molto poco, quindi lo possiamo considerare costante