## Anillos
### Propiedades básicas de las operaciones en $\mathbb{Z}$

**Definición:** $\mathbb{Z} = \{\pm n \mid n \in \mathbb{N}\}$ con $0 \in \mathbb{N}$
**Operaciones:** Suma y producto (operaciones binarias, es decir, se aplica solo a parejas).

Las operaciones son funciones tales que $+: \mathbb{Z} \times \mathbb{Z} \to \mathbb{Z}$ y $\cdot: \mathbb{Z} \times \mathbb{Z} \to \mathbb{Z}$. Esto quiere decir que a las parejas $(a,b) \in \mathbb{Z}$ se les asocia $a+b$ y $a \cdot b$ respectivamente.

### Propiedades Fundamentales de las Operaciones
1. La suma es asociativa
   $a+(b+c) = (a+b)+c \forall a,b,c \in \mathbb{Z}$
2. Existe un entero neutro aditivo
   $\forall a \in \mathbb{Z} \exists b \in \mathbb{Z} : a + b = a \implies b = 0$
3. Existe un inverso aditivo
   $\forall a \in \mathbb{Z} \exists -a : a + -a = 0$
4. La suma es conmutativa
   $a+b=b+a \forall a,b \in \mathbb{Z}$
 
Considerando las propiedades 1-3, se cumple que $(\mathbb{Z}, +)$ es un grupo, y considerando también la propiedad 4, se cumple que $(\mathbb{Z}, +)$ es un grupo abeliano.

5. El producto es asociativo
   $a \cdot (bc) = (ab) \cdot c \forall a,b,c \in \mathbb{Z}$
6. Existe un entero neutro multiplicativo
   $\forall a \in \mathbb{Z} \exists b \in \mathbb{Z} : ab = a \implies b = 1$
7. El producto es conmutativo
   $ab = ba \forall a,b \in \mathbb{Z}$
8. El producto distribuye a la suma
   $a\cdot(b+c) = ab+ac \forall a,b,c \in \mathbb{Z}$

Estas propiedades (5 y 6) nos dicen que $(\mathbb{Z}, \cdot)$ es un monoide, y si además consideramos la propiedad 7 se dice que $(\mathbb{Z}, \cdot)$ es un monoide conmutativo.

Todas juntas nos dicen que $(\mathbb{Z}, +, \cdot)$ es un anillo conmutativo con unidad.
## Anillos Conmutativos con Unidad
### Definición
Sea A un conjunto, una operación binaria en A es cualquier función
$$\cdot: A \times A \to A = (a,a\prime) \rightarrowtail a \cdot a\prime$$

---
Sea A cualquier conjunto y consideramos dos operaciones binarias

$$
 +: A\times A \to A, *: A\times A \to A
$$

Interesa el caso en el que se cumplen los axiomas:

### Axioma 1
La suma es asociativa 
$$a+(b+c) = (a+b)+c \forall a,b,c \in A$$

### Axioma 2
Existe un elemento neutro aditivo en $A$. 
$$\exists c \in A : a+c = a = c+a \forall a \in A$$
#### Lema
El neutro aditivo es necesariamente único.

**Demostración 1 (se require axioma 3):**
1. Sean $c, c\prime$ neutros aditivos $\forall a \in A$
2. Supongamos $c \ne c\prime$
3. Al ambos ser neutros aditivos, tenemos $a+c=a+c\prime = a$
4. Sumamos el inverso aditivo de $a$ a ambos términos: $-a+(a+c) = -a+(a+c\prime)$
5. Por axioma 1, nos queda $(-a+a)+c = (-a+a)+c\prime \implies c=c\prime \text{ !}$
6. Debe cumplirse necesariamente $c = c\prime$ Q.E.D.

**Demostración 2:**
1. Sean $c, c\prime$ neutros aditivos $\forall a \in A$
2. Supongamos $c \ne c\prime$
3. Tenemos $c\prime = c + c\prime = c \text{ !}$
4. Debe cumplirse necesariamente $c = c\prime$ Q.E.D.
 
### Axioma 3
Todo $a \in A$ tiene un inverso aditivo (en $A$).

### Proposición 1
Gracias a los axiomas 1-3 tenemos las **leyes de cancelación aditiva**.

1. $a+b = a+c \implies b=c$
2. $b+a = b+c \implies b=c$

**Demostración**
1. Supongamos $a+b = a+c$
2. Sea $d$ el inverso aditivo de $a$.
3. Sumamos $d$ a ambos términos, entonces $d+(a+b)=d+(a+c)$
4. Por axioma 1, tenemos $(d+a)+b = (d+a)+c \implies 0+b=0+c = b+c$ Q.E.D.

#### Lema
Por proposición 1, el inverso aditivo $b$ de cada $a \in A$ es único si $b\prime$ es otro, $a+b\prime = 0 = a+b$
$\therefore b\prime = b$. En consecuencia, podemos denotar por $-a \in A$ al único inverso aditivo.

### Axioma 4
La suma es conmutativa

$$
a+b=b+a \forall a,b \in A
$$
### Axioma 5
El producto es asociativo

$$
 a(bc) = (ab)c \forall a,b,c\in A
$$
### Axioma 6
Existe un neutro multiplicativo distinto de cero

$$
\forall a \in A \exists u \in A \setminus \{ 0 \} : a\cdot u = a
$$
#### Observación
El neutro multiplicativo del axioma 6 es único

### Axioma 7
El producto es conmutativo

$$
ab=ba \forall a,b \in A
$$
### Axioma 8
El producto distribuye a la suma

$$
 a(b+c) = ab+ac \forall a,b,c \in A
$$


---
## Anillos Conmutativos con Unidad
### Definición
Sea un conjunto $A$, junto con un dos operaciones binarias en él $(A,+,\cdot)$ es un __anillo conmutativo con unidad (ACU)__ si para $(A,+,\cdot)$ valen los axiomas 1-8 ($(A,+)$ es un grupo abeliano y $(A, \cdot)$ es un monoide conmutativo)

### Ejemplos
1. Con las operaciones usuales de suma y producto $+, \cdot; (A, +, \cdot)$ es ACU donde $A$ es cualquiera de $\mathbb{Z}, \mathbb{Q}, \mathbb{R}, \mathbb{C}, \mathbb{R}[x]$
2. $A = \{ a,b \}$

| +   | a   | b   |
| --- | --- | --- |
|  a   | a   | b   |
| b   | b   | a   |

| $\cdot$ | a   | b   |
| ------- | --- | --- |
| a       | a   | a   |
| b       | a   | b   |

---
### Proposición 1

1. $a>b>c \implies a>c$ (es transitiva)
2. $a \not\gt a$ (es irreflexiva)
3. $a > b \implies b \not\lt$ (es asimétrica)

**Demostración**
1. Suponemos $a>b$ y $b>c$

$$
    \therefore a-b \in A^{+}, b-c \in A^{+}
$$


$$
    \therefore (a-b)+(b-c) \in A^{+} \text{ ax. 10}
$$



$$
    \implies a-c
$$


2. Si $a>a \implies a-a \in A^{+} \text{ !}$ 
3. Supongamos $a>b$

$$
    \therefore a-b \in A^{+}
$$


$$
    \therefore b-a \in A^{+}
$$


$$
    -(a-b) \text{ ! ax. 12}
$$



### Proposición 2

1. Si $a,b \in A$, por ax. 12 se cumple una y solo una de

$$
a>b, a=b, a<b
$$

En particular, si $a\in A$ vale 1 y solo una de

$$
a>0, a=0, a<0
$$

### Proposición 3
1. $a>b \implies a+c > b+c$
   
   **Demostración:**
   
   1. Supongamos que $a>b \text{ }(\therefore a-b \in A^{+})$
   2. $(a+c)-(b+c) = a-b \in A^{+}$

### Proposición 4
1. $a>b \land c > 0 \implies ac > bc$
   
   **Demostración**
   1. Suponemos que $a>b \land c>0$
   2. $a-b \in A^{+}, c \in A^{+}$
   3. $(a-b)c \in A^{+}$
   4. $ac-bc$
   5. $\therefore ac>bc$
#### Lema
$a>b \implies -b > -a$ ⭐️

### Proposición 5
$a>b \land c<0 \implies ac<bc$ ⭐️
#### Corolario
Sean $a,b \in A \implies$

**Prop. 4**
1. $a>0 \land b>0 \implies ab>0$
   
**Prop 5**
2. $a>0 \land b<0 \implies ab<0$
3. $a<0 \land b>0 \implies ab<0$
4. $a<0 \land b<0 \implies ab>0$

### Proposición 6
1. Si $a\ne 0 \implies a^2 > 0$ (en particular, $1>0$).
   
   **Demostración** ⭐️
   
   1. $a^2=a \cdot a = (-a)(-a) \in A^{+}$ (ax. 11, pues $a \in A^{+}$ o $(-a) \in A^{+}$ (ax. 12))
### Proposición 7
1. $a>0 \land b>1 \implies ab > a$
   
   **Demostración**
   
   1. $ab-a=a(b-1)$ con $a\in A^{+}, (b-1) \in A^{+}$
