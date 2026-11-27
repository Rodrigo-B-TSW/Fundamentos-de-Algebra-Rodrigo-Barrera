# Actividad #32. Matrices: Método de Gauss y Gauss-Jordan
 
| DATOS | |
| :--- | :--- |
| **Alumno** | Rodrigo Barrera García |
| **Profesor** | Jorge Javier Pedrozo Romero |
| **Materia** | Fundamentos de Álgebra |
| **Fecha** | 16/11/2026 |
| **Lugar** | Mérida, Yucatán. México |

### NOTA: La organización y el diseño en html/markdown fueron utilizadas herramientas de inteligencia artificial como apoyo, los procedimientos de cada ejercicio fueron hechos de manera personal y de lo aprendido en clase.
---
 
## 1. Método de Gauss · Ejercicios 37-44
 
> **Procedimiento:**
>
> 1. Escribo la matriz aumentada $[A \mid b]$ con los coeficientes y los términos independientes.
> 2. Con operaciones entre filas hago ceros debajo de la diagonal (matriz escalonada).
> 3. Resuelvo por sustitución hacia atrás: de la última fila a la primera.
>
> **Tres reglas importantes:** 
>
> - Intercambiar filas: $R_i \leftrightarrow R_j$
> - Multiplicar una fila por un número distinto de cero: $R_i \to kR_i$
> - Sumar o restar a una fila un múltiplo de otra: $R_i \to R_i + kR_j$

#### Ejercicio 37
 
**Sistema:**
 
$$
\begin{aligned}
6x+y-z &= -22 \\
-x+3y+3z &= 22 \\
-6x-6z &= 12
\end{aligned}
$$
 
**Matriz aumentada:**
 
$$
\left[\begin{array}{ccc|c}
6 & 1 & -1 & -22 \\
-1 & 3 & 3 & 22 \\
-6 & 0 & -6 & 12
\end{array}\right]
$$
 
**Paso 1:** $R_1 \leftrightarrow R_2$
 
$$
\left[\begin{array}{ccc|c}
-1 & 3 & 3 & 22 \\
6 & 1 & -1 & -22 \\
-6 & 0 & -6 & 12
\end{array}\right]
$$
 
**Paso 2:** $R_2 \to R_2 + 6R_1,\ R_3 \to R_3 - 6R_1$
 
$$
\left[\begin{array}{ccc|c}
-1 & 3 & 3 & 22 \\
0 & 19 & 17 & 110 \\
0 & -18 & -24 & -120
\end{array}\right]
$$
 
**Paso 3:** $R_3 \to \frac{1}{6}R_3$
 
$$
\left[\begin{array}{ccc|c}
-1 & 3 & 3 & 22 \\
0 & 19 & 17 & 110 \\
0 & -3 & -4 & -20
\end{array}\right]
$$
 
**Paso 4:** $R_3 \to 19R_3 + 3R_2$
 
$$
\left[\begin{array}{ccc|c}
-1 & 3 & 3 & 22 \\
0 & 19 & 17 & 110 \\
0 & 0 & -25 & -50
\end{array}\right]
$$
 
**Paso 5:** $R_3 \to \frac{1}{25}R_3$
 
$$
\left[\begin{array}{ccc|c}
-1 & 3 & 3 & 22 \\
0 & 19 & 17 & 110 \\
0 & 0 & -1 & -2
\end{array}\right]
$$
 
La matriz ya es escalonada (ceros debajo de la diagonal). Ahora resuelvo de la última fila a la primera.
 
**Sustitución hacia atrás:**
 
Fila 3:
 
$$
\begin{aligned}
-z &= -2 \\
z &= 2
\end{aligned}
$$
 
Fila 2:
 
$$
\begin{aligned}
19y+17z &= 110 \\
19y+17(2) &= 110 \\
19y &= 76 \\
y &= 4
\end{aligned}
$$
 
Fila 1:
 
$$
\begin{aligned}
-x+3y+3z &= 22 \\
-x+3(4)+3(2) &= 22 \\
-x &= 4 \\
x &= -4
\end{aligned}
$$
 
**Solución:** $x=-4$, $y=4$, $z=2$
 
 
#### Ejercicio 38
 
**Sistema:**
 
$$
\begin{aligned}
-4a-3b-2c &= -8 \\
a-4b-2c &= -3 \\
4a-2b+c &= 6
\end{aligned}
$$
 
**Matriz aumentada:**
 
$$
\left[\begin{array}{ccc|c}
-4 & -3 & -2 & -8 \\
1 & -4 & -2 & -3 \\
4 & -2 & 1 & 6
\end{array}\right]
$$
 
**Paso 1:** $R_1 \leftrightarrow R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & -4 & -2 & -3 \\
-4 & -3 & -2 & -8 \\
4 & -2 & 1 & 6
\end{array}\right]
$$
 
**Paso 2:** $R_2 \to R_2 + 4R_1,\ R_3 \to R_3 - 4R_1$
 
$$
\left[\begin{array}{ccc|c}
1 & -4 & -2 & -3 \\
0 & -19 & -10 & -20 \\
0 & 14 & 9 & 18
\end{array}\right]
$$
 
**Paso 3:** $R_3 \to 19R_3 + 14R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & -4 & -2 & -3 \\
0 & -19 & -10 & -20 \\
0 & 0 & 31 & 62
\end{array}\right]
$$
 
**Paso 4:** $R_3 \to \frac{1}{31}R_3$
 
$$
\left[\begin{array}{ccc|c}
1 & -4 & -2 & -3 \\
0 & -19 & -10 & -20 \\
0 & 0 & 1 & 2
\end{array}\right]
$$
 
La matriz ya es escalonada (ceros debajo de la diagonal). Ahora resuelvo de la última fila a la primera.
 
**Sustitución hacia atrás:**
 
Fila 3:
 
$$
\begin{aligned}
c &= 2 \\
c &= 2
\end{aligned}
$$
 
Fila 2:
 
$$
\begin{aligned}
-19b-10c &= -20 \\
-19b-10(2) &= -20 \\
-19b &= 0 \\
b &= 0
\end{aligned}
$$
 
Fila 1:
 
$$
\begin{aligned}
a-4b-2c &= -3 \\
a-4(0)-2(2) &= -3 \\
a &= 1 \\
a &= 1
\end{aligned}
$$
 
**Solución:** $a=1$, $b=0$, $c=2$
 
 
#### Ejercicio 39
 
**Sistema:**
 
$$
\begin{aligned}
a+5b-4c &= -14 \\
2a-5b-5c &= -7 \\
3a+3b+2c &= -2
\end{aligned}
$$
 
**Matriz aumentada:**
 
$$
\left[\begin{array}{ccc|c}
1 & 5 & -4 & -14 \\
2 & -5 & -5 & -7 \\
3 & 3 & 2 & -2
\end{array}\right]
$$
 
**Paso 1:** $R_2 \to R_2 - 2R_1,\ R_3 \to R_3 - 3R_1$
 
$$
\left[\begin{array}{ccc|c}
1 & 5 & -4 & -14 \\
0 & -15 & 3 & 21 \\
0 & -12 & 14 & 40
\end{array}\right]
$$
 
**Paso 2:** $R_2 \to \frac{1}{3}R_2,\ R_3 \to \frac{1}{2}R_3$
 
$$
\left[\begin{array}{ccc|c}
1 & 5 & -4 & -14 \\
0 & -5 & 1 & 7 \\
0 & -6 & 7 & 20
\end{array}\right]
$$
 
**Paso 3:** $R_3 \to 5R_3 - 6R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & 5 & -4 & -14 \\
0 & -5 & 1 & 7 \\
0 & 0 & 29 & 58
\end{array}\right]
$$
 
**Paso 4:** $R_3 \to \frac{1}{29}R_3$
 
$$
\left[\begin{array}{ccc|c}
1 & 5 & -4 & -14 \\
0 & -5 & 1 & 7 \\
0 & 0 & 1 & 2
\end{array}\right]
$$
 
La matriz ya es escalonada (ceros debajo de la diagonal). Ahora resuelvo de la última fila a la primera.
 
**Sustitución hacia atrás:**
 
Fila 3:
 
$$
\begin{aligned}
c &= 2 \\
c &= 2
\end{aligned}
$$
 
Fila 2:
 
$$
\begin{aligned}
-5b+c &= 7 \\
-5b+(2) &= 7 \\
-5b &= 5 \\
b &= -1
\end{aligned}
$$
 
Fila 1:
 
$$
\begin{aligned}
a+5b-4c &= -14 \\
a+5(-1)-4(2) &= -14 \\
a &= -1 \\
a &= -1
\end{aligned}
$$
 
**Solución:** $a=-1$, $b=-1$, $c=2$
 
 
#### Ejercicio 40
 
**Sistema:**
 
$$
\begin{aligned}
6x+6y+5z &= 16 \\
-6x+6y+z &= 20 \\
2x-2y+3z &= 0
\end{aligned}
$$
 
**Matriz aumentada:**
 
$$
\left[\begin{array}{ccc|c}
6 & 6 & 5 & 16 \\
-6 & 6 & 1 & 20 \\
2 & -2 & 3 & 0
\end{array}\right]
$$
 
**Paso 1:** $R_2 \to R_2 + R_1,\ R_3 \to 3R_3 - R_1$
 
$$
\left[\begin{array}{ccc|c}
6 & 6 & 5 & 16 \\
0 & 12 & 6 & 36 \\
0 & -12 & 4 & -16
\end{array}\right]
$$
 
**Paso 2:** $R_2 \to \frac{1}{6}R_2,\ R_3 \to \frac{1}{4}R_3$
 
$$
\left[\begin{array}{ccc|c}
6 & 6 & 5 & 16 \\
0 & 2 & 1 & 6 \\
0 & -3 & 1 & -4
\end{array}\right]
$$
 
**Paso 3:** $R_3 \to 2R_3 + 3R_2$
 
$$
\left[\begin{array}{ccc|c}
6 & 6 & 5 & 16 \\
0 & 2 & 1 & 6 \\
0 & 0 & 5 & 10
\end{array}\right]
$$
 
**Paso 4:** $R_3 \to \frac{1}{5}R_3$
 
$$
\left[\begin{array}{ccc|c}
6 & 6 & 5 & 16 \\
0 & 2 & 1 & 6 \\
0 & 0 & 1 & 2
\end{array}\right]
$$
 
La matriz ya es escalonada (ceros debajo de la diagonal). Ahora resuelvo de la última fila a la primera.
 
**Sustitución hacia atrás:**
 
Fila 3:
 
$$
\begin{aligned}
z &= 2 \\
z &= 2
\end{aligned}
$$
 
Fila 2:
 
$$
\begin{aligned}
2y+z &= 6 \\
2y+(2) &= 6 \\
2y &= 4 \\
y &= 2
\end{aligned}
$$
 
Fila 1:
 
$$
\begin{aligned}
6x+6y+5z &= 16 \\
6x+6(2)+5(2) &= 16 \\
6x &= -6 \\
x &= -1
\end{aligned}
$$
 
**Solución:** $x=-1$, $y=2$, $z=2$
 
 
#### Ejercicio 41
 
**Sistema:**
 
$$
\begin{aligned}
-2a+b-4c &= 7 \\
4a+6b+c &= 19 \\
-6a-6b-5c &= -17
\end{aligned}
$$
 
**Matriz aumentada:**
 
$$
\left[\begin{array}{ccc|c}
-2 & 1 & -4 & 7 \\
4 & 6 & 1 & 19 \\
-6 & -6 & -5 & -17
\end{array}\right]
$$
 
**Paso 1:** $R_2 \to R_2 + 2R_1,\ R_3 \to R_3 - 3R_1$
 
$$
\left[\begin{array}{ccc|c}
-2 & 1 & -4 & 7 \\
0 & 8 & -7 & 33 \\
0 & -9 & 7 & -38
\end{array}\right]
$$
 
**Paso 2:** $R_3 \to 8R_3 + 9R_2$
 
$$
\left[\begin{array}{ccc|c}
-2 & 1 & -4 & 7 \\
0 & 8 & -7 & 33 \\
0 & 0 & -7 & -7
\end{array}\right]
$$
 
**Paso 3:** $R_3 \to \frac{1}{7}R_3$
 
$$
\left[\begin{array}{ccc|c}
-2 & 1 & -4 & 7 \\
0 & 8 & -7 & 33 \\
0 & 0 & -1 & -1
\end{array}\right]
$$
 
La matriz ya es escalonada (ceros debajo de la diagonal). Ahora resuelvo de la última fila a la primera.
 
**Sustitución hacia atrás:**
 
Fila 3:
 
$$
\begin{aligned}
-c &= -1 \\
c &= 1
\end{aligned}
$$
 
Fila 2:
 
$$
\begin{aligned}
8b-7c &= 33 \\
8b-7(1) &= 33 \\
8b &= 40 \\
b &= 5
\end{aligned}
$$
 
Fila 1:
 
$$
\begin{aligned}
-2a+b-4c &= 7 \\
-2a+(5)-4(1) &= 7 \\
-2a &= 6 \\
a &= -3
\end{aligned}
$$
 
**Solución:** $a=-3$, $b=5$, $c=1$
 
 
#### Ejercicio 42
 
**Sistema:**
 
$$
\begin{aligned}
5a-3b+5c &= 22 \\
-4a-b+c &= -16 \\
2a+4b-c &= 11
\end{aligned}
$$
 
**Matriz aumentada:**
 
$$
\left[\begin{array}{ccc|c}
5 & -3 & 5 & 22 \\
-4 & -1 & 1 & -16 \\
2 & 4 & -1 & 11
\end{array}\right]
$$
 
**Paso 1:** $R_2 \to 5R_2 + 4R_1,\ R_3 \to 5R_3 - 2R_1$
 
$$
\left[\begin{array}{ccc|c}
5 & -3 & 5 & 22 \\
0 & -17 & 25 & 8 \\
0 & 26 & -15 & 11
\end{array}\right]
$$
 
**Paso 2:** $R_3 \to 17R_3 + 26R_2$
 
$$
\left[\begin{array}{ccc|c}
5 & -3 & 5 & 22 \\
0 & -17 & 25 & 8 \\
0 & 0 & 395 & 395
\end{array}\right]
$$
 
**Paso 3:** $R_3 \to \frac{1}{395}R_3$
 
$$
\left[\begin{array}{ccc|c}
5 & -3 & 5 & 22 \\
0 & -17 & 25 & 8 \\
0 & 0 & 1 & 1
\end{array}\right]
$$
 
La matriz ya es escalonada (ceros debajo de la diagonal). Ahora resuelvo de la última fila a la primera.
 
**Sustitución hacia atrás:**
 
Fila 3:
 
$$
\begin{aligned}
c &= 1 \\
c &= 1
\end{aligned}
$$
 
Fila 2:
 
$$
\begin{aligned}
-17b+25c &= 8 \\
-17b+25(1) &= 8 \\
-17b &= -17 \\
b &= 1
\end{aligned}
$$
 
Fila 1:
 
$$
\begin{aligned}
5a-3b+5c &= 22 \\
5a-3(1)+5(1) &= 22 \\
5a &= 20 \\
a &= 4
\end{aligned}
$$
 
**Solución:** $a=4$, $b=1$, $c=1$
 
 
#### Ejercicio 43
 
**Sistema:**
 
$$
\begin{aligned}
-3a+5b &= 26 \\
-6a+4b+c &= 26 \\
3a+5b+3c &= 8
\end{aligned}
$$
 
**Matriz aumentada:**
 
$$
\left[\begin{array}{ccc|c}
-3 & 5 & 0 & 26 \\
-6 & 4 & 1 & 26 \\
3 & 5 & 3 & 8
\end{array}\right]
$$
 
**Paso 1:** $R_2 \to R_2 - 2R_1,\ R_3 \to R_3 + R_1$
 
$$
\left[\begin{array}{ccc|c}
-3 & 5 & 0 & 26 \\
0 & -6 & 1 & -26 \\
0 & 10 & 3 & 34
\end{array}\right]
$$
 
**Paso 2:** $R_3 \to 3R_3 + 5R_2$
 
$$
\left[\begin{array}{ccc|c}
-3 & 5 & 0 & 26 \\
0 & -6 & 1 & -26 \\
0 & 0 & 14 & -28
\end{array}\right]
$$
 
**Paso 3:** $R_3 \to \frac{1}{14}R_3$
 
$$
\left[\begin{array}{ccc|c}
-3 & 5 & 0 & 26 \\
0 & -6 & 1 & -26 \\
0 & 0 & 1 & -2
\end{array}\right]
$$
 
La matriz ya es escalonada (ceros debajo de la diagonal). Ahora resuelvo de la última fila a la primera.
 
**Sustitución hacia atrás:**
 
Fila 3:
 
$$
\begin{aligned}
c &= -2 \\
c &= -2
\end{aligned}
$$
 
Fila 2:
 
$$
\begin{aligned}
-6b+c &= -26 \\
-6b+(-2) &= -26 \\
-6b &= -24 \\
b &= 4
\end{aligned}
$$
 
Fila 1:
 
$$
\begin{aligned}
-3a+5b &= 26 \\
-3a+5(4) &= 26 \\
-3a &= 6 \\
a &= -2
\end{aligned}
$$
 
**Solución:** $a=-2$, $b=4$, $c=-2$
 
 
#### Ejercicio 44
 
**Sistema:**
 
$$
\begin{aligned}
5a-5b-c &= -30 \\
5a-6b-c &= -29 \\
-5a+4b-4c &= 6
\end{aligned}
$$
 
**Matriz aumentada:**
 
$$
\left[\begin{array}{ccc|c}
5 & -5 & -1 & -30 \\
5 & -6 & -1 & -29 \\
-5 & 4 & -4 & 6
\end{array}\right]
$$
 
**Paso 1:** $R_2 \to R_2 - R_1,\ R_3 \to R_3 + R_1$
 
$$
\left[\begin{array}{ccc|c}
5 & -5 & -1 & -30 \\
0 & -1 & 0 & 1 \\
0 & -1 & -5 & -24
\end{array}\right]
$$
 
**Paso 2:** $R_3 \to R_3 - R_2$
 
$$
\left[\begin{array}{ccc|c}
5 & -5 & -1 & -30 \\
0 & -1 & 0 & 1 \\
0 & 0 & -5 & -25
\end{array}\right]
$$
 
**Paso 3:** $R_3 \to \frac{1}{5}R_3$
 
$$
\left[\begin{array}{ccc|c}
5 & -5 & -1 & -30 \\
0 & -1 & 0 & 1 \\
0 & 0 & -1 & -5
\end{array}\right]
$$
 
La matriz ya es escalonada (ceros debajo de la diagonal). Ahora resuelvo de la última fila a la primera.
 
**Sustitución hacia atrás:**
 
Fila 3:
 
$$
\begin{aligned}
-c &= -5 \\
c &= 5
\end{aligned}
$$
 
Fila 2:
 
$$
\begin{aligned}
-b &= 1 \\
b &= -1
\end{aligned}
$$
 
Fila 1:
 
$$
\begin{aligned}
5a-5b-c &= -30 \\
5a-5(-1)-(5) &= -30 \\
5a &= -30 \\
a &= -6
\end{aligned}
$$
 
**Solución:** $a=-6$, $b=-1$, $c=5$
 
 
---
 
## 2. Método de Gauss-Jordan · Ejercicios 45-52
 
> **Procedimiento:**
>
> 1. Escribo la matriz aumentada $[A \mid b]$.
> 2. En cada columna: convierto el pivote (elemento de la diagonal) en $1$ y hago ceros **arriba y abajo** de él.
> 3. Cuando a la izquierda queda la matriz identidad, la última columna es la solución.
>
> En Gauss-Jordan no hace falta sustituir hacia atrás: la solución se lee directamente.
>
> **Casos especiales:**
>
> - Si aparece una fila $0\ 0\ 0 \mid d$ con $d \neq 0$, equivale a $0=d$: el sistema **no tiene solución**.
> - Si aparece una fila completa de ceros $0\ 0\ 0 \mid 0$, queda una variable libre y el sistema tiene **infinitas soluciones**.
>
> Si el pivote es $0$ o conviene evitar fracciones, se intercambian filas ($R_i \leftrightarrow R_j$).
 
 
#### Ejercicio 45
 
**Sistema:**
 
$$
\begin{aligned}
4r-5s-t &= -20 \\
-r+2s+t &= -1 \\
-r+s &= -4
\end{aligned}
$$
 
**Matriz aumentada:**
 
$$
\left[\begin{array}{ccc|c}
4 & -5 & -1 & -20 \\
-1 & 2 & 1 & -1 \\
-1 & 1 & 0 & -4
\end{array}\right]
$$
 
**Paso 1:** $R_1 \leftrightarrow R_2$
 
$$
\left[\begin{array}{ccc|c}
-1 & 2 & 1 & -1 \\
4 & -5 & -1 & -20 \\
-1 & 1 & 0 & -4
\end{array}\right]
$$
 
**Paso 2:** $R_1 \to -R_1$
 
$$
\left[\begin{array}{ccc|c}
1 & -2 & -1 & 1 \\
4 & -5 & -1 & -20 \\
-1 & 1 & 0 & -4
\end{array}\right]
$$
 
**Paso 3:** $R_2 \to R_2 - 4R_1,\ R_3 \to R_3 + R_1$
 
$$
\left[\begin{array}{ccc|c}
1 & -2 & -1 & 1 \\
0 & 3 & 3 & -24 \\
0 & -1 & -1 & -3
\end{array}\right]
$$
 
**Paso 4:** $R_2 \leftrightarrow R_3$
 
$$
\left[\begin{array}{ccc|c}
1 & -2 & -1 & 1 \\
0 & -1 & -1 & -3 \\
0 & 3 & 3 & -24
\end{array}\right]
$$
 
**Paso 5:** $R_2 \to -R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & -2 & -1 & 1 \\
0 & 1 & 1 & 3 \\
0 & 3 & 3 & -24
\end{array}\right]
$$
 
**Paso 6:** $R_1 \to R_1 + 2R_2,\ R_3 \to R_3 - 3R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & 1 & 7 \\
0 & 1 & 1 & 3 \\
0 & 0 & 0 & -33
\end{array}\right]
$$
 
La última fila quedó como $0\ 0\ 0 \mid d$ con $d \neq 0$, es decir, $0 = d$, que es imposible.
 
**Solución:** el sistema **no tiene solución**.
 
 
#### Ejercicio 46
 
**Sistema:**
 
$$
\begin{aligned}
-5a-5b+5c &= 10 \\
-6a-2c &= -16 \\
-6a+c &= -19
\end{aligned}
$$
 
**Matriz aumentada:**
 
$$
\left[\begin{array}{ccc|c}
-5 & -5 & 5 & 10 \\
-6 & 0 & -2 & -16 \\
-6 & 0 & 1 & -19
\end{array}\right]
$$
 
**Paso 1:** $R_1 \to -\frac{1}{5}R_1$
 
$$
\left[\begin{array}{ccc|c}
1 & 1 & -1 & -2 \\
-6 & 0 & -2 & -16 \\
-6 & 0 & 1 & -19
\end{array}\right]
$$
 
**Paso 2:** $R_2 \to R_2 + 6R_1,\ R_3 \to R_3 + 6R_1$
 
$$
\left[\begin{array}{ccc|c}
1 & 1 & -1 & -2 \\
0 & 6 & -8 & -28 \\
0 & 6 & -5 & -31
\end{array}\right]
$$
 
**Paso 3:** $R_2 \to \frac{1}{6}R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & 1 & -1 & -2 \\
0 & 1 & -\frac{4}{3} & -\frac{14}{3} \\
0 & 6 & -5 & -31
\end{array}\right]
$$
 
**Paso 4:** $R_1 \to R_1 - R_2,\ R_3 \to R_3 - 6R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & \frac{1}{3} & \frac{8}{3} \\
0 & 1 & -\frac{4}{3} & -\frac{14}{3} \\
0 & 0 & 3 & -3
\end{array}\right]
$$
 
**Paso 5:** $R_3 \to \frac{1}{3}R_3$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & \frac{1}{3} & \frac{8}{3} \\
0 & 1 & -\frac{4}{3} & -\frac{14}{3} \\
0 & 0 & 1 & -1
\end{array}\right]
$$
 
**Paso 6:** $R_1 \to R_1 - \frac{1}{3}R_3,\ R_2 \to R_2 + \frac{4}{3}R_3$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & 0 & 3 \\
0 & 1 & 0 & -6 \\
0 & 0 & 1 & -1
\end{array}\right]
$$
 
A la izquierda quedó la identidad, así que la última columna es la solución.
 
**Solución:** $a=3$, $b=-6$, $c=-1$
 
 
#### Ejercicio 47
 
**Sistema:**
 
$$
\begin{aligned}
-3b-2c &= -26 \\
a+2c &= 1 \\
2a-3b+2c &= 3
\end{aligned}
$$
 
**Matriz aumentada:**
 
$$
\left[\begin{array}{ccc|c}
0 & -3 & -2 & -26 \\
1 & 0 & 2 & 1 \\
2 & -3 & 2 & 3
\end{array}\right]
$$
 
**Paso 1:** $R_1 \leftrightarrow R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & 2 & 1 \\
0 & -3 & -2 & -26 \\
2 & -3 & 2 & 3
\end{array}\right]
$$
 
**Paso 2:** $R_3 \to R_3 - 2R_1$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & 2 & 1 \\
0 & -3 & -2 & -26 \\
0 & -3 & -2 & 1
\end{array}\right]
$$
 
**Paso 3:** $R_2 \to -\frac{1}{3}R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & 2 & 1 \\
0 & 1 & \frac{2}{3} & \frac{26}{3} \\
0 & -3 & -2 & 1
\end{array}\right]
$$
 
**Paso 4:** $R_3 \to R_3 + 3R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & 2 & 1 \\
0 & 1 & \frac{2}{3} & \frac{26}{3} \\
0 & 0 & 0 & 27
\end{array}\right]
$$
 
La última fila quedó como $0\ 0\ 0 \mid d$ con $d \neq 0$, es decir, $0 = d$, que es imposible.
 
**Solución:** el sistema **no tiene solución**.
 
 
#### Ejercicio 48
 
**Sistema:**
 
$$
\begin{aligned}
3r-t &= 8 \\
-2r+s &= -5 \\
-3r-3s+5t &= -1
\end{aligned}
$$
 
**Matriz aumentada:**
 
$$
\left[\begin{array}{ccc|c}
3 & 0 & -1 & 8 \\
-2 & 1 & 0 & -5 \\
-3 & -3 & 5 & -1
\end{array}\right]
$$
 
**Paso 1:** $R_1 \to \frac{1}{3}R_1$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & -\frac{1}{3} & \frac{8}{3} \\
-2 & 1 & 0 & -5 \\
-3 & -3 & 5 & -1
\end{array}\right]
$$
 
**Paso 2:** $R_2 \to R_2 + 2R_1,\ R_3 \to R_3 + 3R_1$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & -\frac{1}{3} & \frac{8}{3} \\
0 & 1 & -\frac{2}{3} & \frac{1}{3} \\
0 & -3 & 4 & 7
\end{array}\right]
$$
 
**Paso 3:** $R_3 \to R_3 + 3R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & -\frac{1}{3} & \frac{8}{3} \\
0 & 1 & -\frac{2}{3} & \frac{1}{3} \\
0 & 0 & 2 & 8
\end{array}\right]
$$
 
**Paso 4:** $R_3 \to \frac{1}{2}R_3$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & -\frac{1}{3} & \frac{8}{3} \\
0 & 1 & -\frac{2}{3} & \frac{1}{3} \\
0 & 0 & 1 & 4
\end{array}\right]
$$
 
**Paso 5:** $R_1 \to R_1 + \frac{1}{3}R_3,\ R_2 \to R_2 + \frac{2}{3}R_3$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & 0 & 4 \\
0 & 1 & 0 & 3 \\
0 & 0 & 1 & 4
\end{array}\right]
$$
 
A la izquierda quedó la identidad, así que la última columna es la solución.
 
**Solución:** $r=4$, $s=3$, $t=4$
 
 
#### Ejercicio 49
 
**Sistema:**
 
$$
\begin{aligned}
-6y+3z &= 15 \\
-3x-6y &= -6 \\
x-6y+4z &= 22
\end{aligned}
$$
 
**Matriz aumentada:**
 
$$
\left[\begin{array}{ccc|c}
0 & -6 & 3 & 15 \\
-3 & -6 & 0 & -6 \\
1 & -6 & 4 & 22
\end{array}\right]
$$
 
**Paso 1:** $R_1 \leftrightarrow R_3$
 
$$
\left[\begin{array}{ccc|c}
1 & -6 & 4 & 22 \\
-3 & -6 & 0 & -6 \\
0 & -6 & 3 & 15
\end{array}\right]
$$
 
**Paso 2:** $R_2 \to R_2 + 3R_1$
 
$$
\left[\begin{array}{ccc|c}
1 & -6 & 4 & 22 \\
0 & -24 & 12 & 60 \\
0 & -6 & 3 & 15
\end{array}\right]
$$
 
**Paso 3:** $R_2 \to -\frac{1}{24}R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & -6 & 4 & 22 \\
0 & 1 & -\frac{1}{2} & -\frac{5}{2} \\
0 & -6 & 3 & 15
\end{array}\right]
$$
 
**Paso 4:** $R_1 \to R_1 + 6R_2,\ R_3 \to R_3 + 6R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & 1 & 7 \\
0 & 1 & -\frac{1}{2} & -\frac{5}{2} \\
0 & 0 & 0 & 0
\end{array}\right]
$$
 
Quedó una fila de ceros: el sistema tiene **infinitas soluciones**. La variable sin pivote ($z$) es libre y puede valer cualquier número real; las demás se escriben en función de ella:
 
$$
\begin{aligned}
x &= 7-z \\
y &= -\frac{5}{2}+\frac{1}{2}z
\end{aligned}
$$
 
**Solución:** infinitas soluciones, con $z$ libre: $x=7-z$, $y=-\frac{5}{2}+\frac{1}{2}z$.
 
 
#### Ejercicio 50
 
**Sistema:**
 
$$
\begin{aligned}
-3s &= 3 \\
2r-2s-6t &= -6 \\
5r+s+4t &= -21
\end{aligned}
$$
 
**Matriz aumentada:**
 
$$
\left[\begin{array}{ccc|c}
0 & -3 & 0 & 3 \\
2 & -2 & -6 & -6 \\
5 & 1 & 4 & -21
\end{array}\right]
$$
 
**Paso 1:** $R_1 \leftrightarrow R_2$
 
$$
\left[\begin{array}{ccc|c}
2 & -2 & -6 & -6 \\
0 & -3 & 0 & 3 \\
5 & 1 & 4 & -21
\end{array}\right]
$$
 
**Paso 2:** $R_1 \to \frac{1}{2}R_1$
 
$$
\left[\begin{array}{ccc|c}
1 & -1 & -3 & -3 \\
0 & -3 & 0 & 3 \\
5 & 1 & 4 & -21
\end{array}\right]
$$
 
**Paso 3:** $R_3 \to R_3 - 5R_1$
 
$$
\left[\begin{array}{ccc|c}
1 & -1 & -3 & -3 \\
0 & -3 & 0 & 3 \\
0 & 6 & 19 & -6
\end{array}\right]
$$
 
**Paso 4:** $R_2 \to -\frac{1}{3}R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & -1 & -3 & -3 \\
0 & 1 & 0 & -1 \\
0 & 6 & 19 & -6
\end{array}\right]
$$
 
**Paso 5:** $R_1 \to R_1 + R_2,\ R_3 \to R_3 - 6R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & -3 & -4 \\
0 & 1 & 0 & -1 \\
0 & 0 & 19 & 0
\end{array}\right]
$$
 
**Paso 6:** $R_3 \to \frac{1}{19}R_3$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & -3 & -4 \\
0 & 1 & 0 & -1 \\
0 & 0 & 1 & 0
\end{array}\right]
$$
 
**Paso 7:** $R_1 \to R_1 + 3R_3$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & 0 & -4 \\
0 & 1 & 0 & -1 \\
0 & 0 & 1 & 0
\end{array}\right]
$$
 
A la izquierda quedó la identidad, así que la última columna es la solución.
 
**Solución:** $r=-4$, $s=-1$, $t=0$
 
 
#### Ejercicio 51
 
**Sistema:**
 
$$
\begin{aligned}
-5r+t &= -16 \\
-2r+2s+t &= -7 \\
5r+2s+4t &= 11
\end{aligned}
$$
 
**Matriz aumentada:**
 
$$
\left[\begin{array}{ccc|c}
-5 & 0 & 1 & -16 \\
-2 & 2 & 1 & -7 \\
5 & 2 & 4 & 11
\end{array}\right]
$$
 
**Paso 1:** $R_1 \to -\frac{1}{5}R_1$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & -\frac{1}{5} & \frac{16}{5} \\
-2 & 2 & 1 & -7 \\
5 & 2 & 4 & 11
\end{array}\right]
$$
 
**Paso 2:** $R_2 \to R_2 + 2R_1,\ R_3 \to R_3 - 5R_1$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & -\frac{1}{5} & \frac{16}{5} \\
0 & 2 & \frac{3}{5} & -\frac{3}{5} \\
0 & 2 & 5 & -5
\end{array}\right]
$$
 
**Paso 3:** $R_2 \to \frac{1}{2}R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & -\frac{1}{5} & \frac{16}{5} \\
0 & 1 & \frac{3}{10} & -\frac{3}{10} \\
0 & 2 & 5 & -5
\end{array}\right]
$$
 
**Paso 4:** $R_3 \to R_3 - 2R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & -\frac{1}{5} & \frac{16}{5} \\
0 & 1 & \frac{3}{10} & -\frac{3}{10} \\
0 & 0 & \frac{22}{5} & -\frac{22}{5}
\end{array}\right]
$$
 
**Paso 5:** $R_3 \to \frac{5}{22}R_3$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & -\frac{1}{5} & \frac{16}{5} \\
0 & 1 & \frac{3}{10} & -\frac{3}{10} \\
0 & 0 & 1 & -1
\end{array}\right]
$$
 
**Paso 6:** $R_1 \to R_1 + \frac{1}{5}R_3,\ R_2 \to R_2 - \frac{3}{10}R_3$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & 0 & 3 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & -1
\end{array}\right]
$$
 
A la izquierda quedó la identidad, así que la última columna es la solución.
 
**Solución:** $r=3$, $s=0$, $t=-1$
 
 
#### Ejercicio 52
 
**Sistema:**
 
$$
\begin{aligned}
x+y-5z &= 11 \\
-x-2y-3z &= 7 \\
6x-5y &= 28
\end{aligned}
$$
 
**Matriz aumentada:**
 
$$
\left[\begin{array}{ccc|c}
1 & 1 & -5 & 11 \\
-1 & -2 & -3 & 7 \\
6 & -5 & 0 & 28
\end{array}\right]
$$
 
**Paso 1:** $R_2 \to R_2 + R_1,\ R_3 \to R_3 - 6R_1$
 
$$
\left[\begin{array}{ccc|c}
1 & 1 & -5 & 11 \\
0 & -1 & -8 & 18 \\
0 & -11 & 30 & -38
\end{array}\right]
$$
 
**Paso 2:** $R_2 \to -R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & 1 & -5 & 11 \\
0 & 1 & 8 & -18 \\
0 & -11 & 30 & -38
\end{array}\right]
$$
 
**Paso 3:** $R_1 \to R_1 - R_2,\ R_3 \to R_3 + 11R_2$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & -13 & 29 \\
0 & 1 & 8 & -18 \\
0 & 0 & 118 & -236
\end{array}\right]
$$
 
**Paso 4:** $R_3 \to \frac{1}{118}R_3$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & -13 & 29 \\
0 & 1 & 8 & -18 \\
0 & 0 & 1 & -2
\end{array}\right]
$$
 
**Paso 5:** $R_1 \to R_1 + 13R_3,\ R_2 \to R_2 - 8R_3$
 
$$
\left[\begin{array}{ccc|c}
1 & 0 & 0 & 3 \\
0 & 1 & 0 & -2 \\
0 & 0 & 1 & -2
\end{array}\right]
$$
 
A la izquierda quedó la identidad, así que la última columna es la solución.
 
**Solución:** $x=3$, $y=-2$, $z=-2$
 
