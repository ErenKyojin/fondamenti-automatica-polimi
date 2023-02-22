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
>$u(t) $ 


```tikz
\pgfplotsset{compat=1.1}
\begin{document}
\begin{tikzpicture}
\draw(0,0) -- (1,1);
\end{tikzpicture}
\end{document}
```=