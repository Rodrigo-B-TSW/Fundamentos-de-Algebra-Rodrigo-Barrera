# Actividad #26. Matrices: Suma, Resta y Multiplicación
 
| DATOS | |
| :--- | :--- |
| **Alumno** | Rodrigo Barrera García |
| **Profesor** | Jorge Javier Pedrozo Romero |
| **Materia** | Fundamentos de Álgebra |
| **Fecha** | 16/11/2026 |
| **Lugar** | Mérida, Yucatán. México |
 
### NOTA: La organización y el diseño en html/markdown fueron utilizadas herramientas de inteligencia artificial como apoyo, los procedimientos de cada ejercicio fueron hechos de manera personal y de lo aprendido en clase.
--- 

## 1. Suma y resta de matrices · Ejercicios 1-4

#### Ejercicio 1

$$
\begin{bmatrix}
-6 \\
-2 \\
-6 \\
-3
\end{bmatrix} + \begin{bmatrix}
5 \\
-4 \\
-5 \\
6
\end{bmatrix} + \begin{bmatrix}
6 \\
2 \\
6 \\
-3
\end{bmatrix} \rightarrow \begin{bmatrix}
-6+5+6 \\
-2+(-4)+2 \\
-6+(-5)+6 \\
-3+6+(-3)
\end{bmatrix}
$$

$$
\rightarrow \begin{bmatrix}
5 \\
-2-4+2 \\
-6-5+6 \\
-3+6-3
\end{bmatrix} \rightarrow \begin{bmatrix}
5 \\
-4 \\
-5 \\
0
\end{bmatrix}
$$


#### Ejercicio 2

$$
\begin{bmatrix}
-1 & 3 \\
-6 & -1
\end{bmatrix} - \left( \begin{bmatrix}
4 & 5 \\
0 & -6
\end{bmatrix} - \begin{bmatrix}
-3 & -3 \\
6 & -4
\end{bmatrix} \right)
$$

$$
\rightarrow \begin{bmatrix}
-1 & 3 \\
-6 & -1
\end{bmatrix} - \left( \begin{bmatrix}
4-(-3) & 5-(-3) \\
0-6 & -6-(-4)
\end{bmatrix} \right) \rightarrow \begin{bmatrix}
4+3 & 5+3 \\
0-6 & -6+4
\end{bmatrix}
$$

$$
= \begin{bmatrix}
-1 & 3 \\
-6 & -1
\end{bmatrix} - \begin{bmatrix}
7 & 8 \\
-6 & -2
\end{bmatrix} = \begin{bmatrix}
-1-7 & 3-8 \\
-6-(-6) & -1-(-2)
\end{bmatrix} = \begin{bmatrix}
-8 & -5 \\
0 & 1
\end{bmatrix}
$$


#### Ejercicio 3

$$
\begin{bmatrix}
-4 & 6 & -3 & 5
\end{bmatrix} - \begin{bmatrix}
-4 & -5 & -5 & 3
\end{bmatrix} + \begin{bmatrix}
4 & 4 & 5 & -5
\end{bmatrix}
$$

$$
\begin{aligned}
&=\left[-4-(-4)+4,\ 6-(-5)+4,\ -3-(-5)+5,\ 5-3+(-5)\right] \\
&=\left[-4+4+4,\ 6+5+4,\ -3+5+5,\ 5-3-5\right] \\
&=\begin{bmatrix}
4 & 15 & 7 & -3
\end{bmatrix}
\end{aligned}
$$


#### Ejercicio 4

$$
\begin{bmatrix}
0 & 0
\end{bmatrix} - \begin{bmatrix}
5 & 4
\end{bmatrix} + \begin{bmatrix}
-4 & -3
\end{bmatrix}
$$

$$
\begin{aligned}
&=\left[0-5+(-4),\ 0-4+(-3)\right]=\left[0-5-4,\ 0-4-3\right] \\
&=\begin{bmatrix}
-9 & -7
\end{bmatrix}
\end{aligned}
$$


---

## 2. Multiplicación de un escalar por una matriz · Ejercicios 5-8

#### Ejercicio 5

$$
-3 \left( -2 \begin{bmatrix}
-5 & 2 & 2 & -5
\end{bmatrix} \right)
$$

$$
= -3 \begin{bmatrix}
10 & -4 & -4 & 10
\end{bmatrix} = \begin{bmatrix}
-30 & 12 & 12 & -30
\end{bmatrix}
$$


#### Ejercicio 6

$$
5 \left( -4 \begin{bmatrix}
2 & -2 & 0
\end{bmatrix} \right)
$$

$$
= 5 \begin{bmatrix}
-8 & 8 & 0
\end{bmatrix} = \begin{bmatrix}
-40 & 40 & 0
\end{bmatrix}
$$


#### Ejercicio 7

$$
5 \left( 2 \begin{bmatrix}
-2 & -4 \\
-1 & -5 \\
-1 & -5
\end{bmatrix} \right) = 10 \begin{bmatrix}
-2 & -4 \\
-1 & -5 \\
-1 & -5
\end{bmatrix} = \begin{bmatrix}
-20 & -40 \\
-10 & -50 \\
-10 & -50
\end{bmatrix}
$$


#### Ejercicio 8

$$
-3 \left( 3 \begin{bmatrix}
6 \\
-1
\end{bmatrix} \right) = -3\times3=-9 \begin{bmatrix}
6 \\
-1
\end{bmatrix} = \begin{bmatrix}
-54 \\
9
\end{bmatrix}
$$


---

## 3. Multiplicación de matrices · Ejercicios 9-12

#### Ejercicio 9

$$
\begin{bmatrix}
0 & 5 \\
2 & -4
\end{bmatrix} \cdot \left( \begin{bmatrix}
4 & 0 \\
2 & 1
\end{bmatrix} \cdot \begin{bmatrix}
-2 & 1 & 2 & -3 \\
4 & -2 & 3 & 2
\end{bmatrix} \right)
$$

**Dimensiones:** $A = 2\times2$, $B = 2\times4$ $\rightarrow$ resultado $2\times4 = 8$ elementos

$$
\begin{aligned}
C_{11} &= 4(-2)+0(4) = -8+0 = -8 \\
C_{12} &= 4(1)+0(-2) = 4+0 = 4 \\
C_{13} &= 4(2)+0(3) = 8+0 = 8 \\
C_{14} &= 4(-3)+0(2) = -12+0 = -12 \\
C_{21} &= 2(-2)+1(4) = -4+4 = 0 \\
C_{22} &= 2(1)+1(-2) = 2+(-2) = 2-2 = 0 \\
C_{23} &= 2(2)+1(3) = 4+3 = 7 \\
C_{24} &= 2(-3)+1(2) = -6+2 = -4
\end{aligned}
$$

$$
= \begin{bmatrix}
-8 & 4 & 8 & -12 \\
0 & 0 & 7 & -4
\end{bmatrix} \rightarrow \begin{bmatrix}
0 & 5 \\
2 & -4
\end{bmatrix} \cdot \begin{bmatrix}
-8 & 4 & 8 & -12 \\
0 & 0 & 7 & -4
\end{bmatrix}
$$


$$
\begin{aligned}
D_{11} &= 0(-8)+5(0) = 0+0 = 0 \\
D_{12} &= 0(4)+5(0) = 0+0 = 0 \\
D_{13} &= 0(8)+(7)5 = 0+35 = 35 \\
D_{14} &= 0(-12)+(-4)5 = 0-20 = -20 \\
D_{21} &= 2(-8)+(-4)(0) = -16+0 = -16 \\
D_{22} &= 2(4)+(-4)(0) = 8+0 = 8 \\
D_{23} &= 2(8)+(-4)(7) = 16-28 = -12 \\
D_{24} &= 2(-12)+(-4)(-4) = -24+16 = -8
\end{aligned}
$$

$$
= \begin{bmatrix}
0 & 0 & 35 & -20 \\
-16 & 8 & -12 & -8
\end{bmatrix}
$$


#### Ejercicio 10

$$
\begin{bmatrix}
1 & 2 \\
3 & -4 \\
2 & -4
\end{bmatrix} \cdot \left( \begin{bmatrix}
4 & 2 \\
2 & -5
\end{bmatrix} \cdot \begin{bmatrix}
-1 & 3 \\
1 & 2
\end{bmatrix} \right)
$$

**Dimensiones:** $A = 2\times2$, $B = 2\times2$ $\rightarrow$ resultado $2\times2 = 4$ elementos

$$
\begin{aligned}
C_{11} &= 4(-1)+2(1) = -4+2 = -2 \\
C_{12} &= 4(3)+2(2) = 12+4 = 16 \\
C_{21} &= 2(-1)+(-5)(1) = -2-5 = -7 \\
C_{22} &= 2(3)+(-5)(2) = 6-10 = -4
\end{aligned}
$$

$$
= \begin{bmatrix}
-2 & 16 \\
-7 & -4
\end{bmatrix} \rightarrow \begin{bmatrix}
1 & 2 \\
3 & -4 \\
2 & -4
\end{bmatrix} \cdot \begin{bmatrix}
-2 & 16 \\
-7 & -4
\end{bmatrix}
$$

**Dimensiones:** $A = 3\times2$, $B = 2\times2$ $\rightarrow$ resultado $3\times2 = 6$ elementos

$$
\begin{aligned}
D_{11} &= 1(-2)+2(-7) = -2-14 = -16 \\
D_{12} &= 1(16)+2(-4) = 16-8 = 8 \\
D_{21} &= 3(-2)+(-4)(-7) = -6+28 = 22 \\
D_{22} &= 3(16)+(-4)(-4) = 48+16 = 64 \\
D_{31} &= 2(-2)+(-4)(-7) = -4+28 = 24 \\
D_{32} &= 2(16)+(-4)(-4) = 32+16 = 48
\end{aligned}
$$

$$
= \begin{bmatrix}
-16 & 8 \\
22 & 64 \\
24 & 48
\end{bmatrix}
$$


#### Ejercicio 11

$$
\begin{bmatrix}
5 & -2 & 5 & 6 \\
1 & -5 & 6 & 4
\end{bmatrix} \cdot \left( \begin{bmatrix}
3 & 1 \\
4 & -1 \\
-1 & -3 \\
-2 & -1
\end{bmatrix} \cdot \begin{bmatrix}
0 & 1 \\
-1 & 0
\end{bmatrix} \right)
$$

**Dimensiones:** $A = 4\times2$, $B = 2\times2$ $\rightarrow$ resultado $4\times2 = 8$ elementos

$$
\begin{aligned}
C_{11} &= 3(0)+1(-1) = 0-1 = -1 \\
C_{12} &= 3(1)+1(0) = 3+0 = 3 \\
C_{21} &= 4(0)+(-1)(-1) = 0+1 = 1 \\
C_{22} &= 4(1)+(-1)(0) = 4+0 = 4 \\
C_{31} &= -1(0)+(-3)(-1) = 0+3 = 3 \\
C_{32} &= -1(1)+(-3)(0) = -1+0 = -1 \\
C_{41} &= -2(0)+(-1)(-1) = 0+1 = 1 \\
C_{42} &= -2(1)+(-1)(0) = -2+0 = -2
\end{aligned}
$$

$$
= \begin{bmatrix}
-1 & 3 \\
1 & 4 \\
3 & -1 \\
1 & -2
\end{bmatrix} \rightarrow \begin{bmatrix}
5 & -2 & 5 & 6 \\
1 & -5 & 6 & 4
\end{bmatrix} \cdot \begin{bmatrix}
-1 & 3 \\
1 & 4 \\
3 & -1 \\
1 & -2
\end{bmatrix}
$$

**Dimensiones:** $A = 2\times4$, $B = 4\times2$ $\rightarrow$ resultado $2\times2 = 4$ elementos

$$
\begin{aligned}
D_{11} &= 5(-1)+(-2)(1)+5(3)+6(1) = -5-2+15+6 = 14 \\
D_{12} &= 5(3)+(-2)(4)+5(-1)+6(-2) = 15-8-5-12 = -10 \\
D_{21} &= 1(-1)+(-5)(1)+6(3)+4(1) = -1-5+18+4 = 16 \\
D_{22} &= 1(3)+(-5)(4)+6(-1)+4(-2) = 3-20-6-8 = -31
\end{aligned}
$$

$$
= \begin{bmatrix}
14 & -10 \\
16 & -31
\end{bmatrix}
$$


#### Ejercicio 12

$$
\begin{bmatrix}
0 & -4 \\
1 & -4 \\
-1 & 5 \\
-3 & 4
\end{bmatrix} \cdot \left( \begin{bmatrix}
-3 & -1 & -2 & 3 \\
-1 & -4 & -3 & 5
\end{bmatrix} \cdot \begin{bmatrix}
4 & 0 \\
1 & -5 \\
2 & 5 \\
2 & 1
\end{bmatrix} \right)
$$

**Dimensiones:** $A = 2\times4$, $B = 4\times2$ $\rightarrow$ resultado $2\times2 = 4$ elementos

$$
\begin{aligned}
C_{11} &= -3(4)+(-1)(1)+(-2)(2)+3(2) = -12-1-4+6 = -11 \\
C_{12} &= -3(0)+(-1)(-5)+(-2)(5)+3(1) = 0+5-10+3 = -2 \\
C_{21} &= -1(4)+(-4)(1)+(-3)(2)+5(2) = -4-4-6+10 = -4 \\
C_{22} &= -1(0)+(-4)(-5)+(-3)(5)+5(1) = 0+20-15+5 = 10
\end{aligned}
$$

$$
= \begin{bmatrix}
-11 & -2 \\
-4 & 10
\end{bmatrix} \rightarrow \begin{bmatrix}
0 & -4 \\
1 & -4 \\
-1 & 5 \\
-3 & 4
\end{bmatrix} \cdot \begin{bmatrix}
-11 & -2 \\
-4 & 10
\end{bmatrix}
$$

**Dimensiones:** $A = 4\times2$, $B = 2\times2$ $\rightarrow$ resultado $4\times2 = 8$ elementos

$$
\begin{aligned}
D_{11} &= 0(-11)+(-4)(-4) = 0+16 = 16 \\
D_{12} &= 0(-2)+(-4)(10) = 0-40 = -40 \\
D_{21} &= 1(-11)+(-4)(-4) = -11+16 = 5 \\
D_{22} &= 1(-2)+(-4)(10) = -2-40 = -42 \\
D_{31} &= -1(-11)+5(-4) = 11-20 = -9 \\
D_{32} &= -1(-2)+5(10) = 2+50 = 52 \\
D_{41} &= -3(-11)+4(-4) = 33-16 = 17 \\
D_{42} &= -3(-2)+4(10) = 6+40 = 46
\end{aligned}
$$

$$
= \begin{bmatrix}
16 & -40 \\
5 & -42 \\
-9 & 52 \\
17 & 46
\end{bmatrix}
$$


---

