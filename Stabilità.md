Si può applicare il concetto a [[Equilibrio|equilibri]], (movimenti) e qualche volta a [[sistemi]]:
 - Stabilità di un equilibrio (tempo continuo)
	 Sia $\bar{x}$ uno stato di equilibrio del sistema dinamico $\dot{x} = f(x,u) \dot{c}$ per $u = \bar{u}$ costante
	 
	- Equilibrio stabile $$\forall \varepsilon > 0 \exists \delta > 0 | \lvert x(0) - \bar{x} \rvert < \delta \implies \lvert x(t) - \bar{x} \rvert < \varepsilon \quad\forall t > 0$$
	  Interpretazione grafica:
```tikz
\begin{document}
\begin{tikzpicture}[scale = 2]
\draw[->](0,0) -- (5,0);
\draw[->] (0,0) -- (0,2);
\draw[blue] (0,1)node[left]{$\bar{x} $} -- (5,1);
\draw[red] (0,1.5) node[left]{$\bar{x}+ \varepsilon$} -- (5,1.5);
\draw[red] (0,.5) node[left]{$\bar{x}- \varepsilon$} -- (5,.5); 
\end{tikzpicture}
\end{document}
```
fino a  quanod
- 
	  
	  
