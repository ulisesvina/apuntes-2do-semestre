**Ej. 2** Se resuelve a formulazo

**Ej. 5**: 
b) Buscamos $w \in \mathbb{C} : w^2 = -5+12i$

$$
(x^2-y^2)+2xyi=-5+12i
$$
Planteamos como sistema de ecuaciones
$$
\begin{cases}
& x^2-y^2 = -5 & \text{ (1)} \\
& 2xy = 12 & \text{ (2)}
\end{cases}
$$
Elevamos al cuadrado (1) y (2)
$$
\begin{cases}
& x^4 - 2x^2y^2+y^4 = 25 & \text{ (3)} \\
& 4x^2y^2 = 144 & \text{ (4)}
\end{cases}
$$
Sumamos (3) y (4)
$$
x^4+2x^2y^2+y^4 = 169
$$
$$
 \implies (x^2+y^2)^2 = 13^2
$$
$$
\implies x^2+y^2 = 13 \text{ (5)}
$$
Sumamos (1) y (5)
$$
2x^2 = 8
$$
$$
x^2 = 4
$$
$$
 x = \pm 2
$$
Restamos (5) y (1)
$$
2y^2 = 18
$$
$$
 y= \pm 3
$$
**Ej. 6**
c) Buscamos la solución de $z^2 = (4+6i)z - (5-10i) = 0$

$$
 z = \frac{4+6i\pm \sqrt{ (4+6i)^2 + 4(1)(5-10i) }}{2(1)}
$$
$$
= \frac{4+6i \pm \sqrt{ 48i-40i }}{2}
$$
$$
= \frac{4+6i \pm \sqrt{ 8i }^2}{2}
$$
$$
 = \frac{4+6i \pm (2+2i)}{2}
$$
Aplicamos lo del ej. 5:

Buscamos una $w=x+yi : w^2 = 8i$
$$
(x^2-y^2) + 2xyi = 8i
$$
$$
\begin{cases}
& x^2-y^2 = 0 & \text{ (1)} \\
& 2xy = 8 & \text{ (2)}
\end{cases}
$$
$$
\begin{cases}
& x^4 - 2x^2y^2+y^4 =0 \\
& 4x^2y^2 = 64
\end{cases}
$$
$$
x^2+y^2 = 8
$$

$$
 2x^2 = 8
$$
$$
  2y^2=8
$$

$$
 x= \pm 2
$$$$
 y= \pm 2
$$


$$
 w_{1} = 2+2i
$$
$$
w_{2} = -2-2i
$$

**Ej. 9**
Demostrar que $|\frac{z}{w}| = \frac{|z|}{|w|}$ si $w \in \mathbb{C}^\times$ (nota: $\mathbb{C}^\times = \mathbb{C} \setminus \{ 0 \}$)

Sabemos que $\exists w^{-1} \in \mathbb{C} : ww^{-1}  = 1$

$$
\overline{ww^{-1}} = \overline{1} = 1
$$
$$
 \implies \frac{1}{\overline{w} } = \overline{w^{-1}}
$$
$$
 w \ne 0
$$

$$
\left|\frac{z}{w}\right|^2 = \frac{\left|z\right|^2}{\left|w\right|^2}
$$
$$
\left|\frac{z}{w}\right|^2 = \frac{z}{w} \frac{\overline{z}}{w}
$$
$$
 = \frac{z}{w}\frac{\overline{z}}{\overline{w}}
$$
$$
 \therefore \left|\frac{z}{w}\right|^2 = \frac{\left|z\right|^2}{\left|w\right|^2}
$$
$$
\therefore \left|\frac{z}{w}\right| = \frac{\left|z\right|}{\left|w\right|}
$$
**Ej. 15**
Sean $m,n \in \mathbb{Z}$ dos sumas de cuadrados
$$
 m = a^2+b^2
$$
$$
 n = c^2+d^2
$$
$$
z = a+bi
$$
$$
w = c+di
$$
$$
|z|^2 = a^2+b^2 = m
$$
$$
|w|^2 = c^2+d^2 = n
$$
$$
mn = |z|^2|w|^2
$$
$$
 = |zw|^2
$$
$$
 = |(ac-bd)+(ad+bc)i|
$$
$$
= |(ai-bd)^2+(ad+bc)^2
$$
Estudiar para el examen 2d, 5b, 6c, 9, 10 y 12