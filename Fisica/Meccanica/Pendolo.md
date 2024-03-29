Il pendolo è un sistema meccanico nel quale una massa è appesa ad una fune inestensibile di lunghezza non parallela alla direzione della gravità, l'estremo della fune non connesso alla massa è fissato, di conseguenza la massa oscillerà attorno ad un punto di equilibrio, che sarà il punto nel quale fisseremo il nostro sistema di riferimento (nell'immagine sul punto D, con l'asse x verso destra e l'asse y verso l'alto)
![[pendolo.png]]
Chiameremo: 
+ $m$ la massa appesa al filo ($Kg$)
+ $l$ la lunghezza della fune ($m$)
+ $g$ l'accelerazione gravitazionale ($m/s^2$)
+ $\theta \in [-\pi/2, \pi/2]$ l'angolo iniziale della fune rispetto al $g$ 

# Accelerazione scomponendo le forze
La forza peso della massa $m$ vale
$$ P = mg$$
Possiamo scomporre la forza peso in una componente parallela ed una perpendicolare alla fune:
$$ \begin{aligned}
P_\perp = P\ cos(\theta) = m\ g\ cos(\theta) \\
P_\| = P\ sin(\theta) = m\ g\ sin(\theta) \\
\end{aligned} $$
Ora possiamo usare la componente parallela per ricavare le componenti della forza peso rispetto al nostro sistema di riferimento
$$\begin{gather*}
P_x = P_{\|} \ cos(\theta) = mg\ sin(\theta)\ cos(\theta)\\
P_y = P_{\|} \ sin(\theta) = mg \ sin^2(\theta)
\end{gather*}$$
Da queste l'accelerazione rispetto agli assi è banale
$$\begin{gather*}
a_x = \frac{P_x}{m} = -|g|\ sin(\theta)\ cos(\theta)\\
a_y = \frac{P_y}{m} = -|g|\ sin^2(\theta)\\
\end{gather*}$$
# Accelerazione derivando la posizione
Osservando la posizione del peso rispetto all'angolo, notiamo che
$$ \begin{gather*}
x = l\ sin(\theta) \\
y = l-l\ cos(\theta)
\end{gather*}$$
Possiamo ricavare l'accelerazione derivando due volte rispetto al tempo
$$ 
\left\{ 
    \begin{array}{l}
        x = l\ sin(\theta) &\\
		y = l-l\ cos(\theta)
    \end{array} 
\right.
\xRightarrow{d/dt}
\left\{ 
    \begin{array}{l}
        v_x = l\ cos(\theta)\dot{\theta} &\\
        v_y = l\ sin(\theta)\dot{\theta} 
    \end{array} 
\right.
\xRightarrow{d/dt}
\left\{ 
    \begin{array}{l}
        a_x = -l\ sin(\theta)\dot \theta^2 \ +\ l\ cos(\theta)\ \ddot \theta &\\
        a_y = l\ cos(\theta)\dot \theta^2 \ +\ l\ sin(\theta)\ \ddot \theta 
    \end{array} 
\right.
$$
# Moto armonico di un pendolo
Avendo osservato il moto da due punti di vista diversi, possiamo dimostrare che il moto di un pendolo è approssimabile ad un [[Moto armonico |moto armonico]] se consideriamo $\theta$ abbastanza piccolo:
$$ sin(\theta) \approx \theta,\ cos(\theta) \approx 1, \ tan(\theta) \approx 1$$
Riscriviamo il sistema ed applichiamo queste approssimazioni
$$ \begin{gather*}
\left\{ 
    \begin{array}{l}
         -|g|\ sin(\theta)\ cos(\theta) = -l\ sin(\theta)\dot \theta^2 \ +\ l\ cos(\theta)\ \ddot \theta &\\
          -|g|\ sin^2(\theta) = l\ cos(\theta)\dot \theta^2 \ +\ l\ sin(\theta)\ \ddot \theta 
    \end{array} 
\right. \\ \\
\left\{ 
    \begin{array}{l}
        -|g|\ \theta = -l\ \theta \ \dot \theta^2 \ +\ l\ \ddot \theta &\\
	    -|g|\ \theta^2 = l\ \dot \theta^2 \ +\ l\ \theta\ \ddot \theta 
    \end{array} 
\right.
\end{gather*} $$
Essendo $\theta$ molto piccolo, possiamo approssimare $\theta^2$ a 0
$$
\left\{ 
    \begin{array}{l}
        -|g|\ \theta = -l\ \theta \ \dot \theta^2 \ +\ l\ \ddot \theta &\\
	    0 = l\ \dot \theta^2 \ +\ l\ \theta\ \ddot \theta 
    \end{array} 
\right.
\Rightarrow \
\left\{ 
    \begin{array}{l}
        -\frac{|g|}{l}\ \theta = - \theta \ \dot \theta^2 \ +\ \ddot \theta &\\
	    0 = \dot \theta^2 \ +\ \theta\ \ddot \theta 
    \end{array} 
\right.
\Rightarrow \
\left\{ 
    \begin{array}{l}
        -\frac{|g|}{l}\ \theta = - \theta \ \dot \theta^2 \ +\ \ddot \theta &\\
	    \dot \theta^2 \ = -\ \theta\ \ddot \theta 
    \end{array} 
\right.
$$
Ora possiamo sostituire $\dot \theta^2$ nella prima equazione
$$\begin{gather*} 
-\frac{|g|}{l}\ \theta = - \theta \ \dot (-\ \theta\ \ddot \theta )) \ +\ \ddot \theta \\
-\frac{|g|}{l}\ \theta = \theta^2 \ \ddot \theta \ +\ \ddot \theta \\
-\frac{|g|}{l}\ \theta = \ddot \theta \\
-\frac{|g|}{l}\ \theta = \ddot \theta \\
\ddot \theta \ + \frac{|g|}{l} \theta = 0
\end{gather*}$$
Abbiamo ricavato un'equazione nella forma $\ddot x +\alpha x = 0$ , che è un'equazione del moto armonico, dimostrando quindi che per piccole oscillazioni, il moto di un pendolo è approssimabile ad un moto armonico
