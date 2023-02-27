Si può applicare il concetto a [[Equilibrio|equilibri]], (movimenti) e qualche volta a [[sistemi]]:
 - Stabilità di un equilibrio (tempo continuo)
	 Sia $\bar{x}$ uno stato di equilibrio del sistema dinamico $\dot{x} = f(x,u) \dot{c}$ per $u = \bar{u}$ costante
	 
	- Equilibrio stabile (S)$$\forall \varepsilon > 0 \exists \delta > 0 | \lvert x(0) - \bar{x} \rvert < \delta \implies \lvert x(t) - \bar{x} \rvert < \varepsilon \quad\forall t > 0$$
	  Interpretazione grafica, giallo è stabile, verde no (ogni linea rappresenta un movimento):
	```tikz
	\begin{document}
	\begin{tikzpicture}[scale = 2]
	\draw[->](0,0) -- (5,0);
	\draw[->] (0,0) -- (0,2);
	\draw[blue] (0,1)node[left]{$\bar{x} $} -- (5,1);
	\draw[red] (0,1.5) node[left]{$\bar{x}+ \varepsilon$} -- (5,1.5);
	\draw[red] (0,.5) node[left]{$\bar{x}- \varepsilon$} -- (5,.5); 
	\draw[yellow] (0,1) -- (2,1.4) -- (4,.6) -- (4.5,1.1) -- (5,.9);
	\draw[green] (0,1.5) -- (1,-.4) -- (2, .8) -- (5, .9);
	\end{tikzpicture}
	\end{document}
	```
	- Equilibrio asintoticamente stabile (AS)
	  Vuol dire che:
		  - Equilibrio stabile
		  -  $\lvert \lvert x(t) - \bar{x} \rvert \rvert \to 0$ per $t \to \infty$
	-  Equilibrio  instabile (I) altrimenti



## Stabilita nei [[sistemi dinamici LTI]] (STC)
$\dot{x} = Ax + bu$
Sia $\bar{x}$ uno stato di equilibrio per $u = \bar{u}$ costante, allora
$$
\begin{rcases}
x(t) = \bar{x} \\
u(t) = \bar{u}
\end{rcases} \to x(t) = \bar{x} \quad t \geq 0
$$
E quindi
$$
e^{At} x(0) + \int_{0}^t e^{A(t-\tau)} bu(\tau) \, d\tau 
$$