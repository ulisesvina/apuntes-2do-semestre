# Anillos

## Propiedades básicas de las operaciones en $\mathbb{Z}$

**Definición:** $\mathbb{Z} = \{\pm n \mid n \in \mathbb{N}\}$ con $0 \in \mathbb{N}$

**Operaciones:** Suma y producto (operaciones binarias, es decir, se aplica solo a parejas).

Las operaciones son funciones tales que $+: \mathbb{Z} \times \mathbb{Z} \to \mathbb{Z}$ y $\cdot: \mathbb{Z} \times \mathbb{Z} \to \mathbb{Z}$. Esto quiere decir que a las parejas $(a,b) \in \mathbb{Z}$ se les asocia $a+b$ y $a \cdot b$ respectivamente.

### Propiedades Fundamentales de las Operaciones

1. La suma es asociativa:
$$a+(b+c) = (a+b)+c \quad \forall a,b,c \in \mathbb{Z}$$

2. Existe un entero neutro aditivo:
$$\forall a \in \mathbb{Z}\ \exists\, b \in \mathbb{Z} : a + b = a \implies b = 0$$

3. Existe un inverso aditivo:
$$\forall a \in \mathbb{Z}\ \exists\, {-a} : a + (-a) = 0$$

4. La suma es conmutativa:
$$a+b=b+a \quad \forall a,b \in \mathbb{Z}$$

Considerando las propiedades 1–3, se cumple que $(\mathbb{Z}, +)$ es un **grupo**, y considerando también la propiedad 4, se cumple que $(\mathbb{Z}, +)$ es un **grupo abeliano**.

5. El producto es asociativo:
$$a \cdot (b \cdot c) = (a \cdot b) \cdot c \quad \forall a,b,c \in \mathbb{Z}$$

6. Existe un entero neutro multiplicativo:
$$\forall a \in \mathbb{Z}\ \exists\, b \in \mathbb{Z} : ab = a \implies b = 1$$

7. El producto es conmutativo:
$$ab = ba \quad \forall a,b \in \mathbb{Z}$$

8. El producto distribuye a la suma:
$$a\cdot(b+c) = ab+ac \quad \forall a,b,c \in \mathbb{Z}$$

Estas propiedades (5 y 6) nos dicen que $(\mathbb{Z}, \cdot)$ es un **monoide**, y si además consideramos la propiedad 7 se dice que $(\mathbb{Z}, \cdot)$ es un **monoide conmutativo**.

Todas juntas nos dicen que $(\mathbb{Z}, +, \cdot)$ es un **anillo conmutativo con unidad**.

---

## Anillos Conmutativos con Unidad

### Definición de operación binaria

Sea $A$ un conjunto. Una **operación binaria** en $A$ es cualquier función:
$$\cdot\, : A \times A \to A, \quad (a, a') \mapsto a \cdot a'$$

### Axiomas de un Anillo Conmutativo con Unidad

Sea $A$ cualquier conjunto con dos operaciones binarias:
$$+: A\times A \to A, \qquad *: A\times A \to A$$

#### Axioma 1 — Asociatividad de la suma
$$a+(b+c) = (a+b)+c \quad \forall\, a,b,c \in A$$

#### Axioma 2 — Neutro aditivo
Existe un elemento neutro aditivo en $A$:
$$\exists\, 0 \in A : a+0 = a = 0+a \quad \forall\, a \in A$$

> **Lema:** El neutro aditivo es necesariamente único.
>
> **Demostración 1** (requiere Axioma 3):
> 1. Sean $0, 0'$ neutros aditivos $\forall\, a \in A$.
> 2. Supongamos $0 \ne 0'$.
> 3. Al ambos ser neutros aditivos, tenemos $a+0 = a+0' = a$.
> 4. Sumamos el inverso aditivo de $a$ a ambos términos: $(-a)+(a+0) = (-a)+(a+0')$.
> 5. Por Axioma 1: $\bigl((-a)+a\bigr)+0 = \bigl((-a)+a\bigr)+0' \implies 0 = 0'\ \text{ ❗️}$
> 6. Debe cumplirse necesariamente $0 = 0'$. $\square$
>
> **Demostración 2:**
> 1. Sean $0, 0'$ neutros aditivos $\forall\, a \in A$.
> 2. Supongamos $0 \ne 0'$.
> 3. Tenemos $0' = 0 + 0' = 0\ \text{ ❗️}$
> 4. Debe cumplirse necesariamente $0 = 0'$. $\square$

#### Axioma 3 — Inverso aditivo
Todo $a \in A$ tiene un inverso aditivo en $A$:
$$\forall\, a \in A\ \exists\, (-a) \in A : a + (-a) = 0$$

> **Proposición 1 — Leyes de cancelación aditiva**
>
> Gracias a los Axiomas 1–3:
> 1. $a+b = a+c \implies b = c$
> 2. $b+a = c+a \implies b = c$
>
> **Demostración:**
> 1. Supongamos $a+b = a+c$.
> 2. Sea $d$ el inverso aditivo de $a$.
> 3. Sumamos $d$ a ambos términos: $d+(a+b) = d+(a+c)$.
> 4. Por Axioma 1: $(d+a)+b = (d+a)+c \implies 0+b = 0+c \implies b = c$. $\square$

> **Lema:** Por la Proposición 1, el inverso aditivo $b$ de cada $a \in A$ es único. Si $b'$ es otro inverso, entonces $a+b' = 0 = a+b \implies b' = b$. En consecuencia, podemos denotar por $-a \in A$ al único inverso aditivo de $a$.

#### Axioma 4 — Conmutatividad de la suma
$$a+b = b+a \quad \forall\, a,b \in A$$

#### Axioma 5 — Asociatividad del producto
$$a(bc) = (ab)c \quad \forall\, a,b,c \in A$$

#### Axioma 6 — Neutro multiplicativo
Existe un neutro multiplicativo distinto de cero:
$$\exists\, 1 \in A \setminus \{0\} : a \cdot 1 = a \quad \forall\, a \in A$$

> **Observación:** El neutro multiplicativo del Axioma 6 es único (la demostración es análoga a la del neutro aditivo).

#### Axioma 7 — Conmutatividad del producto
$$ab = ba \quad \forall\, a,b \in A$$

#### Axioma 8 — Distributividad
El producto distribuye a la suma:
$$a(b+c) = ab+ac \quad \forall\, a,b,c \in A$$

---

### Definición de ACU

Sea un conjunto $A$ junto con dos operaciones binarias. La terna $(A, +, \cdot)$ es un **anillo conmutativo con unidad (ACU)** si valen los Axiomas 1–8, es decir:
- $(A, +)$ es un **grupo abeliano**,
- $(A, \cdot)$ es un **monoide conmutativo**.

### Ejemplos

1. Con las operaciones usuales de suma y producto, $(A, +, \cdot)$ es ACU para $A \in \{\mathbb{Z},\, \mathbb{Q},\, \mathbb{R},\, \mathbb{C},\, \mathbb{R}[x]\}$.

2. $A = \{a, b\}$ con las tablas:

| $+$ | $a$ | $b$ |
|-----|-----|-----|
| $a$ | $a$ | $b$ |
| $b$ | $b$ | $a$ |

| $\cdot$ | $a$ | $b$ |
|---------|-----|-----|
| $a$     | $a$ | $a$ |
| $b$     | $a$ | $b$ |

---

## ACU Ordenados — Axiomas de Orden e Inducción

Para definir un **ACU ordenado** (como $\mathbb{Z}$, $\mathbb{Q}$ o $\mathbb{R}$) se añaden cuatro axiomas adicionales sobre un subconjunto distinguido de **elementos positivos** $A^{+} \subseteq A$.

#### Axioma 9 — Cerradura aditiva de los positivos
$$a, b \in A^{+} \implies a + b \in A^{+}$$

Es decir, $A^{+}$ es cerrado bajo la suma.

#### Axioma 10 — Cerradura multiplicativa de los positivos
$$a, b \in A^{+} \implies a \cdot b \in A^{+}$$

Es decir, $A^{+}$ es cerrado bajo el producto.

#### Axioma 11 — Tricotomía (Principio de orden total)
Para todo $a \in A$, se cumple **una y solo una** de las siguientes:
$$a \in A^{+}, \qquad a = 0, \qquad -a \in A^{+}$$

Este axioma nos permite definir la relación de orden estricto: $a > b \iff a - b \in A^{+}$.

#### Axioma 12 — Principio de Inducción Matemática
Sea $A = \mathbb{Z}$ (o un subanillo bien ordenado). Si $S \subseteq \mathbb{N}$ satisface:
1. **Base:** $0 \in S$ (o $1 \in S$),
2. **Paso inductivo:** $n \in S \implies n+1 \in S$,

entonces $S = \mathbb{N}$.

> **Formulación equivalente (Principio de Inducción Fuerte):** Si $S \subseteq \mathbb{N}$ satisface la base y, para todo $n$, $\{0, 1, \ldots, n\} \subseteq S \implies n+1 \in S$, entonces $S = \mathbb{N}$.

> **Nota:** En $\mathbb{Z}$, el Axioma 12 garantiza que todo subconjunto no vacío de $\mathbb{N}$ tiene un **mínimo** (principio del buen orden), lo que es equivalente a la inducción.

---

## Proposiciones sobre el Orden

### Proposición 1 — Propiedades de la relación $>$

1. **(Transitividad)** $a > b$ y $b > c \implies a > c$
2. **(Irreflexividad)** $a \not> a$
3. **(Asimetría)** $a > b \implies b \not> a$

**Demostración:**

1. Suponemos $a > b$ y $b > c$, es decir, $a-b \in A^{+}$ y $b-c \in A^{+}$.
$$\therefore\; (a-b)+(b-c) = a-c \in A^{+} \quad \text{(Ax. 9)} \implies a > c. \qquad \square$$

2. Si $a > a \implies a-a = 0 \in A^{+}$, lo que contradice el Axioma 11. $\square$

3. Supongamos $a > b$, es decir, $a - b \in A^{+}$. Si además $b > a$, entonces $b - a = -(a-b) \in A^{+}$, contradiciendo el Axioma 11 (pues $a-b \ne 0$). $\square$

---

### Proposición 2 — Tricotomía para el orden

Si $a, b \in A$, por el Axioma 11 se cumple una y solo una de:
$$a > b, \qquad a = b, \qquad a < b$$

En particular, si $a \in A$, vale una y solo una de:
$$a > 0, \qquad a = 0, \qquad a < 0$$

---

### Proposición 3 — Monotonía de la suma

$$a > b \implies a + c > b + c$$

**Demostración:**
1. Supongamos $a > b$, es decir, $a - b \in A^{+}$.
2. $(a+c)-(b+c) = a - b \in A^{+}$.
3. $\therefore\; a + c > b + c$. $\square$

---

### Proposición 4 — Monotonía del producto por positivos

$$a > b \;\land\; c > 0 \implies ac > bc$$

**Demostración:**
1. Suponemos $a > b$ y $c > 0$, es decir, $a - b \in A^{+}$ y $c \in A^{+}$.
2. Por Axioma 10: $(a-b)\cdot c \in A^{+}$.
3. $(a-b)\cdot c = ac - bc \in A^{+}$.
4. $\therefore\; ac > bc$. $\square$

> **Lema:** $a > b \implies -b > -a$. ⭐️

---

### Proposición 5 — Inversión del orden al multiplicar por negativos

$$a > b \;\land\; c < 0 \implies ac < bc \tag{⭐️}$$

**Demostración:**
1. Suponemos $a > b$ y $c < 0$, es decir, $a - b \in A^{+}$ y $-c \in A^{+}$.
2. Por Axioma 10: $(a-b)(-c) \in A^{+}$.
3. $(a-b)(-c) = bc - ac \in A^{+}$.
4. $\therefore\; bc > ac$, es decir, $ac < bc$. $\square$

#### Corolario — Signo del producto

Sean $a, b \in A$:

| Hipótesis | Conclusión |
|-----------|-----------|
| $a > 0$ y $b > 0$ | $ab > 0$ (Prop. 4) |
| $a > 0$ y $b < 0$ | $ab < 0$ (Prop. 5) |
| $a < 0$ y $b > 0$ | $ab < 0$ (Prop. 5) |
| $a < 0$ y $b < 0$ | $ab > 0$ (Prop. 5) |

---

### Proposición 6 — Los cuadrados son positivos

$$a \ne 0 \implies a^2 > 0$$

En particular, $1 = 1^2 > 0$.

**Demostración:** ⭐️

Por Axioma 11, $a \ne 0$ implica $a \in A^{+}$ o $-a \in A^{+}$.
- Si $a \in A^{+}$: $a^2 = a \cdot a \in A^{+}$ por Axioma 10.
- Si $-a \in A^{+}$: $a^2 = (-a)(-a) \in A^{+}$ por Axioma 10.

En ambos casos $a^2 \in A^{+}$, es decir, $a^2 > 0$. $\square$

---

### Proposición 7 — Multiplicación por un factor mayor que 1

$$a > 0 \;\land\; b > 1 \implies ab > a$$

**Demostración:**
1. $ab - a = a(b-1)$ con $a \in A^{+}$ y $(b-1) \in A^{+}$.
2. Por Axioma 10: $a(b-1) \in A^{+}$.
3. $\therefore\; ab > a$. $\square$

---

> **Lema 3:** $a, b \in A^{\times} \implies ab \in A^{\times}$
>
> (El producto de unidades es una unidad, donde $A^{\times}$ denota el conjunto de unidades de $A$.)

