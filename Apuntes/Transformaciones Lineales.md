## 1. Transformaciones lineales.

**Definición 1.** Sean $V$ y $W$ espacios vectoriales (sobre $\mathbb{R}$). Una función $T: V \rightarrow W$ se le llama **lineal** cuando, para cualquier $\vec{v}, \vec{u} \in V$ y $c \in \mathbb{R}$, tenemos:
1. $T(\vec{u} + \vec{v}) = T(\vec{u}) + T(\vec{v})$
2. $T(c\vec{u}) = cT(\vec{u})$

---

**Ejercicio 1.** Indique cuáles de las siguientes funciones $f: \mathbb{R} \rightarrow \mathbb{R}$ son lineales y por qué.

*   **(a) $f(x) = |x|$**: **No es lineal.** No cumple con la homogeneidad para escalares negativos. Por ejemplo, si $c = -1$ y $x = 1$, $f(-1 \cdot 1) = |-1| = 1$, pero $-1 \cdot f(1) = -1 \cdot |1| = -1$.
*   **(b) $f(x) = x$**: **Es lineal.** Es la función identidad. Cumple $f(x+y) = x+y = f(x)+f(y)$ y $f(cx) = cx = cf(x)$.
*   **(c) $f(x) = 2x + 1$**: **No es lineal.** Aunque es una función afín, no cumple $f(0) = 0$. Notamos que $f(0) = 1 \neq 0$.
*   **(d) $f(x) = x^2$**: **No es lineal.** No cumple la aditividad. Por ejemplo, $f(1+1) = 2^2 = 4$, mientras que $f(1) + f(1) = 1^2 + 1^2 = 2$.
*   **(e) $f(x) = \frac{1}{2}x$**: **Es lineal.** Cumple $f(x+y) = \frac{1}{2}(x+y) = \frac{1}{2}x + \frac{1}{2}y$ y $f(cx) = \frac{1}{2}(cx) = c(\frac{1}{2}x)$.

---

**Ejercicio 2.** Indique cuáles de las siguientes funciones $f: \mathbb{R}^2 \rightarrow \mathbb{R}$ son lineales y por qué.

*   **(a) $f(x,y) = xy$**: **No es lineal.** El producto de variables rompe la linealidad. Por ejemplo, $f(2(1,1)) = f(2,2) = 4$, pero $2f(1,1) = 2(1) = 2$.
*   **(b) $f(x,y) = x + y$**: **Es lineal.** Es una combinación lineal de las componentes. $f(\vec{u}+\vec{v}) = (u_1+v_1) + (u_2+v_2) = (u_1+u_2) + (v_1+v_2) = f(\vec{u}) + f(\vec{v})$.
*   **(c) $f(x,y) = 2x + 3y + 4$**: **No es lineal.** Debido al término constante $+4$, $f(0,0) = 4 \neq 0$.
*   **(d) $f(x,y) = x - y$**: **Es lineal.** Similar al inciso (b), cumple con las dos condiciones de linealidad.
*   **(e) $f(x,y) = 5x$**: **Es lineal.** Puede verse como $f(x,y) = 5x + 0y$, que es una forma lineal estándar.

---

**Ejercicio 3.** Indique cuáles de las siguientes funciones $T: \mathbb{R}^2 \rightarrow \mathbb{R}^2$ son lineales y por qué.

*   **(a) $T(x,y) = (x,y)$**: **Es lineal.** Es la identidad en $\mathbb{R}^2$.
*   **(b) $T(x,y) = (x+y, x-y)$**: **Es lineal.** Cada componente es una combinación lineal de las variables de entrada.
*   **(c) $T(x,y) = (x, xy)$**: **No es lineal.** La segunda componente $xy$ no es lineal como se vio en el Ejercicio 2(a).
*   **(d) $T(x,y) = (1, x)$**: **No es lineal.** $T(0,0) = (1, 0) \neq (0,0)$.
*   **(e) $T(x,y) = (0, 0)$**: **Es lineal.** Es la transformación nula, siempre cumple $T(\vec{u}+\vec{v}) = \vec{0} + \vec{0} = T(\vec{u}) + T(\vec{v})$.

---

**Ejercicio 4.** Indique cuáles de las siguientes funciones $\alpha: \mathbb{R} \rightarrow \mathbb{R}^2$ son lineales y por qué.

*   **(a) $\alpha(t) = (t, t)$**: **Es lineal.** $\alpha(c t_1 + t_2) = (c t_1 + t_2, c t_1 + t_2) = c(t_1, t_1) + (t_2, t_2)$.
*   **(b) $\alpha(t) = (1, t)$**: **No es lineal.** $\alpha(0) = (1, 0) \neq (0, 0)$.
*   **(c) $\alpha(t) = (3t, 5t)$**: **Es lineal.** Sigue la forma $\alpha(t) = t \vec{v}$ con $\vec{v} = (3, 5)$.
*   **(d) $\alpha(t) = (2t, t+1)$**: **No es lineal.** Debido al $+1$, $\alpha(0) = (0, 1)$.
*   **(e) $\alpha(t) = (t, t^3)$**: **No es lineal.** El término $t^3$ no cumple con la homogeneidad: $\alpha(2t) = (2t, 8t^3) \neq 2\alpha(t) = (2t, 2t^3)$.