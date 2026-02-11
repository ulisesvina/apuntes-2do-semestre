## Proposiciones
Son oraciones que pueden tomar un valor de verdad.

### Ejemplos
P: Hoy es un buen día para un pícnic (v)
Q: El clima de hoy es magnífico (v)
S: El sarampión es una enfermedad (v)

1. P porque Q (v)
2. Q porque M (v)

---
## Conjunción
Representa al "y" en la tabla de verdad, sólo retorna un valor verdadero cuando todas las proposiciones son verdaderas.

| p   | q   | p^q |
| --- | --- | --- |
| 1   | 1   | 1   |
| 1   | 0   | 0   |
| 0   | 1   | 0   |
| 0   | 0   | 0   |

## Disyunción
Representa al "o" en la tabla de verdad y retorna un valor verdadero cuando al menos una de las proposiciones se cumple.

| p   | q   | pvq |
| --- | --- | --- |
| 1   | 1   | 1   |
| 1   | 0   | 1   |
| 0   | 1   | 1   |
| 0   | 0   | 0   |
### O exclusivo (xor)
Representa al "o" en la tabla de verdad, pero sólo retorna un valor verdadero cuando ambas proposiciones son diferentes entre sí.

| p   | q   | p xor q |
| --- | --- | ------- |
| 1   | 1   | 0       |
| 1   | 0   | 1       |
| 0   | 1   | 1       |
| 0   | 0   | 0       |

| p   | q   | pvq | p^q | ¬(p^q) | (pvq)^¬(p^q) |
| --- | --- | --- | --- | ------ | ------------ |
| 1   | 1   | 1   | 1   | 0      | 0            |
| 1   | 0   | 1   | 0   | 1      | 1            |
| 0   | 1   | 1   | 0   | 1      | 1            |
| 0   | 0   | 0   | 0   | 1      | 0            |
### Implicación (Condicional)
Representa a "entonces" en la tabla de verdad, es comúnmente usando con *modus tollendo tollens* y sirve para hacer la implicación de que si se cumple la primera proposición, la segunda también debe cumplirse.

fire
### Doble implicación (Bicondicional)
Representa a "si y solo sí" en la tabla de verdad. Sirve para hacer la implicación de que si se cumple la primera proposición, la segunda también debe cumplirse y viceversa, si la segunda se cumple, la primera necesariamente debe cumplirse también.

| p   | q   | p $\leftrightarrow$ q |
| --- | --- | --------------------- |
| 1   | 1   | 1                     |
| 1   | 0   | 0                     |
| 0   | 1   | 0                     |
| 0   | 0   | 1                     |

---

