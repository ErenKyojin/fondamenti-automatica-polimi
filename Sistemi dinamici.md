![[Sistemi dinamici.canvas]]
Se conosco $u(t)$ sull'intervallo $[t_{0},t]$ queso mi basta per conoscere $y(t)$ su $[t_{0},t]$

- Si $\implies$ sistema **non dinamico**
- No $\implies$ sistema **dinamico**

>[!esempio] Esempio 1
> ![[Untitled.canvas]]
> $y(t) = \frac{1}{R}v(t)$
> Quindi $u(t)$ su $[t_{0},t] \implies$ noto $y(t)$ su $[t_{0},t]$ quindi il sistema non è dinamico
> 
>
>


>[!esempio] Esempio 2
>
>Circuito RC
>Per conoscere $y(t)$ su $[t_{0},t]$ mi ocorrono $u(t)$ su $[t_{0},t]$ e la condizione iniziale $y(t_{0})$ tensione iniziale sul condensatore. Sistema dinamico.

>[!esempio] Esempio 3
>Sistema massa molla
>
>Per conoscere $y([t_{0},t])$ mi occorrono $u([t_{0},t])$ oltre posizione e velocità iniziali
>
>>[!oss]
>>I parametri fisici non sono variabili e si considerano noti

>[!esempio] Esempio 4
>Fermate di un tram
>$0,\dots,N$ con l'indice $k$ che conta le fermate
>$u(k) =$ numero di passaggeri saliti - passeggeri scesi alla fermata k
>$y(k) =$ numero di passeggeri a bordo quando si lascia la fermata $k$
>è necessario conoscere le condizioni iniziali $y(k_{0})$ e $u[k_{0},k]$, quindi è un sistema dinamico

>[!esempio] Esempio 5
>Nastro trasportatore su cui una tramoggia deposita polvere
>
>$u(t) \quad [\frac{kg}{s}]$
>$y(t)$ portata d'uscita 
>
>$y(t) = u(t) - \tau$ con $\tau$ tempo di trasporto
>Per conoscere $y$ da $[t_{0},t]$ occorono $u([t_{0},t])$ e $y([t_{0}-\tau,t_{0}])$ 
>Per l'esattezza $u[t_{0},t - \tau]$
>

>[!esempio] Esempio 6
>Lampada con un pulsante
>Il pulsante accende o spegne in base allo stato, per conoscere l'andamento dell'accensione $y(t)$ su $[t_{0},t]$ occore conoscere l'ingresso, ossia gli istanti di rilascio del pulsante entro $[t_{0},t]$ e lo stato di accensione iniziale a $t_{0}$ (che è un booleano). Si tratta di un sistema dinamico
>
>>[!oss]
>> ```tikz
>>\begin{document}
>>\begin{tikzpicture}
>>\draw (-1.5,0) --(-1,0) -- (-1,1) -- (0,1) -- (0,0) -- (1,0) -- (1,1) -- (1.2,1) -- (1.2,0);
>>\end{tikzpicture}
>>\end{document}
>>```
>>Se gli istanti di rilascio sono l'ingresso è equivalente
>
>>[!oss]
>>Se non interessa tutta $y([t_{0},t])$ ma soltanto $y(t)$ l'informazione che occorre è $y(t_{0})$ ed il fatto che il numero di rilasci sia pari o dispari


Al momento ci specializziamo in 2 classi di sistemi dinamici ma l'idea è molto piú generale di esse

# Sistema dinamico (SD) a tempo continuo (TC)
La quantità di cui occorre conoscere il valore iniziale per poter conoscere l'uscita noto l'ingresso ed ovviamente i parametri del sistema. Si dicono **variabili di stato** e tradizionalmente si indicano con $x$, un certo $x(t_{0})$  ed un certo $u([t_{0},t])$

quindi
$$
\begin{rcases}
x(t_{0}) \\
u[t_{0},t]
\end{rcases}\rightarrow  x(t), y(t) \text{ su }[t_{0},t]\quad t \in \mathbb{R}
$$

($u$ ingresso, $x$ stato, $y$ uscita)

Consideriamo **quasi** sempre sistemi dinamici con un solo ingresso ed una sola uscita, detti anche single input single output
![[SISO]] 

## Espressione del sistema
$$\begin{align}
x_{1}(t) = \phi_{1}(x_{1}(t_{0}),x_{2}(t_{0}),\dots ,x_{n}(t_{0}),u[t_{0},t],t) \\ 
\dots \\
x_{n}(t) = \phi_{1}(x_{1}(t_{0}),x_{2}(t_{0}),\dots ,x_{n}(t_{0}),u[t_{0},t],t)
\end{align}$$