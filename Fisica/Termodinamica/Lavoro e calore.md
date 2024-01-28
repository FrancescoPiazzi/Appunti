[[Lavoro]] e [[Calore]] sono legati molto strettamente, non a caso si misurano entrambe in Joule. Vediamo un paio di esempi
# Trasformazione di lavoro meccanico in calore
Per scaldare un liquido all'interno di un contenitore ermetico, potremmo collegare un peso ad una fune che aziona un mulinello con delle pale all'interno del contenitore, quando il peso viene fatto cadere, le pale girano all'interno del liquido, scaldandolo per attrito

![Engelbart|300](joule-s-experiment.jpg)

Per portare il peso ad una certa altezza (se sono due come nell'immagine facciamo finta sia uno il doppio più pesante), è necessario un lavoro pari a:
$$L_p = \int_0^h F_p \ dy = \int_0^h m\ g\ dy = mgy \bigg\rvert_{0}^{h} = m\ g\ h$$
+ $m$ massa da portare in alto
+ $g$ gravità
+ $h$ altezza al quale portare la massa
Che guarda a caso è uguale all'energia potenziale gravitazionale.

Dal punto di vista del calore dell'acqua si ha che:
![[Calore#^CaloreSensibile]]
Nel nostro caso, assumendo un'efficienza della trasformazione di 1 (irragionevole per il [[Principi della termodinamica#Secondo principio|secondo principio della termodinamica]]), il calore trasferito al liquido è lo stesso del lavoro fatto dal peso che cade, quindi abbiamo che
$$ m\ g\ h = c\ m \ \Delta T $$
Se l'efficienza avesse avuto un valore minore di 1, chiamiamolo $\eta$ (eta), avremmo avuto
$$ \eta \ m\ g\ h = c\ m \ \Delta T  $$
Risolvendo per $\eta$, notiamo che infatti misura la quantità di calore assorbito rispetto al lavoro compiuto:
$$ \eta =  \frac{c\ m \ \Delta T}{m\ g\ h} = \frac{Q_{out}}{W_{in}}$$
Confrontandolo con il rendimento di una macchina motrice
![[Teorema e macchina di Carnot#^RendimentoMacchinaMotrice]]
Dal punto di vista delle direzioni dei flussi di calore e lavoro, notiamo che sono scambiati, questo ha senso perché, al posto di trasformare calore in lavoro come una macchina motrice, stiamo facendo l'opposto.
Dal punto di vista delle direzioni dei flussi di energia, invece notiamo che sono uguali, abbiamo sempre un rapporto tra energia in uscita ed energia in entrata

# Trasformazione di calore in lavoro meccanico
Un esempio è la macchina di Carnot:
![[Teorema e macchina di Carnot#Macchina di Carnot]]