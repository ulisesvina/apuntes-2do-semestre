## 1. Concurrencia de las medianas de un triángulo

Sea un triángulo con vértices  
$$
A(x_1,y_1),\quad B(x_2,y_2),\quad C(x_3,y_3).
$$

El punto medio de \(BC\) es
$$
M_{BC}\left(\frac{x_2+x_3}{2},\frac{y_2+y_3}{2}\right).
$$

La mediana desde \(A\) es la recta que une \(A\) con \(M_{BC}\).
De forma análoga se definen las otras dos medianas.

Definimos el punto
$$
G\left(\frac{x_1+x_2+x_3}{3},\frac{y_1+y_2+y_3}{3}\right).
$$

Se verifica directamente que \(G\) pertenece a cada una de las medianas, ya que satisface la ecuación paramétrica de cada recta mediana.  
Por lo tanto, las tres medianas son concurrentes en \(G\), llamado **baricentro**.

---

## 2. Concurrencia de las mediatrices de un triángulo

Consideremos el mismo triángulo \(ABC\).
La mediatriz de \(AB\) es el conjunto de puntos equidistantes de \(A\) y \(B\), es decir,
$$
PA = PB.
$$

Análogamente, la mediatriz de \(AC\) cumple
$$
PA = PC.
$$

Un punto que pertenece a ambas mediatrices satisface
$$
PA = PB = PC,
$$
por lo que es equidistante de los tres vértices.

Esto determina un único punto, llamado **circuncentro**, y por lo tanto las tres mediatrices son concurrentes.

---

## 3. Concurrencia de las alturas de un triángulo

Sea el triángulo \(ABC\).
La altura desde \(A\) es la recta que pasa por \(A\) y es perpendicular a \(BC\).

Analíticamente, si \(BC\) tiene pendiente \(m\), la altura desde \(A\) tiene pendiente \(-1/m\).

Se construyen de forma análoga las alturas desde \(B\) y \(C\).
Al resolver el sistema formado por dos de estas alturas se obtiene un punto común \(H\).
Al sustituir este punto en la ecuación de la tercera altura se verifica que también pertenece a ella.

Por lo tanto, las tres alturas son concurrentes en el **ortocentro**.

---

## 4. Colinealidad del baricentro, circuncentro y ortocentro

Los vértices del triángulo son
$$
A(1,1),\quad B(4,7),\quad C(6,3).
$$

### Baricentro
$$
G=\left(\frac{1+4+6}{3},\frac{1+7+3}{3}\right)=\left(\frac{11}{3},\frac{11}{3}\right).
$$

### Circuncentro
Se calculan las mediatrices de \(AB\) y \(AC\) y se resuelve su intersección, obteniéndose
$$
O=(4,3).
$$

### Ortocentro
Se calculan dos alturas del triángulo y su intersección, obteniéndose
$$
H=\left(\frac{10}{3},\frac{19}{3}\right).
$$

Se verifica que los puntos \(O\), \(G\) y \(H\) satisfacen la misma ecuación lineal, por lo que son colineales.
Esta recta se llama **recta de Euler**.

---

## 5. Distancia de un punto a una recta

Sea la recta
$$
l: ax+by+c=0
$$
y el punto
$$
P_1(x_1,y_1).
$$

La recta perpendicular a \(l\) que pasa por \(P_1\) tiene dirección \((a,b)\).
La distancia buscada es la longitud del segmento perpendicular desde \(P_1\) a \(l\).

Proyectando \(P_1\) sobre la normal de la recta se obtiene
$$
d=\frac{|ax_1+by_1+c|}{\sqrt{a^2+b^2}}.
$$

Esto demuestra la fórmula de la distancia de un punto a una recta.

---

## 6. Concurrencia de las bisectrices interiores (Incentro)

En un triángulo cualquiera, la bisectriz de un ángulo es el conjunto de puntos equidistantes de los dos lados que forman el ángulo.

Sea un punto \(I\) en la intersección de las bisectrices de los ángulos en \(A\) y \(B\).
Entonces:
$$
d(I,AB)=d(I,AC), \quad d(I,BA)=d(I,BC).
$$

De aquí se deduce
$$
d(I,AB)=d(I,BC)=d(I,CA).
$$

Por lo tanto, \(I\) también pertenece a la bisectriz del tercer ángulo.
Las tres bisectrices son concurrentes en un punto que equidista de los tres lados, llamado **incentro**.
