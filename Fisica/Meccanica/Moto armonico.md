Il moto armonico è un tipo di moto descritto da un'equazione di questo tipo:
$$ \ddot x +\alpha x = 0 $$
+ $\ddot x =\frac{d^2x}{dt^2}$
+ $\alpha$ numero reale

Nel caso in cui il moto descriva il movimento di una [[Molle|molla]] o di un [[Pendolo|pendolo]], si ha che:
$$\frac{d^2x}{dt^2} = -\frac{kx}{m} $$

+ $m$ massa inerziale
+ $x$ spostamento rispetto alla situazione di equilibrio
+ $k$ costante

Risolvere questa equazione produce
$$ x(t) = c_1\ cos(\omega t)\ + \ c_2\ sin(\omega t)$$
+ $\omega = \sqrt{k/m}$ 
+ $c_1$ posizione dell'oggetto al tempo 0
+ $c_2$ velocità iniziale / frequenza angolare

Spiegazione di $c_2 = v_0/\omega$
$$\begin{gather*} 
x(t) = c_1\ cos(\omega t)\ + \ c_2\ sin(\omega t) \\
\dot x(t) = -c_1\ sin(\omega t)\omega\ + \ c_2\ cos(\omega t)\ \omega \\
\dot x(0) = c_2\ \omega = v_0 \\
c_2 = v_0/\omega
\end{gather*}$$
Questo ci consente di riscrivere l'equazione originale come
 $$ x(t) = x_0\ cos(\sqrt{\frac{k}{m}}\ t)\ +
 \ \frac{v_0}{\sqrt{\frac{k}{m}}}\ sin(\sqrt{\frac{k}{m}} t) $$ La stessa equazione può anche essere riscritta nel seguente modo
$$x(t) = A \ cos(\omega t - \varphi)$$
 + $A = \sqrt{c_1^2 + c_2^2}$
 + $\varphi = atan2(c_2/c_1)$
