Se genera por una línea recta que pasa por una curva fija y por un punto fijo. El punto no está contenido en el plano de la curva. La recta móvil se llama generatriz y la curva fija se llama directriz, el punto fijo se llama vértice.

La ecuación de la directriz está dada por:
$$
\overline{P} = \overline{P}_{0} + t(\overline{P}\prime - \overline{P}_{0})
$$

$$
(x,y,z) = \left(x_{0},y_{0},z_{0}\right) + t\left((x\prime,y\prime,z\prime) - (x_{0},y_{0},z_{0})\right)
$$
$$
\frac{x-x_{0}}{x\prime-x_{0}} = \frac{y-y_{0}}{y\prime - y_{0}} = \frac{z-z_{0}}{z\prime-z_{0}}
$$
---
$$
x=x_{0}+t(x\prime-x_{0})
$$
$$
y=y_{0}+t(y\prime-y_{0})
$$
$$
z=z_{0}+t(z\prime-z_{0})
$$
---
Hallar la ecuación de la superficie cónica cuya directriz es la elipse $5x^2+2z^2=1$ y está sobre el plano $y=3$. El vértice no puede estar sobre el plano, está sobre $(2,1,1)$

$$
\implies (x,y,z) = (2,1,1)+t((x\prime,y\prime,z\prime)-(2,1,1))
$$
$$
\implies \frac{x-2}{x\prime-2} = \frac{y-1}{y\prime-1} = \frac{z-1}{z\prime-1}
$$
Sustituyendo:
$$
\frac{x-2}{x\prime-2} = \frac{y-1}{2}
$$
$$
\frac{z-1}{z\prime-1} = \frac{y-1}{2}
$$
Despejando:
$$
5\left(\frac{2(x-2)}{y-1} +2 \right) + 2\left(\frac{z(z-1)(y-1)}{y-1}+1\right) = 1
$$
$$
\implies 5\left(2(x-2)+2(y-1)\right)^2 + 2\left(2(z-1)+(y-1)\right)^2 = (y-1)^2
$$
$$
\implies 20x^2+21y^2+8z^2 + 40xy + 8yz + -120x + -130y + 8z + 197 = 0
$$
---

**Elipse:** $2x^2 + 6y^2 =1$
**Plano:** $z=5$
**Vértice:** $(2,3,1)$

Sustituyendo:
$$
\frac{x-2}{x\prime-2} = \frac{y-3}{y\prime-3} = \frac{z-1}{z\prime-1}
$$
$$
\implies \frac{x-2}{x\prime-2} = \frac{z-1}{4}
$$
$$
\implies \frac{y-3}{y\prime-3} = \frac{z-1}{4}
$$
Despejando:
$$
2\left(\frac{}{z-1} + 2\right)^2 + 6\left(\frac{}{z-1} + 3\right)^2 = 1
$$