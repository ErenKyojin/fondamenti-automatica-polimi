lINEARIZZAZIONE DI sdnl [[SISO]], TC, nell'interno di un equilibrio

Consideriamo un SD NL (TI)
$$
S:\begin{cases}
\dot{x} = f(x,u) \\
y = g(x,u)
\end{cases}
$$
ed un suo equilibrio $(\bar{u},\bar{x},\bar{y})$

Vogliamo determinare un sistema lineare che approssima il comportamento di $S$ nell'intorno dell'equilibrio fintanto che $u(t), x(t), y(t)$ non si discostano troppo da $\bar{u},\bar{x},\bar{y}$ rispettivamente

Consideriamo l'equazione di stato, e sviluppiamola in serie fermandoci al primo ordine:
$$
f(\bar{x} + \delta x, \bar{u} + \delta u) = f(\bar{x},\bar{u}) + f_{x}\bigg|_{\bar{x},\bar{u}} \delta x + f_{u}|
$$
Con i $\delta$ variazioni di $x$ e $u$ rispetto all'equilibrio