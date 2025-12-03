# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: Ariff Iazid Medina Gómez
## Grupo: C
## Actividad #22.  Última documentación

## **Objetivo general**
Documentar la resolución de varios sistemas de ecuaciones usando distintos métodos de matrices.

---

# ✏️ **Ejercicio 1 – Resolver el sistema por todos los métodos**

**Sistema original:**
```math
\begin{cases}
x + y + z = 6\\
2x - y + z = 3\\
x + 2y - z = 2
\end{cases}
```

---

## Método Gauss

### **Matriz aumentada inicial:**
```
| 1   1   1 | 6 |
| 2  -1   1 | 3 |
| 1   2  -1 | 2 |
```

### **Operaciones aplicadas:**
1. `F2 = F2 - 2F1`
2. `F3 = F3 - F1`
3. `F3 = F3 + F2`

### **Resultado:**
```
| 1   1   1 | 6 |
| 0  -3  -1 | -9|
| 0   0   2 | 4 |
```

### **Resultados**
- `z = 2`
- `y = 3`
- `x = 1`

---

## Método Gauss–Jordan

Partimos de la matriz escalonada anterior:
```
| 1   1   1 | 6 |
| 0  -3  -1 | -9|
| 0   0   2 | 4 |
```

### **Pasos:**
1. `F3 = (1/2)F3`
2. `F2 = F2 + F3`
3. `F1 = F1 - F3`
4. `F1 = F1 - F2`

### **Matriz identidad resultante:**
```
| 1  0  0 | 1 |
| 0  1  0 | 3 |
| 0  0  1 | 2 |
```

---

## Método Matriz inversa

### **Matriz A:**
```math
A = \begin{bmatrix}
1 & 1 & 1\\
2 & -1 & 1\\
1 & 2 & -1
\end{bmatrix}
```

### **Vector B:**
```math
B = \begin{bmatrix} 6 \\ 3 \\ 2 \end{bmatrix}
```

### **Cálculo:**
`X = A^{-1}B`

### **Resultado:**
```math
X = \begin{bmatrix} 1 \\ 3 \\ 2 \end{bmatrix}
```

---

## Método Regla de Cramer

- Determinante: `det(A) = 6`
- Resultados:
  - `x = 1`
  - `y = 3`
  - `z = 2`

---

### **Resultado**
```math
(x, y, z) = (1, 3, 2)
```

---

# ✏️ **Ejercicio 2 – Tipo de solución**

### **a)** Sistema dependiente → *soluciones infinitas*.
### **b)** Sistema incompatible → *no tiene solución*.
### **c)** Sistema compatible determinado → *solución única*.

---

# ✏️ **Ejercicio 3 – Sistema 4×4**

```math
\begin{cases}
x + y + z + w = 10\\
2x + y - z + w = 5\\
x - y + z - w = 1\\
x + y - z + 2w = 8
\end{cases}
```

### **Matriz aumentada:**
```
| 1  1  1  1 | 10 |
| 2  1 -1  1 | 5  |
| 1 -1  1 -1 | 1  |
| 1  1 -1  2 | 8  |
```

### **Después de Gauss:**
```
| 1  1  0  0 | 3 |
| 0  1  0  1 | 4 |
| 0  0  1  1 | 3 |
| 0  0  0  1 | 1 |
```

### **Resultados**
- `w = 1`
- `z = 2`
- `y = 3`
- `x = 0`

---

# ✏️ **Ejercicio 4 – Aplicación práctica**

**Productos:** `P = Premium`, `S = Standard`, `U = Utilitario`  
**Materias:** res (R), pollo (Q), cerdo (C)

Sistema:
```math
\begin{bmatrix}
2 & 1 & 3\\
3 & 1 & 2\\
1 & 2 & 1
\end{bmatrix}
\begin{bmatrix} P \\ S \\ U \end{bmatrix}
=
\begin{bmatrix} 100 \\ 120 \\ 80 \end{bmatrix}
```

### **Luego de Gauss:**
```
| 1  0  1 | 20 |
| 0  1  1 | 40 |
| 0  0  1 | 20 |
```

### **Resultado**
- `U = 20`
- `S = 20`
- `P = 0`

---
