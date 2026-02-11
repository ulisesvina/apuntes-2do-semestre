## Conjuntos acotados
1. $A \subseteq \mathbb{R}$ está acotado superiormente si $\exists m \in \mathbb{R} : \forall a \in A \to M \ge a$.
2. $A \subseteq \mathbb{R}$ está acotado inferiormente si $\exists m \in \mathbb{R} : \forall a \in A \to m \le a$
3. $A$ está acotado si $\exists M > 0 : \forall a \in A |a| \le M$

---
Sean $f: [a, b] \to \mathbb{R}$ una función acotada y $P = \{  a = t_{o} < t_{1} < \text{ ... } < t_{m} =b \}$ una partición de $[a,b]$.

$$
m_{j} = inf\{ f(x)|x\in[t_{j-i}, t_{j}] \}
$$
$$
 M_{j} = sup\{  \}
$$
---
$$
I(f, P) := \sum_{j=1}^m m_{j}(t_{j}-t_{j-i})
$$
$$
S(f, P) := \sum_{j=1}^m M_{j}(t_{j}-t_{j-i})
$$
Para mejorar la precisión de la aproximación del área de $R(f,a,b)$ por una suma inferior $I(f,P)$, vamos a agregar un punto a P.

Comenzamos agregando uno:
$$
Q = P\cup \{ r \}
$$
Calculamos las sumas inferiores:
$$
I(f,P) = \sum_{j=1}^m m_{j}(t_{j}-t_{j-i})
$$
$$
= \sum_{j=1; j\ne c}^m m_{j}(t_{j}-t_{j-1}) + m_{c} (t_{c}-t_{c-1})
$$
en donde $m_{j} = inf \{ f(x)|x \in [tj-1, tj] \}$.

Para calcular $I(f,Q)$ necesitamos 
$$
\mu_{c-1} := inf \{ f(x) | x \in [t_{c-1}, r] \}
$$
$$
\mu_{c} = inf \{ f(x) | x \in [r, t_{c}] \}
$$
Entonces, el intervalo $[t_{c-1}, t_{c}]$ se reemplaza por dos intervalos $[t_{c-1}, r]$ y $[r, t_{c}]$.

Como $A \subseteq C \implies$
$$
 m_{c} = inf C \le inf A = \mu_{c-1}
$$

Similarmente,
$$
m_{c} \le \mu_{c}
$$
---
$$
I(f,P) = \sum_{j=1; j\ne c}^m m_{j}(t_{j} - t_{j-i}) + m_{c}(t_{c}-t_{c-1})
$$
$$
I(f,Q) = \sum_{j=1; j\ne c}^m m_{j}(t_{j}-t_{j-i}) + \mu_{c-1}(r_{t_{c-1}}) + \mu_{c(t_{c}-r)}
$$
Sean $P,Q$ particiones de $[a,b]$. Decimos que $Q$ refina a $P$ si $P \subseteq Q$

### Proposición
Sean $f:[a,b] \to \mathbb{R}$ una función acotada y $P, Q$ particiones de $[a,b]$ tales que $Q$ refina a $P$, entonces $$
I(f,P) \le I(f,Q)
$$
**Demostración**
Como $P, Q$ son finitas, existen particiones $P = R_{0} \subseteq R_{1} =\subseteq R_{2} \text{ ... } \subseteq R_{k} = Q$
tales que $|R_{j} \setminus R_{j-1}| = 1$. Por el resultado anterior, $$
I(f,R_{j-1}) \le I(f,R_{j})
$$
$$
\therefore I(f,P) = I(f, R_{0}) \le I(f,R_{1}) \le \text{ ...} \le I(f_{1}, R_{k})
$$
$$
\therefore I(f,P) \le I(f,Q)
$$
Con la misma idea se prueba:
### Proposición
Sean $f:[a,b] \to \mathbb{R}$ acotada y $P,Q$ particiones de $[a,b]$ tales que $P \subseteq Q \implies$
$$
S(f,Q) \le S(f,P)
$$
