# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Ariff Iazid Medina Gómez
## Grupo: C
## Actividad #16.  Documentación matrices

---
# Objetivo

Familiarizarse con la clasificación y operaciones básicas de matrices, incluyendo suma, resta, multiplicación y transposición.

---

# Ejercicio 1: Clasificación de matrices

## Objetivo del ejercicio: Reconocer y distinguir los distintos tipos de matrices de acuerdo con sus propiedades.


### a) 

$$A = \begin{bmatrix}
1 & 0 \\
0 & 1 
\end{bmatrix}$$

Es una **matriz identidad** porque tiene unos en su diagonal principal y ceros en el resto de sus posiciones. 

### b) 

$$ B = \begin{bmatrix}
3 & 0 & 0 \\
0 & -2 & 0 \\
0 & 0 & 5 
\end{bmatrix}  $$

Es una **matriz diagonal**, pues todos sus elementos son ceros excepto los que se encuentran en la diagonal principal.

### c)

$$C = \begin{bmatrix}
2 & 1 & 4 \\
1 & 3 & 5 \\
4 & 5 & 6 
\end{bmatrix}  $$

Se trata de una **matriz simétrica** porque cumple que $a_ij = a_ji$ es decir, sus elementos se reflejan respecto a la diagonal principal.

### d)

$$ D = \begin{bmatrix}
1 & 2 & 3 \\
0 & 4 & 5 \\
0 & 0 & 6 
\end{bmatrix}  $$

Es una **matriz triangular** superior porque todos los elementos que se encuentran por debajo de la diagonal principal son ceros.

---

# Ejercicio 2: Operaciones con matrices

## Objetivo del ejercicio: Realizar operaciones fundamentales con matrices, como la suma, resta, multiplicación y transposición

Dadas las siguientes matrices:

$$ A = \begin{bmatrix}
2 & -1 \\
3 & 4 
\end{bmatrix}, \quad B = \begin{bmatrix}
5 & 2 \\
-1 & 3 
\end{bmatrix} $$

Calculamos: 

### a) \( A + B \)
$$ A + B = \begin{bmatrix}
2 + 5 & -1 + 2 \\
3 + (-1) & 4 + 3
\end{bmatrix} => \begin{bmatrix}
7 & 1 \\
2 & 7
\end{bmatrix} $$

### b) \(2A - B \)

$$ 2A = \begin{bmatrix}
2(2) & 2(-1) \\
2(3) & 2(4)
\end{bmatrix} => \begin{bmatrix}
4 & -2 \\    
6 & 8
\end{bmatrix} $$
$$ 2A - B = 2 \begin{bmatrix}
4-5 & -2-2 \\
6-(-1) & 8-3
\end{bmatrix} => \begin{bmatrix}
-1 & -4 \\
7 & 5
\end{bmatrix} $$

### c) \( AB \)
$$ AB = \begin{bmatrix}
2\cdot5+(-1)\cdot(-1) & 2\cdot2+(-1)\cdot3\\
3\cdot5+4\cdot(-1)    & 3\cdot2+4\cdot3
\end{bmatrix} => \begin{bmatrix}
10 + 1 & 4 - 3\\
15 - 4 & 6 + 12
\end{bmatrix} => \begin{bmatrix}
11 & 1 \\
11 & 18
\end{bmatrix} $$

### d) \( BA \)
$$ BA = \begin{bmatrix}
(5\cdot2) + (2\cdot3) & (5\cdot-1) + (2\cdot4) \\
(-1\cdot2) + (3\cdot3) & (-1\cdot-1) + (3\cdot4)
\end{bmatrix} => \begin{bmatrix}
10 + 6 & -5 + 8 \\
-2 + 9 & 1 + 12
\end{bmatrix} => \begin{bmatrix}
16 & 3 \\
7 & 13
\end{bmatrix} $$

### e) \( A^T \)
$$ A^T = \begin{bmatrix}
2 & 3 \\
-1 & 4
\end{bmatrix} $$

---

# Ejercicio 3: Multiplicación cadena

## Objetivo del ejercicio: Comprobar la propiedad asociativa de la multiplicación de matrices mediante el cálculo de productos en cadena.


---

 

Dadas las matrices:

$$ A = \begin{bmatrix}
1 & 2 \\
3 & 4 
\end{bmatrix}, \quad B = \begin{bmatrix}
2 & 0 \\
1 & 3 
\end{bmatrix}, \quad C = \begin{bmatrix}
1 & 1 \\
0 & 2
\end{bmatrix} $$

*Verificar que* $(AB)C = A(BC)$

### a) Calcular (AB)C 
$$ AB = \begin{bmatrix}
(1\cdot2) + (2\cdot1) & (1\cdot0) + (2\cdot3) \\
(3\cdot2) + (4\cdot1) & (3\cdot0) + (4\cdot3)
\end{bmatrix} => \begin{bmatrix}
2 + 2 & 0 + 6 \\
6 + 4 & 0 + 12
\end{bmatrix} => \begin{bmatrix}
4 & 6 \\
10 & 12
\end{bmatrix} $$

$$ (AB)C = \begin{bmatrix}
(4\cdot1) + (6\cdot0) & (4\cdot1) + (6\cdot2) \\
(10\cdot1) + (12\cdot0) & (10\cdot1) + (12\cdot2)
\end{bmatrix} => \begin{bmatrix}
4 + 0 & 4 + 12 \\
10 + 0 & 10 + 24
\end{bmatrix} => \begin{bmatrix}
4 & 16 \\
10 & 34
\end{bmatrix} $$

### b) Calcular A(BC) 
$$ BC = \begin{bmatrix}
(2\cdot1) + (0\cdot0) & (2\cdot1) + (0\cdot2) \\
(1\cdot1) + (3\cdot0) & (1\cdot1) + (3\cdot2)
\end{bmatrix} => \begin{bmatrix}
2 + 0 & 2 + 0 \\
1 + 0 & 1 + 6
\end{bmatrix} => \begin{bmatrix}
2 & 2 \\
1 & 7
\end{bmatrix} $$
$$ A(BC) = \begin{bmatrix}
(1\cdot2) + (2\cdot1) & (1\cdot2) + (2\cdot7) \\
(3\cdot2) + (4\cdot1) & (3\cdot2) + (4\cdot7)
\end{bmatrix} = \begin{bmatrix}
2 + 2 & 2 + 14 \\
6 + 4 & 6 + 28
\end{bmatrix} => \begin{bmatrix}
4 & 16 \\
10 & 34
\end{bmatrix} $$

*Veredicto final*: Se verifica que $(AB)C y A(BC)$ **son iguales** puesto que resultan con los mismos elementos en su matriz.
