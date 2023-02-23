Domanda, Dato un sistema dinamico sottoposto ad ingresso $u = \begin{pmatrix}t\\k\end{pmatrix} = \bar{u}$ costante.
$\exists$ quale $\bar{x}$ costante/i tale per cui
 $$
\begin{rcases}
x(0) = \bar{x} \\
u = \begin{pmatrix}
t \\
k
\end{pmatrix} = \bar{u}\quad \text{per }t,k \geq 0
\end{rcases} \to x \begin{pmatrix}
t \\
k
\end{pmatrix} = \bar{x} 
\text{ per } t,k \geq 0 ?
$$

Se esistono, tali $\bar{x}$ si dicono **stati di equilibrio** per $u = \bar{u}$


Come trovare gli stati di equilibrio?

## Tempo continuo
Se $x$ deve rimanere costante ($\bar{x}$) allora $\dot{x}$ deve essere zero quindi dato $\dot{x} = f(x,u)$
con $u = \bar{u}$ costante
Gli eventuali stati di equilibrio $\bar{x}$ sono le eventuali soluzioni di $f(\bar{x},\bar{u}=0)$



## Tempo determinato
Se $x$ deve rimanere costante allora $x(k+1) = x(k) \forall k$ quindi dato $x(k) = f(n(k-1),u(k-1))$ con $u(k) = \bar{u}$ cost.
Gli equilibri sono le soluzioni di $\bar{x} = f(\bar{x},\bar{u})$

## [[sistemi dinamici LTI]] a tempo continuo
$$
\begin{cases}
\dot{x} = Ax + bu \\
y = cx + du
\end{cases}
$$
$u=\bar{u}$ costante gli equilibri soluzionei di $0 = A\bar{x} + b\bar{u}$
Se $A$ non è singolare (?) $\exists! \bar{x} = -A^{-1}b\bar{u}$
altrimenti o $\cancel{ \exists } \bar{a}$ o $\exists \infty \bar{a}$i

## Uscita di equilibrio
Se $\exists \bar{x}$ per $u = \bar{u}$ in generale puó esistere l'uscita di equilibrio $\bar{y} = g(\bar{x},\bar{u})$
Nel caso LTI $\exists$ sempre $\bar{y} = c\bar{x} + d\bar{u}$



>[!esempio] Esempio 1 - Massa molla
> $$
>\begin{cases}
>\dot{x}_{1} = x_{2} \\
\dot{x}_{2} = -\frac{k}{m}x - \frac{h}{m}x_{2} + \frac{1}{m}u \\
y= x
>\end{cases}
>$$
>
> $$
> \begin{align}
> \begin{bmatrix}
>\dot{x}_{1} \\
> \dot{x}_{2}
>\end{bmatrix} = \begin{bmatrix}
>0 & 1 \\
>-\frac{k}{m} & \frac{h}{m}
>\end{bmatrix} + \begin{bmatrix}
>0 \\
>\frac{1}{m}
>\end{bmatrix}u \\
>y = \begin{bmatrix}
1 & 0
\end{bmatrix} \begin{bmatrix}
x_{1} \\
x_{2}
\end{bmatrix}
>\end{align}
>$$
>Pongo $u = \bar{u} : \exists \bar{x}$?