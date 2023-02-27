È una condizione necessaria e sufficiente per la stabilità asintotica di un sistema dinamico lineare tempo invariante a TC (Per TD: criterio di jury).

Si basa sulla [[tabella di Routh]] che si costruiisce a partire dal polinomio caratteristico $\Pi(s)$, dalla matrice dinamica $A$ del sistema



>[!def]
>Il sistema dinamico con polinomio caratteristico $\Pi(s)$ è asintoticamente stabile $\iff$ tutti gli elementi della prima colonna della tabella sono concordi e non nulli.
>
>>[!corollario]
>>Se nonci sono elementi nulli in prima colonna il numero di inversioni di segno su quella colonna è pari al numero di radici di $\Pi(s)$ con $Re> 0$

>[!esempio] Esempio 1
> $$
> \Pi (s) = s^4 + 2s^3 + 4s^2 + s + 5
>$$
>
>Tabella di Routh, $n = 4 \implies 5$ righe:
> $$
> \begin{array}{}
>1 & 4 & 5 \\
>2 & 1 & 0 \\
>\alpha
>\end{array} \qquad \begin{align}
> \alpha = \frac{1}{2}\det(\begin{bmatrix}
>1 & 
>\end{bmatrix})
>\end{align}
>$$

