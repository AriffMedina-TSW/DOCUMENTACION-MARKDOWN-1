# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Ariff Iazid Medina Gómez
## Grupo: C
## Actividad #18. Documentación de Ejercicios con Git Branches
## Fecha de realización: 18/11/2025
## Tema: Operaciones con matrices

---
# Objetivo

Poder ser más agil con respecto a operaciones un poco más complicadas de matrices, entre las cuales se incluyen los determinantes, regla de Sarrus, Método de cofactores y las aplicaciones geométricas que se le pueden atribuir.

---

## Ejercicio 1: Determinantes 2x2 
### Calcula los determinantes:

$$ A =
\begin{pmatrix}
5 & 2 \\
3 & 1 \\
\end{pmatrix}
$$
 
### Procedimiento 
#### *Paso 1: Multiplicar en diagonal*
    (3)(2)(-1) = -6   |   (5)(1)(1) = 5
#### *Paso 2: Sumar los productos*
    (-6) + 5 = -1
#### **Resultado:** det(A) = -1

$$ B =
\begin{pmatrix}
-1 & 4 \\
2 & -8 \\
\end{pmatrix}
$$
 
### Procedimiento 
#### *Paso 1: Multiplicar en diagonal*
    (2)(4)(-1) = -8   |   (-1)(-8)(1) = 8
#### *Paso 2: Sumar los productos*
    (-8) + 8 = 0
#### **Resultado:** det(B) = 0

$$ C =
\begin{pmatrix}
6 & 9 \\
2 & 3 \\
\end{pmatrix}
$$

### Procedimiento 
#### *Paso 1: Multiplicar en diagonal*
    (2)(9)(-1) = -18   |   (6)(3)(1) = 18
#### *Paso 2: Sumar los productos*
    (-18) + 18 = 0
#### *Resultado: det(C) = 0*

$$ D =
\begin{pmatrix}
0 & 5 \\
-5 & 0 \\
\end{pmatrix}
$$

### Procedimiento 
#### *Paso 1: Multiplicar en diagonal*
    (-5)(5)(-1) = 25   |   (0)(0)(1) = 0
#### *Paso 2: Sumar los productos*
    25 + 0 = 25
#### **Resultado:** det(D) = 25

---

## Ejercicio 2: Regla de Sarrus
### Usa Sarrus para calcular:

$$ E =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 4 & 1 \\
5 & 6 & 0 \\
\end{pmatrix}
$$

#### *Paso 1: Bajar las 2 filas de arriba*

$$
\begin{matrix}
1 & 2 & 3 \\
0 & 1 & 4 \\
5 & 6 & 0 \\
1 & 2 & 3 \\
0 & 1 & 4 \\
\end{matrix}
$$

#### *Paso 2: Multiplicar forma ascendente*
    (0)(2)(0)(-1) = 0
    (1)(6)(4)(-1) = -24
    (5)(1)(3)(-1) = -15

#### *Paso 3: Multiplicar de forma descendente*
    (1)(1)(0)(1) = 0
    (0)(6)(3)(1) = 0
    (5)(2)(4)(1) = 40

#### *Paso 4: Sumar los resultados de la diagonales*
    40 - 39 = 1
#### *Resultado:* det(E) = 1

$$ F =
\begin{pmatrix}
2 & -1 & 3 \\
1 & 4 & 0 \\
3 & 2 & -2 \\
\end{pmatrix}
$$

#### *Paso 1: bajar las 2 filas de arriba*

$$
\begin{matrix}
2 & -1 & 3 \\
1 & 4 & 0 \\
3 & 2 & -2 \\
2 & -1 & 3 \\
1 & 4 & 0 \\
\end{matrix}
$$

#### *Paso 2: Multiplicar forma ascendente*
    (1)(-1)(-2)(-1) = -2
    (-2)(2)(0)(-1) = 0
    (3)(4)(3)(-1) = -36

#### *Paso 3: Multiplicar de forma descendente*
    (2)(4)(-2)(1) = -16
    (1)(2)(3)(1) = 6
    (3)(-1)(0)(1) = 0

#### *Paso 4: Sumar los resultados de la diagonales*
    -52 + 6 = -48
    
#### *Resultado:* det(F) = -48

---

## Ejercicio 3: Método de cofactores
### Calcula usando cofactores (expandir por la fila o columna más conveniente)

$$ G =
\begin{pmatrix}
1 & 0 & 2 \\
-1 & 3 & 1 \\
2 & 0 & 1 \\
\end{pmatrix}
$$

#### *Paso 1: A la primera columna se le agrega el signo +, y se va alternando el signo*

$$ G =
\begin{pmatrix}
(+) & (-) & (+) \\
1 & 0 & 2 \\
-1 & 3 & 1 \\
2 & 0 & 1 \\
\end{pmatrix}
$$

#### *Paso 2: Aplicar la expansión por cofactores en la primera fila.* 
    Se multiplica cada elemento de la primera fila por el determinante de su menor correspondiente, respetando el signo (+,-,+) asignado previamente:

$$ det(G) = 1
\begin{bmatrix}
3 & 1 \\
0 & 1 \\
\end{bmatrix}  - 0
\begin{bmatrix}
-1 & 1 \\
2 & 1 \\
\end{bmatrix} +2
\begin{bmatrix}
-1 & 3 \\
2 & 0 \\
\end{bmatrix}
$$

#### *Paso 3: Multiplicar y sumar los resultados*
    det(G) = 1 (3 - 0) - 0 (-1 - 2)+ 2(0 - 6)
    det(G) = 3 - 12
    det(G) = -9

#### *Respuesta:* det(G) = -9

---

## Ejercicio 4: Verificar propiedades 
### Dadas A y B, Verifica que:

- **det(AB) = det(A) x det(B)**

#### det(AB)=

$$ A =
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
$$

$$ B =
\begin{pmatrix}
1 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

#### *Paso 1: Multiplicar la matriz A por la Matriz B*

$$ AB =
\begin{bmatrix}
(2)(1) & (2)(2) \\
(1)(3) & (1)(1) \\
(1)(1) & (1)(2) \\
(3)(3) & (3)(1) \\
\end{bmatrix}
$$

#### *Paso 2: Sumar el resultado de las multiplicaciones.* 
$$ AB =
\begin{bmatrix}
2 + 3 & 4 + 1 \\
1 + 9 & 2 + 3 \\
\end{bmatrix}
$$

#### *Paso 3: Se escribe la matriz*
$$ AB =
\begin{pmatrix}
5 & 5 \\
10 & 5 \\
\end{pmatrix}
$$

#### Calcular la determinanate de AB
#### *Paso 4: Multiplicar en diagonal*
    (5)(5) = 25   |   (5)(10)(-1) = -50
#### *Paso 5: Sumar los resultados de las multiplicaciones*
    25 - 50 = -25
#### *Respuesta:* det(AB)=-25

#### det(A) x det(B)

$$ A =
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
$$

#### Calcular la determinante de A
#### *Paso 1: Multiplicar en diagonal*
    (2)(3) = 6   |   (1)(1) = -1
#### *Paso 2: Sumar los resultados de las multiplicaciones*
    6 - 1 = 5
#### *Resultado:* det(A)=5

$$ B =
\begin{pmatrix}
1 & 2 \\
3 & 1 \\
\end{pmatrix}
$$

#### Calcular la determinanate de B
#### *Paso 1: Multiplicar en diagonal*
    (1)(1)(1) = 1   |   (3)(2)(-1)=-6
#### *Paso 2: Sumar los resultados de las multiplicaciones*
    1 - 6 = -5
#### *Resultado:* det(B)=-5
#### *Paso 3: Multiplicar las determinanates de A y B*
    det(A) x det(B) = (5)(-5) = -25

#### COMPARAR LA DETERMINANTE DE AB Y DE A x B
#### det(AB) = det(A) x det(B)
    -25 = -25
#### Se comprueba que efectivamente, son iguales

- **det(A ^T)= det(A)**

$$ A =
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
$$

---

#### Calcular la determinanate de A
#### *Paso 1: Multiplicar en diagonal*
    (2)(3)(1) = 6   |   (1)(1)(-1) = -1
#### *Paso 2: Sumar los resultados de las multiplicaciones*
    6 - 1 = 5
#### *Resultado:* det(A)=5

#### Escribir la transpuesta de A

$$ A ^T =
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
$$
#### Calcular la determinanate de A ^T
#### *Paso 1: Multiplicar en diagonal*
    (2)(3)(1) = 6   |   (1)(1)(-1) = -1
#### *Paso 2: Sumar los resultados de las multiplicaciones*
    6 - 1 = 5
#### *Resultado:* det(A ^T)=5

#### Comparamos
#### det(A ^T)=det(A)
    5 = 5
#### Se comprueba que son iguales


## Ejercicio 5: Aplicaciones geometricas 
### Dados los vectores u=(3,2) y v=(1,4)

#### a) Calcula el área del paralelogramo que forman 

$$ A =
\begin{pmatrix}
3 & 2 \\
1 & 4 \\
\end{pmatrix}
$$

#### Calcular la determinanate de A
#### *Paso 1: Multiplicar en diagonal*
    (3)(4)(1) = 12   |   (1)(2)(-1) = -2
#### *Paso 2: Sumar los resultados de las multiplicaciones*
    10 - 12 = 10
#### *Resultado:* det(A)=10
#### El Area es: Area=10

#### b) ¿Cambia el área si intercambias los vectores?

#### Paso 1: Intercambiar vectores
$$ A =
\begin{pmatrix}
3 & 2 \\
1 & 4 \\
\end{pmatrix} => \\ B = 
\begin{pmatrix}
1 & 4 \\
3 & 2 \\
\end{pmatrix} 
$$ 

#### Calcular la determinanate de B
#### *Paso 1: Multiplicar en diagonal*
    (1)(2)(1) = 2   |   (3)(4)(-1) = -12
#### *Paso 2: Sumar los resultados de las multiplicaciones*
    -12 + 2=-10
#### *Resultado:* det(B) = -10
#### El Area es: Area = -10
#### El area SÍ cambia si intercambias los vectores

#### c) ¿Qué representa el signo del teterminante?
#### La forma en la que se acomodan los vectores.
