**Tema antecesor:** [[Lógica Proposicional]]
## Definición
Colección de objetos matemáticos, pueden ser números.

## Unión
$$
A \cup B = \{  x | x \in A \lor x \in B \}
$$
$$
x \in A \cup B \leftrightarrow  x \in A \lor x \in B
$$

```tikz
\usepackage{tikz}

\begin{document}

\begin{tikzpicture}

% Fill both sets (this guarantees full union shading)
\fill[blue!25] (0,0) circle (2cm);
\fill[blue!25] (2,0) circle (2cm);

% Draw outlines on top
\draw[thick] (0,0) circle (2cm) node[left] {$A$};
\draw[thick] (2,0) circle (2cm) node[right] {$B$};

% Label
\node at (1,-2.5) {$A \cup B$};

\end{tikzpicture}

\end{document}
```

## Conjunción
$$
A \cap B = \{  x | x \in A \land x \in B \}
$$
$$
x \in A \cap B \leftrightarrow  x \in A \land x \in B
$$

```tikz
\usepackage{tikz}

\begin{document}

\begin{tikzpicture}

% Draw sets
\draw[thick] (0,0) circle (2cm) node[left] {$A$};
\draw[thick] (2,0) circle (2cm) node[right] {$B$};

% Shade intersection
\begin{scope}
  \clip (0,0) circle (2cm);
  \fill[blue!40] (2,0) circle (2cm);
\end{scope}

% Label
\node at (1,-2.5) {$A \cap B$};

\end{tikzpicture}

\end{document}
```
## Contención
$$
 A \subseteq C = \forall x(x \in A \implies x \in B)
$$

```tikz
\usepackage{tikz}

\begin{document}

\begin{tikzpicture}

% Draw superset B
\draw[thick] (0,0) circle (3cm) node[right] {$B$};

% Draw subset A
\fill[blue!20] (-0.8,0) circle (1.5cm);
\draw[thick] (-0.8,0) circle (1.5cm) node {$A$};

% Label
\node at (0,-3.8) {$A \subseteq B$};

\end{tikzpicture}

\end{document}
```
### Teorema
Sean $A,B$ conjuntos, entonces:

$A \subseteq A \cup B, B \subseteq A \cup B$
**Demostración:**

1

$A\cup A\subseteq A$ (idenpotencia)
**Demostración:**

$A=A\cup \varnothing$ (vacío como neutro de la unión)
**Demostración:**

$A \cup (B \cup C) = (A\cup B) \cup C$ (asociatividad)
**Demostración:**

$A\cup B=B\cup A$ (conmutatividad)
**Demostración:**

1. Consideramos que $\forall x(x\in A \cup B \leftrightarrow x \in A \lor x \in B)$ y que $\forall x(x\in B \cup U \leftrightarrow B \in A \lor x \in U)$
2. Notamos que ambas condiciones son equivalentes, ya que $x \in A \lor x \in B \equiv x \in B \lor x \in A$
3. Por inspección de condición, ambos conjuntos están definidos bajo la misma condición, por lo tanto, contienen los mismos elementos.
   
$A\cup B=B \leftrightarrow A  \subseteq B$
**Demostración:**