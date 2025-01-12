Le cose si muovono così quando l'accelerazione è costante:
$$
\begin{aligned}
s(t) = s_0 + v_0t + \frac{1}{2}a{t}^{2} \\
v(t) = s(t)\frac{ds}{dt} = v_0 + a{t}
\end{aligned}
$$
^SpazioEVelocita
questo perché:
$$
s(t) = s_0 + \int_0^{t} v(\tau)d\tau = s_0 + \int_0^{t} v_0 + a{\tau} d\tau = s_0 +(v_0\tau+\frac{1}{2}a\tau^2)\bigg\rvert_{0}^{t} = s_0 + v_0t+\frac{1}{2}at^2
$$

# Prima legge della dinamica
Se non muovi qualcosa non si muove (waw)

# Seconda legge della dinamica
$$F = ma$$
Usando questa, possiamo riscrivere le leggi che descrivono la velocità e la posizione di un punto in modo più generico, ovvero dove ad un punto con una posizione iniziale $x_0$ ed una velocità iniziale $v_0$, viene applicata una forza potenzialmente variabile in funzione della sua posizione, velocità, o del tempo

$$
\vec{v}(t) \stackrel{\text{def}}{=} 
\vec{v_0} + \int_{t_0}^t \vec{a}(\tau) d\tau = 
\vec{v_0} + \int_{t_0}^t \frac{\vec{F}(\vec{x},\ \vec{v},\ \tau)}{m} d\tau
$$
^VelocitaPuntoConFFunzione

$$
\vec{x}(t) \stackrel{\text{def}}{=} 
\vec{x_0} \int_{t_0}^t \vec{v}(\tau) d\tau = 
\vec{x_0} + \int_{t_0}^t 
	\left(v_0 +\int_{t_0}^t \frac{\vec{F}(\vec{x},\ \vec{v},\ \tau)}{m} d\tau
	\right) d\sigma
$$
^PosizionePuntoConFFunzione

# Terza legge della dinamica
$$F_{1\rightarrow2} = -F_{1\rightarrow2}$$
