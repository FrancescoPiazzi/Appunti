Definiamo come centro di massa di una serie di punti materiali come la media pesata delle posizioni dei punti
$$ 
\vec{r}_{CM}
\stackrel{\text{def}}{=} 
\frac{\sum_{i=1}^n m_i\vec{r_i}}{\sum_{i=1}^n m_i} = 
\frac{\sum_{i=1}^n m_i\vec{r_i}}{M_{\text{TOT}}}
$$
+ $\vec{r}_{i}$ posizione i-esimo elemento
+ $m_i$ massa i-esimo elemento

Consideriamo la forza totale che agisce su un sistema come la somma delle forze interne ed esterne che agiscono su ogni punto
$$
\vec{F}_{\text{TOT}} = 
\sum_i^N (F_i^{\text{int}} + F_i^{\text{ext}})
$$
La forza che agisce su un corpo $i$ dovuta a fattori interni vale
$$
\vec{F}_{\text{i}}^{\text{int}} =
\sum_i^N \vec{F}_{j \rightarrow i} \
$$
Sommando le forze $j$-esime per ogni corpo $i$
$$
\sum_i^N\vec{F}_{\text{i}}^{\text{int}} =
\sum_i^N\sum_{j}^N \vec{F}_{j \rightarrow i} \ |\ i\ne j 
$$
Per il [[Leggi della dinamica#Terza legge della dinamica|terzo principio della dinamica]], per ogni forza interna $F_{i\rightarrow j}$ ne esiste una uguale e opposta  $F_{j\rightarrow i}$, quindi la forza totale del sistema è pari alla somma delle forze esterne 
$$
\vec{F}_{\text{TOT}} = \vec{F}_{\text{TOT}}^{\text{ext}} = 
\sum_i^N F_i^{\text{ext}} = 
\sum_i^N m_i\frac{d^2\vec{x}_i}{dt^2} = 
\frac{d^2}{dt^2} \left( \sum_i^N m_i\vec{x}_i \right)
$$
Ora divido e moltiplico per la massa totale del sistema, notando che quello tra parentesi è la definizione del centro di massa data prima
$$
M_{\text{TOT}} \frac{d^2}{dt^2} \left( \frac{\sum_i^N m_i\vec{x}_i}{M_{\text{TOT}}} \right) = 
M_{\text{TOT}} \frac{d^2\vec{r}_{CM}}{dt^2} = 
M_{\text{TOT}} \ \vec{a}_{CM}
$$
Da questo ricaviamo il **teorema del centro di massa**
$$ \vec{F}_{\text{TOT}} = M_{\text{TOT}} \ \vec{a}_{CM} $$


---------

La [[Quantità di moto|quantità di moto]] di un sistema si conserva dopo un qualunque urto