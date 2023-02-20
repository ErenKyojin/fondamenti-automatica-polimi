1. Controllo in anello aperto (AA)
 ![[Controllo in anello aperto.canvas]]

2. Controllo in anello aperto con compensazione del disturbo (supposto misurabile)
	- $Md$ misuratore del disturbo, funziona se $(u,d) \to y$ è esattamente noto
	- $d_{m} = d$

![[Anello aperto con compensazione.canvas]]

3. Controllo in anello chiuso (AC) o in retroazione o feedback
![[Controllo in anello chiuso.canvas]]
Puó contenere disturbi $d$ ed incertezza di modello (legame $(u,d) \to y$ ) non esisattamente noto. Tramite $y_{m}$ o


4. ![[Controllo in anello chius con compensazione.canvas]]
>[!esempio]
> Grafico molla
> 
> 1. modello statico (all'equilibrio)
>    Equilibrio $\implies$ vettore nullo $\implies$ l'attrito è $0 \implies F + F_{att} =0$
>    $$
> \bar{F} - k\bar{y} = 0 \implies \bar{y}= \frac{\bar{F}}{k}
>$$
>Quindi se voglio $y = y^o$ dovró applicare $F = ky^o$
>
>Vediamo cosa succede con un controllo in anello aperto supponendo che $k$ sia uguale ad un certo $k_{n} + \Delta k$
>Applicando $F = k_{n}y^o$ otteró
> $$
> y = \frac{F}{K_{n}+\Delta K} = \frac{k_{n}}{k_{n} + \Delta K}y^o
>$$
>Quindi un errore di modello ($\Delta K$) diventa un errore nel controllo $(y \neq y^o)$


>[!esempio] di controllo in Anello chiuso
> variabile di controllo proporzionale all'errore $\to (y^o - y)$ (convenzione quello che voglio meno quello che ho)
> $$F = \alpha(y^o-y)\quad \alpha > 0$$
> otetengo
> $$y = \frac{F}{l}$$



