**Ej. 2**  
Se resuelve utilizando la fórmula general para ecuaciones de segundo grado ("formulazo").

---

**Ej. 5: Cálculo de Raíces Cuadradas**

**b)** Buscamos $w \in \mathbb{C}$ tal que $w^2 = -5+12i$.  
Sea $w = x+iy$, entonces $(x^2-y^2) + 2xyi = -5+12i$.

Planteamos el sistema de ecuaciones:
$$
\begin{cases}
x^2 - y^2 = -5 & \text{(1)} \\
2xy = 12 & \text{(2)}
\end{cases}
$$

Elevamos al cuadrado ambos lados de (1) y (2):
$$
\begin{cases}
x^4 - 2x^2y^2 + y^4 = 25 & \text{(3)} \\
4x^2y^2 = 144 & \text{(4)}
\end{cases}
$$

Sumamos (3) y (4) para obtener el cuadrado del módulo ($|w|^2$):
$$ x^4 + 2x^2y^2 + y^4 = 169 \implies (x^2+y^2)^2 = 13^2 $$
$$ \implies x^2 + y^2 = 13 \quad \text{(5)} $$

Para hallar $x$ e $y$, operamos con (1) y (5):
*   **Sumando (1) y (5):** $2x^2 = 8 \implies x^2 = 4 \implies x = \pm 2$.
*   **Restando (5) menos (1):** $2y^2 = 18 \implies y^2 = 9 \implies y = \pm 3$.

Como $2xy = 12 > 0$, $x$ e $y$ deben tener el mismo signo.  
$\therefore w_1 = 2+3i$ y $w_2 = -2-3i$.

---

**Ej. 6: Ecuaciones de Segundo Grado con Coeficientes Complejos**

**c)** Buscamos la solución de $z^2 - (4+6i)z + (5-10i) = 0$.  
Aplicamos la fórmula cuadrática:
$$ z = \frac{(4+6i) \pm \sqrt{(4+6i)^2 - 4(1)(5-10i)}}{2(1)} $$

Desarrollamos el discriminante $\Delta$:
$$ \Delta = (16 + 48i - 36) - (20 - 40i) = -20 + 48i - 20 + 40i = -40 + 88i $$

*Nota: Siguiendo el procedimiento del Ej. 5

Buscamos $w = x+yi$ tal que $w^2 = 8i$:
$$
\begin{cases}
x^2 - y^2 = 0 & \text{(1)} \\
2xy = 8 & \text{(2)}
\end{cases}
$$
Usando el método de suma de cuadrados: $x^2 + y^2 = \sqrt{0^2 + 8^2} = 8$.  
De $2x^2 = 8 \implies x = \pm 2$ y $2y^2 = 8 \implies y = \pm 2$.  
Como $2xy > 0$, entonces $w = \pm(2+2i)$.

Regresando a la solución de $z$:
$$ z = \frac{4+6i \pm (2+2i)}{2} $$
$$ z_1 = \frac{6+8i}{2} = 3+4i, \quad z_2 = \frac{2+4i}{2} = 1+2i $$

---

**Ej. 9: Propiedad del Módulo del Cociente**

Demostrar que $\left| \frac{z}{w} \right| = \frac{|z|}{|w|}$ para $w \in \mathbb{C}^\times$.

**Demostración:**  
Sabemos que para todo $w \neq 0$, existe $w^{-1} = \frac{\bar{w}}{|w|^2}$.  
Recordamos que $|z|^2 = z\bar{z}$. Entonces:
$$ \left| \frac{z}{w} \right|^2 = \left( \frac{z}{w} \right) \overline{\left( \frac{z}{w} \right)} $$
Por propiedades del conjugado ($\overline{z/w} = \bar{z}/\bar{w}$):
$$ \left| \frac{z}{w} \right|^2 = \frac{z}{w} \cdot \frac{\bar{z}}{\bar{w}} = \frac{z\bar{z}}{w\bar{w}} = \frac{|z|^2}{|w|^2} $$
Aplicando raíz cuadrada en ambos lados (dado que el módulo es siempre no negativo):
$$ \therefore \left| \frac{z}{w} \right| = \frac{|z|}{|w|} $$

---

**Ej. 15: Identidad de Brahmagupta-Fibonacci**

Sean $m, n \in \mathbb{Z}$ tales que ambos son sumas de dos cuadrados:
$$ m = a^2 + b^2, \quad n = c^2 + d^2 $$

Definimos los complejos $z = a+bi$ y $w = c+di$. Sus normas al cuadrado son:
$$ |z|^2 = a^2 + b^2 = m, \quad |w|^2 = c^2 + d^2 = n $$

Utilizando la propiedad multiplicativa del módulo $|zw| = |z||w|$, tenemos:
$$ mn = |z|^2|w|^2 = |zw|^2 $$

Calculamos el producto $zw$:
$$ zw = (a+bi)(c+di) = (ac-bd) + (ad+bc)i $$

Sustituyendo en la igualdad de las normas:
$$ mn = |(ac-bd) + (ad+bc)i|^2 $$
$$ mn = (ac-bd)^2 + (ad+bc)^2 $$
Esto demuestra que el producto de dos números que son suma de dos cuadrados es, a su vez, una suma de dos cuadrados.

---

**Recordatorio para el examen:**  
Estudiar detalladamente los ejercicios: **2d, 5b, 6c, 9, 10 y 12**.