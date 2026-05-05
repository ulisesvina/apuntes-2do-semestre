	**Tema antecesor:** [[Números Enteros]]

### Definición
Sea $A$ un ACU (y $D$ un dominio entero que luego será ordenado, entonces si $a,b \in A$, se dice que $a$ divide a $b$ $(a|b)$ si $\exists c \in A : b = ac$

#### Ejemplos
1. $2|3$ en $\mathbb{Q}, \mathbb{R}, \mathbb{C}$, pero $2\not| 3$ en $\mathbb{Z}$ 
2. $1|a \forall a \in A$
3. $u|1 \leftrightarrow u \in A^\times (\leftrightarrow u|a\forall a \in A)$
4. $0|a \leftrightarrow a=0$

### Proposición 5
Si $b\ne 0$ y $a|b \implies |a| \le |b|$

**Demostración:**
1. Suponemos s.p.g. $b>0$ y $a\ge 0$.
2. Tenemos $b=aq \land q>0 (\therefore q \ge 1)$

### Proposición 6
Si $a|b$ y $a|c$, entonces $a|(b+c)$
 
### Proposición 7
Si $a|b$ y $a|c$, entonces $a|(b \cdot c)$

### Corolario 2
$a|b \land a|c \implies a|br+cs\forall r,s\in \mathbb{Z}$

### Corolario 3
$a|b \land a|c \leftrightarrow \text{ a divide a toda combinación lineal de b y c}$.

## Algoritmo de la División en $\mathbb{Z}$
### Teorema 1
Si $a,b \in \mathbb{Z}$ y $b\ne 0 \implies$
$$
 \exists!q,r \in \mathbb{Z} : \begin{cases}
a=bq+r\\ 0\le r<b
\end{cases}
$$
**Demostración:**
Sea $M = \{  a-bx : x \in \mathbb{Z} \land a-bx\ge 0 \}$, y $M \ne \varnothing$, sea $s=(-|a|\cdot b) \in \mathbb{Z}$

### Máximo Común Divisor
**Notación:** Si $a \in \mathbb{Z}, D(a) = \{  d \in \mathbb{Z} : d|a \}$

Sabemos
1. $D(0)=\mathbb{Z}$
2. Si $u \in \mathbb{Z}^{\times}, D(a)=D(ua)$
3. $a \ne 0, D(a) \subseteq \{  -|a|, \text{ ...}, -1, 1, \text{ ...}, |a| \}$
   $\therefore \#D(a) < 2|a| \land \text{máx}D(a)=|a|$

#### Lema 1
Si $\varnothing \ne C \subseteq \mathbb{Z}, C$ finito, entonces, $\exists$ el máximo común divisor de C.

**Demostración:**
1. Si $\#C=1, C = \{  c \}, \therefore c = \text{max}C$
2. Si $\#C>1$, sea $C\prime = C \setminus \{ \text{min}C \}$
3. $\therefore \#C\prime < \#C$ y $\text{máx}C=\text{máx}C\prime$

#### Definición
Si $a,b \in \mathbb{Z}$, el máximo común diviso de $a$ y $b$ (notación: $mcd(a,b)$ o simplemente $(a,b)$) es
$$
\begin{cases}
\text{1. }(0,0) = 0 \text{ (si } \{ a,b \} = \{ 0 \} \text{)}\\ \\
\text{2. }(a,b) = \text{max(}D(a)\cap D(b)\text{) (si } \{ a,b \} \ne \{ 0 \}\text{)}
\end{cases}
$$
#### Lema 2
1. $(a,b) = (b,a)$
2. $(a,0) = |a| \forall a \in \mathbb{Z}$
3. $(a,b) = 0 \Leftrightarrow a=b=0$
4. $(au,bv) = (a,b) \forall a,b,\in \mathbb{Z},\forall u,v\in \mathbb{Z}^{\times}$
5. $(a,b) = (|a|,|b|)$

#### Proposición 1
Si $\{ a,b \} \ne \{ 0 \}$ y $0<d=as+bt$ es la combinación lineal positiva mínima de $a$ y $b$. Entonces $d|a \land d|b$

**Demostración**
1. Sean $q,r \in \mathbb{Z} : a = dq + r, 0 \le r < d$
2. $0\le r = a-dq = a-(ar+bs)q = a()$

#### Corolario 1
Si $\{ a,b \} \ne \{ 0 \}$, entonces $(a,b)$ es la combinación lineal positiva mínima de $a$ y $b$.

**Demostración:**
Sin pérdida de generalidad, sean $a,b \ge 0$.
Si $a = 0 \lor b = 0$, es trivial, $\therefore$ puedo suponer $a>0, b>0$.

Sea $d=as+bt$ la combinación linea mínima de $a$ y $b$.
Sea $d\prime = (a,b)$

Por prop. 1, $d|a \land d|b$ ($d\in D(a)\cap D(b)$)
$\therefore d \le d\prime$

Como $d\prime|a$ y $d\prime|b$.
$$
d'|(as+bt)=d
$$
$$
\therefore d' \le d
$$
$$
\therefore d=d' \square
$$
---
Supongamos $d = (a,b) | c$

$$
ax+by=c \text{ diofantina}
$$
$$
ax+by=0 \text{ la homogénea asociativa}
$$

---
Si $d=(a,b)$, sean $a=a\prime d, b = b\prime d (\exists a\prime,b\prime \in \mathbb{R})$

La ecuación homogénea reducida asociada
$$a(*) \text{ es } (*_{hr}): a\prime x+b\prime y = 0$$

### Lema 2
$$
(a', b') = 1
$$
### Lema 3
$(*_{h})$ y $(*_{hr})$ tienen exactamente las $\hat{m}$ soluciones.

$$
\sqrt{1+\sqrt{1+x^2}}
$$

---

### Ejemplo 4 (Tsuntse)

---
### Ejemplo 5 (Brahamagupta, 628, "cuttaca")

$$
\begin{cases}
  \text{1. }x \equiv 1 \pmod{2} \\
\text{2. }x \equiv 1 \pmod{3}  \\
\text{3. }x \equiv 1 \pmod{4}  \\
\text{4. }x \equiv 1 \pmod{5}  \\
\text{5. }x \equiv 1 \pmod{6}  \\
\text{6. }x \equiv 0 \pmod{7} 
\end{cases}
$$

Entonces,
$$
\left(2,3,4,5,6\right) \mid x-1
$$

$$
60 = \left[2,3,4,5,6\right] \mid x-1
$$
$$
\begin{cases}
\text{1. } x \equiv 1 \pmod{60} \\
\text{2.} x \equiv 0 \pmod{7}
\end{cases}
$$
Sólo de $(2)$: $\overline{0}_{7}: x=7k, k\in \mathbb{Z}$
Buscamos $k : 7k \equiv 1 \pmod{60}$, es decir $7k=1+60l$

i.e. $7k-60l = 1$

Bersout: $1=7(-17)+60(2)$

---
## Los anillos $\mathbb{Z}_{m}$
$$
m \gt 1, m \in \mathbb{Z}
$$
Todas las congruencias y clases de congruencia serán módulo m.

**Rec:** $b \in \overline{a} \Longleftrightarrow a \equiv b \pmod{m} \Longleftrightarrow \overline{a} = \overline{b}$

En particular, toda clase $\overline{a}$ puede representarse como $\overline{b}$ para cualquier $b \in \overline{a}$: todos los elementos de $\overline{a} = \{ a + mk | k \in \mathbb{Z} \}$ son representantes igualmente válidos de $\overline{a}$.

### Lema 1
Si $0 \le r \lt m, 0 \le r\prime \lt m$ y $r \equiv r\prime \pmod{m} \implies r = r\prime$

**Dem.**
1. s.p.g. $r\prime = r$
2. Como $0 \le r-r\prime < r$
3. Y como $m \mid r-r\prime, \therefore r-r\prime = 0$
4. $\therefore r = r\prime$

### Proposición 1
Cada clase de congruencia $\overline{a}$ tiene un único representante $r\in \overline{a}$ tal que $0\le r \lt m$.

**Demostración (existencia):**
