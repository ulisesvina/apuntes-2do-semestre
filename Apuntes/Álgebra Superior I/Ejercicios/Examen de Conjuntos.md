### Ejercicio 1
¿Es cierto que $\{0\} \subseteq \{0, \{0\}\}$? Justifica.

Sí.

Para demostrarlo, supongamos que no lo es, entonces:

1. Recordamos la definición de contención, sean $A,X$ conjuntos tales que $A=\{ 0 \}, X=\{ 0,\{ 0 \} \}$, entonces:
$$
A \subseteq  X \Leftrightarrow \forall a\in A,(a\in X)
$$
2.  Tomemos $0\in A$, notamos que $0\in X$ también, por lo que por definición, $A$ debe ser subconjunto de $X$.

Q.E.D.

---

### Ejercicio 2
Determina cuáles son verdaderas:

a) $\{1\} \in \{1, \{1\}\}$ Verdadera
b) $\{1\} \subseteq \{1, \{1\}\}$  Verdadera
c) $1 \subseteq \{1\}$ Falsa

---

### Ejercicio 3
¿Es cierto que $\{\{a\}\} \subseteq \{a, \{a\}, \{\{a\}\}\}$?

Sí. Para la demostración refiérase al ej. 1 (corolario).

---

### Ejercicio 4
Da un conjunto $X$ con al menos 3 elementos tal que:

$$
\forall x \in X,\ x \subseteq X
$$
$$
X= \{ \varnothing, \{ \varnothing \}, \{\{ \varnothing \} \} \}
$$

---

### Ejercicio 5
Encuentra un conjunto $X$ tal que:

- $X \in X$
- $X \subseteq X$

El conjunto que cumple eso es $X= \{ \varnothing \}$

---

## Parte 2: Contención

### Ejercicio 6
Demuestra que si:

$$
A \subseteq B \quad \text{y} \quad B \subseteq C
$$

entonces:

$$
A \subseteq C
$$

---

### Ejercicio 7
Demuestra que:

$$
A \subseteq B \iff A \cap B = A
$$

---

### Ejercicio 8
Demuestra que:

$$
A \subseteq B \iff A \cup B = B
$$

---

### Ejercicio 9
Si $A \subseteq B$, demuestra que:

$$
A \cap C \subseteq B \cap C
$$

---

### Ejercicio 10
Si $A \subseteq B$, demuestra que:

$$
A \cup C \subseteq B \cup C
$$

---

## Parte 3: Equivalencias

### Ejercicio 11
Demuestra que:

$$
(A \cup B)^c = A^c \cap B^c
$$

---

### Ejercicio 12
Demuestra que:

$$
(A \cap B)^c = A^c \cup B^c
$$

---

### Ejercicio 13
Demuestra que:

$$
A \setminus B = A \cap B^c
$$

---

### Ejercicio 14
Demuestra que:

$$
A \subseteq B \iff A^c \supseteq B^c
$$

---

### Ejercicio 15
Demuestra que:

$$
A \cap (B \cup C) = (A \cap B) \cup (A \cap C)
$$

---

### Ejercicio 16
Demuestra que:

$$
A \cup (B \cap C) = (A \cup B) \cap (A \cup C)
$$

---

## Bonus

### Ejercicio 17
Demuestra que:

$$
A \subseteq B \iff A \setminus B = \varnothing
$$

---

### Ejercicio 18
Demuestra que:

$$
(A \setminus B) \cap B = \varnothing
$$

---

### Ejercicio 19
Demuestra que:

$$
A \subseteq B \iff \mathcal{P}(A) \subseteq \mathcal{P}(B)
$$