**Tema antecesor:** [[Números Complejos]]

## División con resto en $K[x]$
### Observación
$$
K[x]^x = \{ p \in K[x] \mid gi(p) = 0 \}
$$
$$
 = \{  \text{ constantes no nulos} \} = K \setminus \{ 0 \} = K^x
$$

### Proposición 1 (Algoritmo de la División)
Sean $f, g \in K[x] : g\ne 0$ con $f$ dividendo y $g$ divisor
$$
\implies \exists! q,r \in K[x] : \begin{cases}
& f =gq+r & \land  \\
& gr(r) < gr(g)
\end{cases}
$$

#### Demostración
$$
f = \sum a_{i}x^i, g = \sum b_{i}x^i \ne 0
$$
$$
\begin{cases}
 \exists & \text{Sea } n = gr(g) \ge 0 \text{ y sea } m = gr(f) \in \{ -1,0,1, \dots \} \\
& \text{Si } m<n \text{, podemos tomar } q=0, r=f \land f=g:0+f \land gr(f)<gr(g) \\
& \text{Sup. } m\ge n \text{, s.p.g. } m-n\ge 0 \\
& \text{"Inducción" } m-n \text{ sabiendo que la parte de existencia es válida si } m-n<0 \\
& \text{Pie: } m-n=-(m+1), \dots, -1
\end{cases}
$$