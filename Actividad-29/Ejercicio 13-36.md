# Actividad #29. Matrices: Determinantes
 
| DATOS | |
| :--- | :--- |
| **Alumno** | Rodrigo Barrera García |
| **Profesor** | Jorge Javier Pedrozo Romero |
| **Materia** | Fundamentos de Álgebra |
| **Fecha** | 19/11/2026 |
| **Lugar** | Mérida, Yucatán. México |
 
### NOTA: La organización y el diseño en html/markdown fueron utilizadas herramientas de inteligencia artificial como apoyo, los procedimientos de cada ejercicio fueron hechos de manera personal y de lo aprendido en clase.
--- 

## 1. Matriz inversa · Ejercicios 13-20

> **Método (cofactores):**
>
> $A^{-1}=\dfrac{1}{\det A}\,\operatorname{adj}(A)$, donde $\operatorname{adj}(A)=C^{T}$ y $C$ es la matriz de cofactores.
>
> 1. Calculo cada cofactor $C_{ij}=(-1)^{i+j}M_{ij}$. El menor $M_{ij}$ es un determinante de $2\times2$ (se quita la fila $i$ y la columna $j$). Si sus filas son $(a,\ b)$ y $(c,\ d)$, su determinante es $ad-bc$.
> 2. Armo la matriz de cofactores $C$.
> 3. Calculo $\det A$ desarrollando por la fila 1: $\det A=a_{11}C_{11}+a_{12}C_{12}+a_{13}C_{13}$.
> 4. La adjunta es la transpuesta de $C$ (las filas pasan a ser columnas).
> 5. Divido la adjunta entre el determinante: $A^{-1}=\dfrac{1}{\det A}\operatorname{adj}(A)$.
>
> **Signos** $(-1)^{i+j}$ en una matriz $3\times3$: fila 1: $+\ -\ +$, fila 2: $-\ +\ -$, fila 3: $+\ -\ +$.
>
> Si $\det A=0$, la matriz **no tiene inversa**.


#### Ejercicio 13

$$
A= \begin{bmatrix}
3 & -4 & -1 \\
-1 & 2 & 2 \\
-3 & -1 & 2
\end{bmatrix}
$$

**Cofactores** (cada menor de $2\times2$ se calcula con $ad-bc$):

$$
C_{11}=(-1)^{1+1} \begin{vmatrix}
2 & 2 \\
-1 & 2
\end{vmatrix} =(+1)\left[(2)(2)-(2)(-1)\right]=(+1)(6)=6
$$

$$
C_{12}=(-1)^{1+2} \begin{vmatrix}
-1 & 2 \\
-3 & 2
\end{vmatrix} =(-1)\left[(-1)(2)-(2)(-3)\right]=(-1)(4)=-4
$$

$$
C_{13}=(-1)^{1+3} \begin{vmatrix}
-1 & 2 \\
-3 & -1
\end{vmatrix} =(+1)\left[(-1)(-1)-(2)(-3)\right]=(+1)(7)=7
$$

$$
C_{21}=(-1)^{2+1} \begin{vmatrix}
-4 & -1 \\
-1 & 2
\end{vmatrix} =(-1)\left[(-4)(2)-(-1)(-1)\right]=(-1)(-9)=9
$$

$$
C_{22}=(-1)^{2+2} \begin{vmatrix}
3 & -1 \\
-3 & 2
\end{vmatrix} =(+1)\left[(3)(2)-(-1)(-3)\right]=(+1)(3)=3
$$

$$
C_{23}=(-1)^{2+3} \begin{vmatrix}
3 & -4 \\
-3 & -1
\end{vmatrix} =(-1)\left[(3)(-1)-(-4)(-3)\right]=(-1)(-15)=15
$$

$$
C_{31}=(-1)^{3+1} \begin{vmatrix}
-4 & -1 \\
2 & 2
\end{vmatrix} =(+1)\left[(-4)(2)-(-1)(2)\right]=(+1)(-6)=-6
$$

$$
C_{32}=(-1)^{3+2} \begin{vmatrix}
3 & -1 \\
-1 & 2
\end{vmatrix} =(-1)\left[(3)(2)-(-1)(-1)\right]=(-1)(5)=-5
$$

$$
C_{33}=(-1)^{3+3} \begin{vmatrix}
3 & -4 \\
-1 & 2
\end{vmatrix} =(+1)\left[(3)(2)-(-4)(-1)\right]=(+1)(2)=2
$$

**Matriz de cofactores:**

$$
C= \begin{bmatrix}
6 & -4 & 7 \\
9 & 3 & 15 \\
-6 & -5 & 2
\end{bmatrix}
$$

**Determinante** (desarrollo por la fila 1):

$$
\begin{aligned}
\det A &= (3)(6)+(-4)(-4)+(-1)(7) \\
&= 18+16-7 = 27
\end{aligned}
$$

**Adjunta** (transpuesta de $C$):

$$
\operatorname{adj}(A)=C^{T}= \begin{bmatrix}
6 & 9 & -6 \\
-4 & 3 & -5 \\
7 & 15 & 2
\end{bmatrix}
$$

**Inversa:**

$$
A^{-1}=\frac{1}{\det A}\operatorname{adj}(A)= \frac{1}{27} \begin{bmatrix}
6 & 9 & -6 \\
-4 & 3 & -5 \\
7 & 15 & 2
\end{bmatrix}
$$

**Resultado:**

$$
A^{-1}= \begin{bmatrix}
\frac{2}{9} & \frac{1}{3} & -\frac{2}{9} \\
-\frac{4}{27} & \frac{1}{9} & -\frac{5}{27} \\
\frac{7}{27} & \frac{5}{9} & \frac{2}{27}
\end{bmatrix}
$$


#### Ejercicio 14

$$
A= \begin{bmatrix}
3 & 0 & 2 \\
4 & 5 & -2 \\
-1 & -3 & -4
\end{bmatrix}
$$

**Cofactores** (cada menor de $2\times2$ se calcula con $ad-bc$):

$$
C_{11}=(-1)^{1+1} \begin{vmatrix}
5 & -2 \\
-3 & -4
\end{vmatrix} =(+1)\left[(5)(-4)-(-2)(-3)\right]=(+1)(-26)=-26
$$

$$
C_{12}=(-1)^{1+2} \begin{vmatrix}
4 & -2 \\
-1 & -4
\end{vmatrix} =(-1)\left[(4)(-4)-(-2)(-1)\right]=(-1)(-18)=18
$$

$$
C_{13}=(-1)^{1+3} \begin{vmatrix}
4 & 5 \\
-1 & -3
\end{vmatrix} =(+1)\left[(4)(-3)-(5)(-1)\right]=(+1)(-7)=-7
$$

$$
C_{21}=(-1)^{2+1} \begin{vmatrix}
0 & 2 \\
-3 & -4
\end{vmatrix} =(-1)\left[(0)(-4)-(2)(-3)\right]=(-1)(6)=-6
$$

$$
C_{22}=(-1)^{2+2} \begin{vmatrix}
3 & 2 \\
-1 & -4
\end{vmatrix} =(+1)\left[(3)(-4)-(2)(-1)\right]=(+1)(-10)=-10
$$

$$
C_{23}=(-1)^{2+3} \begin{vmatrix}
3 & 0 \\
-1 & -3
\end{vmatrix} =(-1)\left[(3)(-3)-(0)(-1)\right]=(-1)(-9)=9
$$

$$
C_{31}=(-1)^{3+1} \begin{vmatrix}
0 & 2 \\
5 & -2
\end{vmatrix} =(+1)\left[(0)(-2)-(2)(5)\right]=(+1)(-10)=-10
$$

$$
C_{32}=(-1)^{3+2} \begin{vmatrix}
3 & 2 \\
4 & -2
\end{vmatrix} =(-1)\left[(3)(-2)-(2)(4)\right]=(-1)(-14)=14
$$

$$
C_{33}=(-1)^{3+3} \begin{vmatrix}
3 & 0 \\
4 & 5
\end{vmatrix} =(+1)\left[(3)(5)-(0)(4)\right]=(+1)(15)=15
$$

**Matriz de cofactores:**

$$
C= \begin{bmatrix}
-26 & 18 & -7 \\
-6 & -10 & 9 \\
-10 & 14 & 15
\end{bmatrix}
$$

**Determinante** (desarrollo por la fila 1):

$$
\begin{aligned}
\det A &= (3)(-26)+(0)(18)+(2)(-7) \\
&= -78+0-14 = -92
\end{aligned}
$$

**Adjunta** (transpuesta de $C$):

$$
\operatorname{adj}(A)=C^{T}= \begin{bmatrix}
-26 & -6 & -10 \\
18 & -10 & 14 \\
-7 & 9 & 15
\end{bmatrix}
$$

**Inversa:**

$$
A^{-1}=\frac{1}{\det A}\operatorname{adj}(A)= -\frac{1}{92} \begin{bmatrix}
-26 & -6 & -10 \\
18 & -10 & 14 \\
-7 & 9 & 15
\end{bmatrix}
$$

**Resultado:**

$$
A^{-1}= \begin{bmatrix}
\frac{13}{46} & \frac{3}{46} & \frac{5}{46} \\
-\frac{9}{46} & \frac{5}{46} & -\frac{7}{46} \\
\frac{7}{92} & -\frac{9}{92} & -\frac{15}{92}
\end{bmatrix}
$$


#### Ejercicio 15

$$
A= \begin{bmatrix}
-1 & 4 & -4 \\
0 & -3 & 4 \\
0 & 0 & 0
\end{bmatrix}
$$

Primero calculo los cofactores de la fila 1, que son los que se necesitan para el determinante:

$$
C_{11}=(-1)^{1+1} \begin{vmatrix}
-3 & 4 \\
0 & 0
\end{vmatrix} =(+1)\left[(-3)(0)-(4)(0)\right]=(+1)(0)=0
$$

$$
C_{12}=(-1)^{1+2} \begin{vmatrix}
0 & 4 \\
0 & 0
\end{vmatrix} =(-1)\left[(0)(0)-(4)(0)\right]=(-1)(0)=0
$$

$$
C_{13}=(-1)^{1+3} \begin{vmatrix}
0 & -3 \\
0 & 0
\end{vmatrix} =(+1)\left[(0)(0)-(-3)(0)\right]=(+1)(0)=0
$$

$$
\begin{aligned}
\det A &= (-1)(0)+(4)(0)+(-4)(0) \\
&= 0+0+0 = 0
\end{aligned}
$$

**Resultado:** como $\det A = 0$, la matriz $A$ **no tiene inversa**.


#### Ejercicio 16

$$
A= \begin{bmatrix}
6 & -5 & 1 \\
-4 & 6 & -3 \\
2 & 6 & -2
\end{bmatrix}
$$

**Cofactores** (cada menor de $2\times2$ se calcula con $ad-bc$):

$$
C_{11}=(-1)^{1+1} \begin{vmatrix}
6 & -3 \\
6 & -2
\end{vmatrix} =(+1)\left[(6)(-2)-(-3)(6)\right]=(+1)(6)=6
$$

$$
C_{12}=(-1)^{1+2} \begin{vmatrix}
-4 & -3 \\
2 & -2
\end{vmatrix} =(-1)\left[(-4)(-2)-(-3)(2)\right]=(-1)(14)=-14
$$

$$
C_{13}=(-1)^{1+3} \begin{vmatrix}
-4 & 6 \\
2 & 6
\end{vmatrix} =(+1)\left[(-4)(6)-(6)(2)\right]=(+1)(-36)=-36
$$

$$
C_{21}=(-1)^{2+1} \begin{vmatrix}
-5 & 1 \\
6 & -2
\end{vmatrix} =(-1)\left[(-5)(-2)-(1)(6)\right]=(-1)(4)=-4
$$

$$
C_{22}=(-1)^{2+2} \begin{vmatrix}
6 & 1 \\
2 & -2
\end{vmatrix} =(+1)\left[(6)(-2)-(1)(2)\right]=(+1)(-14)=-14
$$

$$
C_{23}=(-1)^{2+3} \begin{vmatrix}
6 & -5 \\
2 & 6
\end{vmatrix} =(-1)\left[(6)(6)-(-5)(2)\right]=(-1)(46)=-46
$$

$$
C_{31}=(-1)^{3+1} \begin{vmatrix}
-5 & 1 \\
6 & -3
\end{vmatrix} =(+1)\left[(-5)(-3)-(1)(6)\right]=(+1)(9)=9
$$

$$
C_{32}=(-1)^{3+2} \begin{vmatrix}
6 & 1 \\
-4 & -3
\end{vmatrix} =(-1)\left[(6)(-3)-(1)(-4)\right]=(-1)(-14)=14
$$

$$
C_{33}=(-1)^{3+3} \begin{vmatrix}
6 & -5 \\
-4 & 6
\end{vmatrix} =(+1)\left[(6)(6)-(-5)(-4)\right]=(+1)(16)=16
$$

**Matriz de cofactores:**

$$
C= \begin{bmatrix}
6 & -14 & -36 \\
-4 & -14 & -46 \\
9 & 14 & 16
\end{bmatrix}
$$

**Determinante** (desarrollo por la fila 1):

$$
\begin{aligned}
\det A &= (6)(6)+(-5)(-14)+(1)(-36) \\
&= 36+70-36 = 70
\end{aligned}
$$

**Adjunta** (transpuesta de $C$):

$$
\operatorname{adj}(A)=C^{T}= \begin{bmatrix}
6 & -4 & 9 \\
-14 & -14 & 14 \\
-36 & -46 & 16
\end{bmatrix}
$$

**Inversa:**

$$
A^{-1}=\frac{1}{\det A}\operatorname{adj}(A)= \frac{1}{70} \begin{bmatrix}
6 & -4 & 9 \\
-14 & -14 & 14 \\
-36 & -46 & 16
\end{bmatrix}
$$

**Resultado:**

$$
A^{-1}= \begin{bmatrix}
\frac{3}{35} & -\frac{2}{35} & \frac{9}{70} \\
-\frac{1}{5} & -\frac{1}{5} & \frac{1}{5} \\
-\frac{18}{35} & -\frac{23}{35} & \frac{8}{35}
\end{bmatrix}
$$


#### Ejercicio 17

$$
A= \begin{bmatrix}
1 & -5 & -5 \\
7 & -3 & -1 \\
-2 & -6 & 0
\end{bmatrix}
$$

**Cofactores** (cada menor de $2\times2$ se calcula con $ad-bc$):

$$
C_{11}=(-1)^{1+1} \begin{vmatrix}
-3 & -1 \\
-6 & 0
\end{vmatrix} =(+1)\left[(-3)(0)-(-1)(-6)\right]=(+1)(-6)=-6
$$

$$
C_{12}=(-1)^{1+2} \begin{vmatrix}
7 & -1 \\
-2 & 0
\end{vmatrix} =(-1)\left[(7)(0)-(-1)(-2)\right]=(-1)(-2)=2
$$

$$
C_{13}=(-1)^{1+3} \begin{vmatrix}
7 & -3 \\
-2 & -6
\end{vmatrix} =(+1)\left[(7)(-6)-(-3)(-2)\right]=(+1)(-48)=-48
$$

$$
C_{21}=(-1)^{2+1} \begin{vmatrix}
-5 & -5 \\
-6 & 0
\end{vmatrix} =(-1)\left[(-5)(0)-(-5)(-6)\right]=(-1)(-30)=30
$$

$$
C_{22}=(-1)^{2+2} \begin{vmatrix}
1 & -5 \\
-2 & 0
\end{vmatrix} =(+1)\left[(1)(0)-(-5)(-2)\right]=(+1)(-10)=-10
$$

$$
C_{23}=(-1)^{2+3} \begin{vmatrix}
1 & -5 \\
-2 & -6
\end{vmatrix} =(-1)\left[(1)(-6)-(-5)(-2)\right]=(-1)(-16)=16
$$

$$
C_{31}=(-1)^{3+1} \begin{vmatrix}
-5 & -5 \\
-3 & -1
\end{vmatrix} =(+1)\left[(-5)(-1)-(-5)(-3)\right]=(+1)(-10)=-10
$$

$$
C_{32}=(-1)^{3+2} \begin{vmatrix}
1 & -5 \\
7 & -1
\end{vmatrix} =(-1)\left[(1)(-1)-(-5)(7)\right]=(-1)(34)=-34
$$

$$
C_{33}=(-1)^{3+3} \begin{vmatrix}
1 & -5 \\
7 & -3
\end{vmatrix} =(+1)\left[(1)(-3)-(-5)(7)\right]=(+1)(32)=32
$$

**Matriz de cofactores:**

$$
C= \begin{bmatrix}
-6 & 2 & -48 \\
30 & -10 & 16 \\
-10 & -34 & 32
\end{bmatrix}
$$

**Determinante** (desarrollo por la fila 1):

$$
\begin{aligned}
\det A &= (1)(-6)+(-5)(2)+(-5)(-48) \\
&= -6-10+240 = 224
\end{aligned}
$$

**Adjunta** (transpuesta de $C$):

$$
\operatorname{adj}(A)=C^{T}= \begin{bmatrix}
-6 & 30 & -10 \\
2 & -10 & -34 \\
-48 & 16 & 32
\end{bmatrix}
$$

**Inversa:**

$$
A^{-1}=\frac{1}{\det A}\operatorname{adj}(A)= \frac{1}{224} \begin{bmatrix}
-6 & 30 & -10 \\
2 & -10 & -34 \\
-48 & 16 & 32
\end{bmatrix}
$$

**Resultado:**

$$
A^{-1}= \begin{bmatrix}
-\frac{3}{112} & \frac{15}{112} & -\frac{5}{112} \\
\frac{1}{112} & -\frac{5}{112} & -\frac{17}{112} \\
-\frac{3}{14} & \frac{1}{14} & \frac{1}{7}
\end{bmatrix}
$$


#### Ejercicio 18

$$
A= \begin{bmatrix}
-5 & 1 & -4 \\
-3 & -6 & -4 \\
-1 & -1 & -4
\end{bmatrix}
$$

**Cofactores** (cada menor de $2\times2$ se calcula con $ad-bc$):

$$
C_{11}=(-1)^{1+1} \begin{vmatrix}
-6 & -4 \\
-1 & -4
\end{vmatrix} =(+1)\left[(-6)(-4)-(-4)(-1)\right]=(+1)(20)=20
$$

$$
C_{12}=(-1)^{1+2} \begin{vmatrix}
-3 & -4 \\
-1 & -4
\end{vmatrix} =(-1)\left[(-3)(-4)-(-4)(-1)\right]=(-1)(8)=-8
$$

$$
C_{13}=(-1)^{1+3} \begin{vmatrix}
-3 & -6 \\
-1 & -1
\end{vmatrix} =(+1)\left[(-3)(-1)-(-6)(-1)\right]=(+1)(-3)=-3
$$

$$
C_{21}=(-1)^{2+1} \begin{vmatrix}
1 & -4 \\
-1 & -4
\end{vmatrix} =(-1)\left[(1)(-4)-(-4)(-1)\right]=(-1)(-8)=8
$$

$$
C_{22}=(-1)^{2+2} \begin{vmatrix}
-5 & -4 \\
-1 & -4
\end{vmatrix} =(+1)\left[(-5)(-4)-(-4)(-1)\right]=(+1)(16)=16
$$

$$
C_{23}=(-1)^{2+3} \begin{vmatrix}
-5 & 1 \\
-1 & -1
\end{vmatrix} =(-1)\left[(-5)(-1)-(1)(-1)\right]=(-1)(6)=-6
$$

$$
C_{31}=(-1)^{3+1} \begin{vmatrix}
1 & -4 \\
-6 & -4
\end{vmatrix} =(+1)\left[(1)(-4)-(-4)(-6)\right]=(+1)(-28)=-28
$$

$$
C_{32}=(-1)^{3+2} \begin{vmatrix}
-5 & -4 \\
-3 & -4
\end{vmatrix} =(-1)\left[(-5)(-4)-(-4)(-3)\right]=(-1)(8)=-8
$$

$$
C_{33}=(-1)^{3+3} \begin{vmatrix}
-5 & 1 \\
-3 & -6
\end{vmatrix} =(+1)\left[(-5)(-6)-(1)(-3)\right]=(+1)(33)=33
$$

**Matriz de cofactores:**

$$
C= \begin{bmatrix}
20 & -8 & -3 \\
8 & 16 & -6 \\
-28 & -8 & 33
\end{bmatrix}
$$

**Determinante** (desarrollo por la fila 1):

$$
\begin{aligned}
\det A &= (-5)(20)+(1)(-8)+(-4)(-3) \\
&= -100-8+12 = -96
\end{aligned}
$$

**Adjunta** (transpuesta de $C$):

$$
\operatorname{adj}(A)=C^{T}= \begin{bmatrix}
20 & 8 & -28 \\
-8 & 16 & -8 \\
-3 & -6 & 33
\end{bmatrix}
$$

**Inversa:**

$$
A^{-1}=\frac{1}{\det A}\operatorname{adj}(A)= -\frac{1}{96} \begin{bmatrix}
20 & 8 & -28 \\
-8 & 16 & -8 \\
-3 & -6 & 33
\end{bmatrix}
$$

**Resultado:**

$$
A^{-1}= \begin{bmatrix}
-\frac{5}{24} & -\frac{1}{12} & \frac{7}{24} \\
\frac{1}{12} & -\frac{1}{6} & \frac{1}{12} \\
\frac{1}{32} & \frac{1}{16} & -\frac{11}{32}
\end{bmatrix}
$$


#### Ejercicio 19

$$
A= \begin{bmatrix}
-1 & -1 & -3 \\
-6 & -6 & -3 \\
3 & 6 & -2
\end{bmatrix}
$$

**Cofactores** (cada menor de $2\times2$ se calcula con $ad-bc$):

$$
C_{11}=(-1)^{1+1} \begin{vmatrix}
-6 & -3 \\
6 & -2
\end{vmatrix} =(+1)\left[(-6)(-2)-(-3)(6)\right]=(+1)(30)=30
$$

$$
C_{12}=(-1)^{1+2} \begin{vmatrix}
-6 & -3 \\
3 & -2
\end{vmatrix} =(-1)\left[(-6)(-2)-(-3)(3)\right]=(-1)(21)=-21
$$

$$
C_{13}=(-1)^{1+3} \begin{vmatrix}
-6 & -6 \\
3 & 6
\end{vmatrix} =(+1)\left[(-6)(6)-(-6)(3)\right]=(+1)(-18)=-18
$$

$$
C_{21}=(-1)^{2+1} \begin{vmatrix}
-1 & -3 \\
6 & -2
\end{vmatrix} =(-1)\left[(-1)(-2)-(-3)(6)\right]=(-1)(20)=-20
$$

$$
C_{22}=(-1)^{2+2} \begin{vmatrix}
-1 & -3 \\
3 & -2
\end{vmatrix} =(+1)\left[(-1)(-2)-(-3)(3)\right]=(+1)(11)=11
$$

$$
C_{23}=(-1)^{2+3} \begin{vmatrix}
-1 & -1 \\
3 & 6
\end{vmatrix} =(-1)\left[(-1)(6)-(-1)(3)\right]=(-1)(-3)=3
$$

$$
C_{31}=(-1)^{3+1} \begin{vmatrix}
-1 & -3 \\
-6 & -3
\end{vmatrix} =(+1)\left[(-1)(-3)-(-3)(-6)\right]=(+1)(-15)=-15
$$

$$
C_{32}=(-1)^{3+2} \begin{vmatrix}
-1 & -3 \\
-6 & -3
\end{vmatrix} =(-1)\left[(-1)(-3)-(-3)(-6)\right]=(-1)(-15)=15
$$

$$
C_{33}=(-1)^{3+3} \begin{vmatrix}
-1 & -1 \\
-6 & -6
\end{vmatrix} =(+1)\left[(-1)(-6)-(-1)(-6)\right]=(+1)(0)=0
$$

**Matriz de cofactores:**

$$
C= \begin{bmatrix}
30 & -21 & -18 \\
-20 & 11 & 3 \\
-15 & 15 & 0
\end{bmatrix}
$$

**Determinante** (desarrollo por la fila 1):

$$
\begin{aligned}
\det A &= (-1)(30)+(-1)(-21)+(-3)(-18) \\
&= -30+21+54 = 45
\end{aligned}
$$

**Adjunta** (transpuesta de $C$):

$$
\operatorname{adj}(A)=C^{T}= \begin{bmatrix}
30 & -20 & -15 \\
-21 & 11 & 15 \\
-18 & 3 & 0
\end{bmatrix}
$$

**Inversa:**

$$
A^{-1}=\frac{1}{\det A}\operatorname{adj}(A)= \frac{1}{45} \begin{bmatrix}
30 & -20 & -15 \\
-21 & 11 & 15 \\
-18 & 3 & 0
\end{bmatrix}
$$

**Resultado:**

$$
A^{-1}= \begin{bmatrix}
\frac{2}{3} & -\frac{4}{9} & -\frac{1}{3} \\
-\frac{7}{15} & \frac{11}{45} & \frac{1}{3} \\
-\frac{2}{5} & \frac{1}{15} & 0
\end{bmatrix}
$$


#### Ejercicio 20

$$
A= \begin{bmatrix}
-2 & 2 & -2 \\
5 & -2 & 1 \\
-1 & 5 & 3
\end{bmatrix}
$$

**Cofactores** (cada menor de $2\times2$ se calcula con $ad-bc$):

$$
C_{11}=(-1)^{1+1} \begin{vmatrix}
-2 & 1 \\
5 & 3
\end{vmatrix} =(+1)\left[(-2)(3)-(1)(5)\right]=(+1)(-11)=-11
$$

$$
C_{12}=(-1)^{1+2} \begin{vmatrix}
5 & 1 \\
-1 & 3
\end{vmatrix} =(-1)\left[(5)(3)-(1)(-1)\right]=(-1)(16)=-16
$$

$$
C_{13}=(-1)^{1+3} \begin{vmatrix}
5 & -2 \\
-1 & 5
\end{vmatrix} =(+1)\left[(5)(5)-(-2)(-1)\right]=(+1)(23)=23
$$

$$
C_{21}=(-1)^{2+1} \begin{vmatrix}
2 & -2 \\
5 & 3
\end{vmatrix} =(-1)\left[(2)(3)-(-2)(5)\right]=(-1)(16)=-16
$$

$$
C_{22}=(-1)^{2+2} \begin{vmatrix}
-2 & -2 \\
-1 & 3
\end{vmatrix} =(+1)\left[(-2)(3)-(-2)(-1)\right]=(+1)(-8)=-8
$$

$$
C_{23}=(-1)^{2+3} \begin{vmatrix}
-2 & 2 \\
-1 & 5
\end{vmatrix} =(-1)\left[(-2)(5)-(2)(-1)\right]=(-1)(-8)=8
$$

$$
C_{31}=(-1)^{3+1} \begin{vmatrix}
2 & -2 \\
-2 & 1
\end{vmatrix} =(+1)\left[(2)(1)-(-2)(-2)\right]=(+1)(-2)=-2
$$

$$
C_{32}=(-1)^{3+2} \begin{vmatrix}
-2 & -2 \\
5 & 1
\end{vmatrix} =(-1)\left[(-2)(1)-(-2)(5)\right]=(-1)(8)=-8
$$

$$
C_{33}=(-1)^{3+3} \begin{vmatrix}
-2 & 2 \\
5 & -2
\end{vmatrix} =(+1)\left[(-2)(-2)-(2)(5)\right]=(+1)(-6)=-6
$$

**Matriz de cofactores:**

$$
C= \begin{bmatrix}
-11 & -16 & 23 \\
-16 & -8 & 8 \\
-2 & -8 & -6
\end{bmatrix}
$$

**Determinante** (desarrollo por la fila 1):

$$
\begin{aligned}
\det A &= (-2)(-11)+(2)(-16)+(-2)(23) \\
&= 22-32-46 = -56
\end{aligned}
$$

**Adjunta** (transpuesta de $C$):

$$
\operatorname{adj}(A)=C^{T}= \begin{bmatrix}
-11 & -16 & -2 \\
-16 & -8 & -8 \\
23 & 8 & -6
\end{bmatrix}
$$

**Inversa:**

$$
A^{-1}=\frac{1}{\det A}\operatorname{adj}(A)= -\frac{1}{56} \begin{bmatrix}
-11 & -16 & -2 \\
-16 & -8 & -8 \\
23 & 8 & -6
\end{bmatrix}
$$

**Resultado:**

$$
A^{-1}= \begin{bmatrix}
\frac{11}{56} & \frac{2}{7} & \frac{1}{28} \\
\frac{2}{7} & \frac{1}{7} & \frac{1}{7} \\
-\frac{23}{56} & -\frac{1}{7} & \frac{3}{28}
\end{bmatrix}
$$


---

## 2. Determinante por la regla de Sarrus · Ejercicios 21-28

> **Regla de Sarrus** (matrices $3\times3$): se repiten las dos primeras columnas a la derecha.
>
> - Diagonales principales (de arriba hacia abajo, se **suman**): $a_{11}a_{22}a_{33}+a_{12}a_{23}a_{31}+a_{13}a_{21}a_{32}$
> - Diagonales secundarias (de abajo hacia arriba, se **restan**): $a_{13}a_{22}a_{31}+a_{11}a_{23}a_{32}+a_{12}a_{21}a_{33}$
>
> $\det A = (\text{suma de principales}) - (\text{suma de secundarias})$


#### Ejercicio 21

$$
\left|\begin{array}{ccc|cc}
-6 & 0 & -3 & -6 & 0 \\
3 & 4 & -8 & 3 & 4 \\
10 & 7 & 11 & 10 & 7
\end{array}\right|
$$

$$
\begin{aligned}
D_{+} &= (-6)(4)(11)+(0)(-8)(10)+(-3)(3)(7) \\
&= -264+0-63 = -327
\end{aligned}
$$

$$
\begin{aligned}
D_{-} &= (-3)(4)(10)+(-6)(-8)(7)+(0)(3)(11) \\
&= -120+336+0 = 216
\end{aligned}
$$

$$
\begin{aligned}
\det A &= D_{+} - D_{-} = -327-(216) = -543
\end{aligned}
$$

**Resultado:** $\det A = -543$


#### Ejercicio 22

$$
\left|\begin{array}{ccc|cc}
10 & -5 & 0 & 10 & -5 \\
7 & -2 & -1 & 7 & -2 \\
5 & -3 & 1 & 5 & -3
\end{array}\right|
$$

$$
\begin{aligned}
D_{+} &= (10)(-2)(1)+(-5)(-1)(5)+(0)(7)(-3) \\
&= -20+25+0 = 5
\end{aligned}
$$

$$
\begin{aligned}
D_{-} &= (0)(-2)(5)+(10)(-1)(-3)+(-5)(7)(1) \\
&= 0+30-35 = -5
\end{aligned}
$$

$$
\begin{aligned}
\det A &= D_{+} - D_{-} = 5-(-5) = 10
\end{aligned}
$$

**Resultado:** $\det A = 10$


#### Ejercicio 23

$$
\left|\begin{array}{ccc|cc}
-9 & 11 & 5 & -9 & 11 \\
9 & 10 & 0 & 9 & 10 \\
-2 & 9 & 10 & -2 & 9
\end{array}\right|
$$

$$
\begin{aligned}
D_{+} &= (-9)(10)(10)+(11)(0)(-2)+(5)(9)(9) \\
&= -900+0+405 = -495
\end{aligned}
$$

$$
\begin{aligned}
D_{-} &= (5)(10)(-2)+(-9)(0)(9)+(11)(9)(10) \\
&= -100+0+990 = 890
\end{aligned}
$$

$$
\begin{aligned}
\det A &= D_{+} - D_{-} = -495-(890) = -1385
\end{aligned}
$$

**Resultado:** $\det A = -1385$


#### Ejercicio 24

$$
\left|\begin{array}{ccc|cc}
5 & -7 & 12 & 5 & -7 \\
-11 & -5 & 7 & -11 & -5 \\
1 & 10 & 11 & 1 & 10
\end{array}\right|
$$

$$
\begin{aligned}
D_{+} &= (5)(-5)(11)+(-7)(7)(1)+(12)(-11)(10) \\
&= -275-49-1320 = -1644
\end{aligned}
$$

$$
\begin{aligned}
D_{-} &= (12)(-5)(1)+(5)(7)(10)+(-7)(-11)(11) \\
&= -60+350+847 = 1137
\end{aligned}
$$

$$
\begin{aligned}
\det A &= D_{+} - D_{-} = -1644-(1137) = -2781
\end{aligned}
$$

**Resultado:** $\det A = -2781$


#### Ejercicio 25

$$
\left|\begin{array}{ccc|cc}
-8 & 5 & 11 & -8 & 5 \\
2 & 1 & 10 & 2 & 1 \\
2 & 12 & 4 & 2 & 12
\end{array}\right|
$$

$$
\begin{aligned}
D_{+} &= (-8)(1)(4)+(5)(10)(2)+(11)(2)(12) \\
&= -32+100+264 = 332
\end{aligned}
$$

$$
\begin{aligned}
D_{-} &= (11)(1)(2)+(-8)(10)(12)+(5)(2)(4) \\
&= 22-960+40 = -898
\end{aligned}
$$

$$
\begin{aligned}
\det A &= D_{+} - D_{-} = 332-(-898) = 1230
\end{aligned}
$$

**Resultado:** $\det A = 1230$


#### Ejercicio 26

$$
\left|\begin{array}{ccc|cc}
-7 & 8 & 2 & -7 & 8 \\
1 & -3 & 2 & 1 & -3 \\
0 & 4 & 1 & 0 & 4
\end{array}\right|
$$

$$
\begin{aligned}
D_{+} &= (-7)(-3)(1)+(8)(2)(0)+(2)(1)(4) \\
&= 21+0+8 = 29
\end{aligned}
$$

$$
\begin{aligned}
D_{-} &= (2)(-3)(0)+(-7)(2)(4)+(8)(1)(1) \\
&= 0-56+8 = -48
\end{aligned}
$$

$$
\begin{aligned}
\det A &= D_{+} - D_{-} = 29-(-48) = 77
\end{aligned}
$$

**Resultado:** $\det A = 77$


#### Ejercicio 27

$$
\left|\begin{array}{ccc|cc}
-6 & -4 & -11 & -6 & -4 \\
3 & -9 & 6 & 3 & -9 \\
-12 & 1 & -11 & -12 & 1
\end{array}\right|
$$

$$
\begin{aligned}
D_{+} &= (-6)(-9)(-11)+(-4)(6)(-12)+(-11)(3)(1) \\
&= -594+288-33 = -339
\end{aligned}
$$

$$
\begin{aligned}
D_{-} &= (-11)(-9)(-12)+(-6)(6)(1)+(-4)(3)(-11) \\
&= -1188-36+132 = -1092
\end{aligned}
$$

$$
\begin{aligned}
\det A &= D_{+} - D_{-} = -339-(-1092) = 753
\end{aligned}
$$

**Resultado:** $\det A = 753$


#### Ejercicio 28

$$
\left|\begin{array}{ccc|cc}
0 & 12 & 3 & 0 & 12 \\
6 & 6 & -4 & 6 & 6 \\
-7 & -3 & -8 & -7 & -3
\end{array}\right|
$$

$$
\begin{aligned}
D_{+} &= (0)(6)(-8)+(12)(-4)(-7)+(3)(6)(-3) \\
&= 0+336-54 = 282
\end{aligned}
$$

$$
\begin{aligned}
D_{-} &= (3)(6)(-7)+(0)(-4)(-3)+(12)(6)(-8) \\
&= -126+0-576 = -702
\end{aligned}
$$

$$
\begin{aligned}
\det A &= D_{+} - D_{-} = 282-(-702) = 984
\end{aligned}
$$

**Resultado:** $\det A = 984$


---

## 3. Determinante por cofactores · Ejercicios 29-36

> **Desarrollo por cofactores:** el determinante es la suma de cada elemento de una fila (o columna) por su cofactor:
>
> $|A| = \sum a_{ij}C_{ij}$, con $C_{ij}=(-1)^{i+j}M_{ij}$
>
> $M_{ij}$ (menor) es el determinante de la matriz que queda al quitar la fila $i$ y la columna $j$.
>
> **Signos** $(-1)^{i+j}$: alternan empezando con $+$ en la esquina superior izquierda.
>
> **Procedimiento:**
>
> 1. Elijo la fila o columna con más ceros (los términos con $0$ se anulan).
> 2. Planteo el desarrollo con los elementos distintos de cero.
> 3. Cada menor $M_{ij}$ es de $4\times4$: lo desarrollo otra vez por su fila o columna con más ceros.
> 4. Los menores de $3\times3$ ($N_{ij}$) se calculan con Sarrus, escribiendo solo los productos: diagonales principales $-$ (diagonales secundarias).
> 5. Sumo los términos.


#### Ejercicio 29

$$
|A|= \begin{vmatrix}
-6 & 1 & 5 & 8 & -7 \\
3 & 9 & 9 & -3 & -6 \\
6 & 5 & 0 & -10 & -5 \\
4 & 0 & -1 & -3 & -7 \\
9 & 10 & 2 & -10 & -4
\end{vmatrix}
$$

**Desarrollo por la fila 3** (tiene 1 cero, quedan 4 términos):

$$
\begin{aligned}
|A| &= (6)(-1)^{3+1}M_{31}+(5)(-1)^{3+2}M_{32}+(-10)(-1)^{3+4}M_{34}+(-5)(-1)^{3+5}M_{35} \\
&= (6)(+1)(-3420)+(5)(-1)(189)+(-10)(-1)(3033)+(-5)(+1)(-639) \\
&= 12060
\end{aligned}
$$

**Cálculo de cada menor:**

Menor $M_{31}$ (se quita la fila 3 y la columna 1):

$$
M_{31}= \begin{vmatrix}
1 & 5 & 8 & -7 \\
9 & 9 & -3 & -6 \\
0 & -1 & -3 & -7 \\
10 & 2 & -10 & -4
\end{vmatrix}
$$

Desarrollo por la fila 3:

$$
\begin{aligned}
|N_{32}| &= 12-480+630-(210+60-288) = 180 \\
|N_{33}| &= -36-300-126-(-630-12-180) = 360 \\
|N_{34}| &= -90-150+144-(720-6-450) = -360 \\
M_{31} &= (-1)(-1)(180)+(-3)(+1)(360)+(-7)(-1)(-360) = -3420
\end{aligned}
$$

Menor $M_{32}$ (se quita la fila 3 y la columna 2):

$$
M_{32}= \begin{vmatrix}
-6 & 5 & 8 & -7 \\
3 & 9 & -3 & -6 \\
4 & -1 & -3 & -7 \\
9 & 2 & -10 & -4
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= 108+42-60-(36+630-12) = -564 \\
|N_{12}| &= 36+189+240-(162+210+48) = 45 \\
|N_{13}| &= 12-567-48-(54-42-144) = -471 \\
|N_{14}| &= 30-243-24-(27-18-360) = 114 \\
M_{32} &= (-6)(+1)(-564)+(5)(-1)(45)+(8)(+1)(-471)+(-7)(-1)(114) = 189
\end{aligned}
$$

Menor $M_{34}$ (se quita la fila 3 y la columna 4):

$$
M_{34}= \begin{vmatrix}
-6 & 1 & 5 & -7 \\
3 & 9 & 9 & -6 \\
4 & 0 & -1 & -7 \\
9 & 10 & 2 & -4
\end{vmatrix}
$$

Desarrollo por la fila 3:

$$
\begin{aligned}
|N_{31}| &= -36-300-126-(-630-12-180) = 360 \\
|N_{33}| &= 216-54-210-(-567+360-12) = 171 \\
|N_{34}| &= -108+81+150-(405-540+6) = 252 \\
M_{34} &= (4)(+1)(360)+(-1)(+1)(171)+(-7)(-1)(252) = 3033
\end{aligned}
$$

Menor $M_{35}$ (se quita la fila 3 y la columna 5):

$$
M_{35}= \begin{vmatrix}
-6 & 1 & 5 & 8 \\
3 & 9 & 9 & -3 \\
4 & 0 & -1 & -3 \\
9 & 10 & 2 & -10
\end{vmatrix}
$$

Desarrollo por la fila 3:

$$
\begin{aligned}
|N_{31}| &= -90-150+144-(720-6-450) = -360 \\
|N_{33}| &= 540-27+240-(648+180-30) = -45 \\
|N_{34}| &= -108+81+150-(405-540+6) = 252 \\
M_{35} &= (4)(+1)(-360)+(-1)(+1)(-45)+(-3)(-1)(252) = -639
\end{aligned}
$$

**Resultado:** $|A| = 12060$


#### Ejercicio 30

$$
|A|= \begin{vmatrix}
-8 & -9 & 9 & 0 & 0 \\
4 & -9 & 4 & -1 & 7 \\
4 & -7 & -3 & 7 & -1 \\
2 & 9 & 5 & 7 & -4 \\
-9 & -10 & 5 & -3 & 4
\end{vmatrix}
$$

**Desarrollo por la fila 1** (tiene 2 ceros, quedan 3 términos):

$$
\begin{aligned}
|A| &= (-8)(-1)^{1+1}M_{11}+(-9)(-1)^{1+2}M_{12}+(9)(-1)^{1+3}M_{13} \\
&= (-8)(+1)(-4611)+(-9)(-1)(-4437)+(9)(+1)(-5394) \\
&= -51591
\end{aligned}
$$

**Cálculo de cada menor:**

Menor $M_{11}$ (se quita la fila 1 y la columna 1):

$$
M_{11}= \begin{vmatrix}
-9 & 4 & -1 & 7 \\
-7 & -3 & 7 & -1 \\
9 & 5 & 7 & -4 \\
-10 & 5 & -3 & 4
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= -84-140+15-(-35-36+140) = -278 \\
|N_{12}| &= -196+280+27-(70-84+252) = -127 \\
|N_{13}| &= -140-120-45-(50+140-108) = -387 \\
|N_{14}| &= 105+210+315-(-350-245+81) = 1144 \\
M_{11} &= (-9)(+1)(-278)+(4)(-1)(-127)+(-1)(+1)(-387)+(7)(-1)(1144) = -4611
\end{aligned}
$$

Menor $M_{12}$ (se quita la fila 1 y la columna 2):

$$
M_{12}= \begin{vmatrix}
4 & 4 & -1 & 7 \\
4 & -3 & 7 & -1 \\
2 & 5 & 7 & -4 \\
-9 & 5 & -3 & 4
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= -84-140+15-(-35-36+140) = -278 \\
|N_{12}| &= 112+252+6-(63+48+56) = 203 \\
|N_{13}| &= 80-108-10-(45-80-24) = 21 \\
|N_{14}| &= -60+189+70-(-315+140+18) = 356 \\
M_{12} &= (4)(+1)(-278)+(4)(-1)(203)+(-1)(+1)(21)+(7)(-1)(356) = -4437
\end{aligned}
$$

Menor $M_{13}$ (se quita la fila 1 y la columna 3):

$$
M_{13}= \begin{vmatrix}
4 & -9 & -1 & 7 \\
4 & -7 & 7 & -1 \\
2 & 9 & 7 & -4 \\
-9 & -10 & -3 & 4
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= -196+280+27-(70-84+252) = -127 \\
|N_{12}| &= 112+252+6-(63+48+56) = 203 \\
|N_{13}| &= 144-252+20-(81+160-56) = -273 \\
|N_{14}| &= -108+441-140-(-567-280+42) = 998 \\
M_{13} &= (4)(+1)(-127)+(-9)(-1)(203)+(-1)(+1)(-273)+(7)(-1)(998) = -5394
\end{aligned}
$$

**Resultado:** $|A| = -51591$


#### Ejercicio 31

$$
|A|= \begin{vmatrix}
3 & 2 & 7 & -8 & -10 \\
-1 & 6 & 6 & 0 & -2 \\
-1 & 5 & 2 & -9 & 2 \\
0 & 3 & 5 & 2 & -7 \\
-2 & 8 & 0 & 9 & 10
\end{vmatrix}
$$

**Desarrollo por la fila 2** (tiene 1 cero, quedan 4 términos):

$$
\begin{aligned}
|A| &= (-1)(-1)^{2+1}M_{21}+(6)(-1)^{2+2}M_{22}+(6)(-1)^{2+3}M_{23}+(-2)(-1)^{2+5}M_{25} \\
&= (-1)(-1)(-1419)+(6)(+1)(2111)+(6)(-1)(3217)+(-2)(-1)(1396) \\
&= -5263
\end{aligned}
$$

**Cálculo de cada menor:**

Menor $M_{21}$ (se quita la fila 2 y la columna 1):

$$
M_{21}= \begin{vmatrix}
2 & 7 & -8 & -10 \\
5 & 2 & -9 & 2 \\
3 & 5 & 2 & -7 \\
8 & 0 & 9 & 10
\end{vmatrix}
$$

Desarrollo por la fila 4:

$$
\begin{aligned}
|N_{41}| &= 441-80-40-(450+28+112) = -269 \\
|N_{43}| &= -28+42-250-(-60+20-245) = 49 \\
|N_{44}| &= 8-189-200-(-48-90+70) = -313 \\
M_{21} &= (8)(-1)(-269)+(9)(-1)(49)+(10)(+1)(-313) = -1419
\end{aligned}
$$

Menor $M_{22}$ (se quita la fila 2 y la columna 2):

$$
M_{22}= \begin{vmatrix}
3 & 7 & -8 & -10 \\
-1 & 2 & -9 & 2 \\
0 & 5 & 2 & -7 \\
-2 & 0 & 9 & 10
\end{vmatrix}
$$

Desarrollo por la fila 3:

$$
\begin{aligned}
|N_{32}| &= -270+32+90-(-180+54+80) = -102 \\
|N_{33}| &= 60-28+0-(40+0-70) = 62 \\
|N_{34}| &= 54+126+0-(32+0-63) = 211 \\
M_{22} &= (5)(-1)(-102)+(2)(+1)(62)+(-7)(-1)(211) = 2111
\end{aligned}
$$

Menor $M_{23}$ (se quita la fila 2 y la columna 3):

$$
M_{23}= \begin{vmatrix}
3 & 2 & -8 & -10 \\
-1 & 5 & -9 & 2 \\
0 & 3 & 2 & -7 \\
-2 & 8 & 9 & 10
\end{vmatrix}
$$

Desarrollo por la fila 3:

$$
\begin{aligned}
|N_{32}| &= -270+32+90-(-180+54+80) = -102 \\
|N_{33}| &= 150-8+80-(100+48-20) = 94 \\
|N_{34}| &= 135+36+64-(80-216-18) = 389 \\
M_{23} &= (3)(-1)(-102)+(2)(+1)(94)+(-7)(-1)(389) = 3217
\end{aligned}
$$

Menor $M_{25}$ (se quita la fila 2 y la columna 5):

$$
M_{25}= \begin{vmatrix}
3 & 2 & 7 & -8 \\
-1 & 5 & 2 & -9 \\
0 & 3 & 5 & 2 \\
-2 & 8 & 0 & 9
\end{vmatrix}
$$

Desarrollo por la fila 3:

$$
\begin{aligned}
|N_{32}| &= 54+126+0-(32+0-63) = 211 \\
|N_{33}| &= 135+36+64-(80-216-18) = 389 \\
|N_{34}| &= 0-8-56-(-70+48+0) = -42 \\
M_{25} &= (3)(-1)(211)+(5)(+1)(389)+(2)(-1)(-42) = 1396
\end{aligned}
$$

**Resultado:** $|A| = -5263$


#### Ejercicio 32

$$
|A|= \begin{vmatrix}
-1 & -8 & -4 & 6 & -4 \\
-1 & -8 & 1 & -10 & 9 \\
6 & -7 & 7 & 8 & 9 \\
-9 & 7 & 10 & 8 & 8 \\
-5 & 6 & 9 & 0 & 3
\end{vmatrix}
$$

**Desarrollo por la fila 5** (tiene 1 cero, quedan 4 términos):

$$
\begin{aligned}
|A| &= (-5)(-1)^{5+1}M_{51}+(6)(-1)^{5+2}M_{52}+(9)(-1)^{5+3}M_{53}+(3)(-1)^{5+5}M_{55} \\
&= (-5)(+1)(-2128)+(6)(-1)(10844)+(9)(+1)(32058)+(3)(+1)(-23722) \\
&= 162932
\end{aligned}
$$

**Cálculo de cada menor:**

Menor $M_{51}$ (se quita la fila 5 y la columna 1):

$$
M_{51}= \begin{vmatrix}
-8 & -4 & 6 & -4 \\
-8 & 1 & -10 & 9 \\
-7 & 7 & 8 & 9 \\
7 & 10 & 8 & 8
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= 64-900+504-(720+72-560) = -564 \\
|N_{12}| &= -512-630-504-(504-576+560) = -2134 \\
|N_{13}| &= -448+63-630-(441-720-56) = -680 \\
|N_{14}| &= -448+56+700-(-490-640-56) = 1494 \\
M_{51} &= (-8)(+1)(-564)+(-4)(-1)(-2134)+(6)(+1)(-680)+(-4)(-1)(1494) = -2128
\end{aligned}
$$

Menor $M_{52}$ (se quita la fila 5 y la columna 2):

$$
M_{52}= \begin{vmatrix}
-1 & -4 & 6 & -4 \\
-1 & 1 & -10 & 9 \\
6 & 7 & 8 & 9 \\
-9 & 10 & 8 & 8
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= 64-900+504-(720+72-560) = -564 \\
|N_{12}| &= -64+810+432-(-648-72-480) = 2378 \\
|N_{13}| &= -56-81+540-(-567-90+48) = 1012 \\
|N_{14}| &= -56-72-600-(630-80+48) = -1326 \\
M_{52} &= (-1)(+1)(-564)+(-4)(-1)(2378)+(6)(+1)(1012)+(-4)(-1)(-1326) = 10844
\end{aligned}
$$

Menor $M_{53}$ (se quita la fila 5 y la columna 3):

$$
M_{53}= \begin{vmatrix}
-1 & -8 & 6 & -4 \\
-1 & -8 & -10 & 9 \\
6 & -7 & 8 & 9 \\
-9 & 7 & 8 & 8
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= -512-630-504-(504-576+560) = -2134 \\
|N_{12}| &= -64+810+432-(-648-72-480) = 2378 \\
|N_{13}| &= 56+648+378-(567-63-384) = 962 \\
|N_{14}| &= 56+576-420-(-630-56-384) = 1282 \\
M_{53} &= (-1)(+1)(-2134)+(-8)(-1)(2378)+(6)(+1)(962)+(-4)(-1)(1282) = 32058
\end{aligned}
$$

Menor $M_{55}$ (se quita la fila 5 y la columna 5):

$$
M_{55}= \begin{vmatrix}
-1 & -8 & -4 & 6 \\
-1 & -8 & 1 & -10 \\
6 & -7 & 7 & 8 \\
-9 & 7 & 10 & 8
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= -448+56+700-(-490-640-56) = 1494 \\
|N_{12}| &= -56-72-600-(630-80+48) = -1326 \\
|N_{13}| &= 56+576-420-(-630-56-384) = 1282 \\
|N_{14}| &= 70+504+42-(63-49-480) = 1082 \\
M_{55} &= (-1)(+1)(1494)+(-8)(-1)(-1326)+(-4)(+1)(1282)+(6)(-1)(1082) = -23722
\end{aligned}
$$

**Resultado:** $|A| = 162932$


#### Ejercicio 33

$$
|A|= \begin{vmatrix}
10 & -10 & -2 & 4 & 4 \\
2 & 4 & 9 & 2 & 2 \\
2 & -5 & -3 & 6 & -8 \\
5 & 10 & 6 & -3 & 4 \\
1 & 8 & -4 & 2 & 3
\end{vmatrix}
$$

**Desarrollo por la fila 1** (tiene 0 ceros, quedan 5 términos):

$$
\begin{aligned}
|A| &= (10)(-1)^{1+1}M_{11}+(-10)(-1)^{1+2}M_{12}+(-2)(-1)^{1+3}M_{13}+(4)(-1)^{1+4}M_{14}+(4)(-1)^{1+5}M_{15} \\
&= (10)(+1)(3531)+(-10)(-1)(2382)+(-2)(+1)(-738)+(4)(-1)(-1089)+(4)(+1)(3465) \\
&= 78822
\end{aligned}
$$

**Cálculo de cada menor:**

Menor $M_{11}$ (se quita la fila 1 y la columna 1):

$$
M_{11}= \begin{vmatrix}
4 & 9 & 2 & 2 \\
-5 & -3 & 6 & -8 \\
10 & 6 & -3 & 4 \\
8 & -4 & 2 & 3
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= 27-96-96-(-96-24+108) = -153 \\
|N_{12}| &= 45+192-160-(192-40+180) = -255 \\
|N_{13}| &= -90-96+320-(-384+80-90) = 528 \\
|N_{14}| &= -60+72-240-(288-60-60) = -396 \\
M_{11} &= (4)(+1)(-153)+(9)(-1)(-255)+(2)(+1)(528)+(2)(-1)(-396) = 3531
\end{aligned}
$$

Menor $M_{12}$ (se quita la fila 1 y la columna 2):

$$
M_{12}= \begin{vmatrix}
2 & 9 & 2 & 2 \\
2 & -3 & 6 & -8 \\
5 & 6 & -3 & 4 \\
1 & -4 & 2 & 3
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= 27-96-96-(-96-24+108) = -153 \\
|N_{12}| &= -18+24-80-(24+16+90) = -204 \\
|N_{13}| &= 36-12+160-(-48-32-45) = 309 \\
|N_{14}| &= 24+9-120-(36+24-30) = -117 \\
M_{12} &= (2)(+1)(-153)+(9)(-1)(-204)+(2)(+1)(309)+(2)(-1)(-117) = 2382
\end{aligned}
$$

Menor $M_{13}$ (se quita la fila 1 y la columna 3):

$$
M_{13}= \begin{vmatrix}
2 & 4 & 2 & 2 \\
2 & -5 & 6 & -8 \\
5 & 10 & -3 & 4 \\
1 & 8 & 2 & 3
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= 45+192-160-(192-40+180) = -255 \\
|N_{12}| &= -18+24-80-(24+16+90) = -204 \\
|N_{13}| &= 60-20-320-(-80+64-75) = -189 \\
|N_{14}| &= 40+15+240-(60-48-50) = 333 \\
M_{13} &= (2)(+1)(-255)+(4)(-1)(-204)+(2)(+1)(-189)+(2)(-1)(333) = -738
\end{aligned}
$$

Menor $M_{14}$ (se quita la fila 1 y la columna 4):

$$
M_{14}= \begin{vmatrix}
2 & 4 & 9 & 2 \\
2 & -5 & -3 & -8 \\
5 & 10 & 6 & 4 \\
1 & 8 & -4 & 3
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= -90-96+320-(-384+80-90) = 528 \\
|N_{12}| &= 36-12+160-(-48-32-45) = 309 \\
|N_{13}| &= 60-20-320-(-80+64-75) = -189 \\
|N_{14}| &= -80-30-120-(-30+96+100) = -396 \\
M_{14} &= (2)(+1)(528)+(4)(-1)(309)+(9)(+1)(-189)+(2)(-1)(-396) = -1089
\end{aligned}
$$

Menor $M_{15}$ (se quita la fila 1 y la columna 5):

$$
M_{15}= \begin{vmatrix}
2 & 4 & 9 & 2 \\
2 & -5 & -3 & 6 \\
5 & 10 & 6 & -3 \\
1 & 8 & -4 & 2
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= -60+72-240-(288-60-60) = -396 \\
|N_{12}| &= 24+9-120-(36+24-30) = -117 \\
|N_{13}| &= 40+15+240-(60-48-50) = 333 \\
|N_{14}| &= -80-30-120-(-30+96+100) = -396 \\
M_{15} &= (2)(+1)(-396)+(4)(-1)(-117)+(9)(+1)(333)+(2)(-1)(-396) = 3465
\end{aligned}
$$

**Resultado:** $|A| = 78822$


#### Ejercicio 34

$$
|A|= \begin{vmatrix}
-5 & -9 & 10 & 8 & 0 \\
-5 & -9 & -2 & 0 & 10 \\
3 & -4 & -5 & -10 & 2 \\
1 & 8 & -6 & -4 & -6 \\
7 & -3 & 3 & -1 & -3
\end{vmatrix}
$$

**Desarrollo por la fila 1** (tiene 1 cero, quedan 4 términos):

$$
\begin{aligned}
|A| &= (-5)(-1)^{1+1}M_{11}+(-9)(-1)^{1+2}M_{12}+(10)(-1)^{1+3}M_{13}+(8)(-1)^{1+4}M_{14} \\
&= (-5)(+1)(-1942)+(-9)(-1)(1704)+(10)(+1)(198)+(8)(-1)(493) \\
&= 23082
\end{aligned}
$$

**Cálculo de cada menor:**

Menor $M_{11}$ (se quita la fila 1 y la columna 1):

$$
M_{11}= \begin{vmatrix}
-9 & -2 & 0 & 10 \\
-4 & -5 & -10 & 2 \\
8 & -6 & -4 & -6 \\
-3 & 3 & -1 & -3
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= -60+180+12-(-24-30-180) = 366 \\
|N_{12}| &= -48-180-16-(24-24+240) = -484 \\
|N_{14}| &= -24-60-240-(-180+48+40) = -232 \\
M_{11} &= (-9)(+1)(366)+(-2)(-1)(-484)+(10)(-1)(-232) = -1942
\end{aligned}
$$

Menor $M_{12}$ (se quita la fila 1 y la columna 2):

$$
M_{12}= \begin{vmatrix}
-5 & -2 & 0 & 10 \\
3 & -5 & -10 & 2 \\
1 & -6 & -4 & -6 \\
7 & 3 & -1 & -3
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= -60+180+12-(-24-30-180) = 366 \\
|N_{12}| &= 36+420-2-(-56+18+30) = 462 \\
|N_{14}| &= 18+140-30-(420-36+5) = -261 \\
M_{12} &= (-5)(+1)(366)+(-2)(-1)(462)+(10)(-1)(-261) = 1704
\end{aligned}
$$

Menor $M_{13}$ (se quita la fila 1 y la columna 3):

$$
M_{13}= \begin{vmatrix}
-5 & -9 & 0 & 10 \\
3 & -4 & -10 & 2 \\
1 & 8 & -4 & -6 \\
7 & -3 & -1 & -3
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= -48-180-16-(24-24+240) = -484 \\
|N_{12}| &= 36+420-2-(-56+18+30) = 462 \\
|N_{14}| &= -24+112+30-(-560+36+4) = 638 \\
M_{13} &= (-5)(+1)(-484)+(-9)(-1)(462)+(10)(-1)(638) = 198
\end{aligned}
$$

Menor $M_{14}$ (se quita la fila 1 y la columna 4):

$$
M_{14}= \begin{vmatrix}
-5 & -9 & -2 & 10 \\
3 & -4 & -5 & 2 \\
1 & 8 & -6 & -6 \\
7 & -3 & 3 & -3
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= -72-90+48-(36+72+120) = -342 \\
|N_{12}| &= 54+210+6-(-84-54+15) = 393 \\
|N_{13}| &= -72+168-6-(112+54+12) = -88 \\
|N_{14}| &= 72+168+15-(-280+54-12) = 493 \\
M_{14} &= (-5)(+1)(-342)+(-9)(-1)(393)+(-2)(+1)(-88)+(10)(-1)(493) = 493
\end{aligned}
$$

**Resultado:** $|A| = 23082$


#### Ejercicio 35

$$
|A|= \begin{vmatrix}
2 & 0 & -5 & -4 & 0 \\
8 & 10 & 8 & 10 & -5 \\
10 & -9 & 3 & -4 & -3 \\
-3 & 9 & 4 & -8 & 3 \\
2 & -8 & 2 & -1 & -6
\end{vmatrix}
$$

**Desarrollo por la fila 1** (tiene 2 ceros, quedan 3 términos):

$$
\begin{aligned}
|A| &= (2)(-1)^{1+1}M_{11}+(-5)(-1)^{1+3}M_{13}+(-4)(-1)^{1+4}M_{14} \\
&= (2)(+1)(4505)+(-5)(+1)(-12905)+(-4)(-1)(4900) \\
&= 93135
\end{aligned}
$$

**Cálculo de cada menor:**

Menor $M_{11}$ (se quita la fila 1 y la columna 1):

$$
M_{11}= \begin{vmatrix}
10 & 8 & 10 & -5 \\
-9 & 3 & -4 & -3 \\
9 & 4 & -8 & 3 \\
-8 & 2 & -1 & -6
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= 144-24+12-(48-9+96) = -3 \\
|N_{12}| &= -432+96+27-(-192+27+216) = -360 \\
|N_{13}| &= 216-72-54-(96-54-162) = 210 \\
|N_{14}| &= 36+192-72-(128+144-27) = -89 \\
M_{11} &= (10)(+1)(-3)+(8)(-1)(-360)+(10)(+1)(210)+(-5)(-1)(-89) = 4505
\end{aligned}
$$

Menor $M_{13}$ (se quita la fila 1 y la columna 3):

$$
M_{13}= \begin{vmatrix}
8 & 10 & 10 & -5 \\
10 & -9 & -4 & -3 \\
-3 & 9 & -8 & 3 \\
2 & -8 & -1 & -6
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= -432+96+27-(-192+27+216) = -360 \\
|N_{12}| &= 480-24-9-(48-30-72) = 501 \\
|N_{13}| &= -540-54-72-(-54-240-162) = -210 \\
|N_{14}| &= -90+144-96-(-72+640-27) = -583 \\
M_{13} &= (8)(+1)(-360)+(10)(-1)(501)+(10)(+1)(-210)+(-5)(-1)(-583) = -12905
\end{aligned}
$$

Menor $M_{14}$ (se quita la fila 1 y la columna 4):

$$
M_{14}= \begin{vmatrix}
8 & 10 & 8 & -5 \\
10 & -9 & 3 & -3 \\
-3 & 9 & 4 & 3 \\
2 & -8 & 2 & -6
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= 216-72-54-(96-54-162) = 210 \\
|N_{12}| &= -240+18+18-(-24+60+54) = -294 \\
|N_{13}| &= -540-54-72-(-54-240-162) = -210 \\
|N_{14}| &= 180-72+72-(54-320+54) = 392 \\
M_{14} &= (8)(+1)(210)+(10)(-1)(-294)+(8)(+1)(-210)+(-5)(-1)(392) = 4900
\end{aligned}
$$

**Resultado:** $|A| = 93135$


#### Ejercicio 36

$$
|A|= \begin{vmatrix}
-5 & -5 & -5 & -9 & -5 \\
-9 & 1 & -1 & -2 & -1 \\
3 & 2 & -9 & 0 & 8 \\
-9 & -8 & -2 & -4 & -3 \\
4 & 4 & 1 & 3 & 7
\end{vmatrix}
$$

**Desarrollo por la fila 3** (tiene 1 cero, quedan 4 términos):

$$
\begin{aligned}
|A| &= (3)(-1)^{3+1}M_{31}+(2)(-1)^{3+2}M_{32}+(-9)(-1)^{3+3}M_{33}+(8)(-1)^{3+5}M_{35} \\
&= (3)(+1)(-45)+(2)(-1)(9)+(-9)(+1)(-2709)+(8)(+1)(-315) \\
&= 21708
\end{aligned}
$$

**Cálculo de cada menor:**

Menor $M_{31}$ (se quita la fila 3 y la columna 1):

$$
M_{31}= \begin{vmatrix}
-5 & -5 & -9 & -5 \\
1 & -1 & -2 & -1 \\
-8 & -2 & -4 & -3 \\
4 & 1 & 3 & 7
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= 28+6+6-(4+9+28) = -1 \\
|N_{12}| &= -28+24+24-(16-9+112) = -99 \\
|N_{13}| &= -14+12+8-(8-3+56) = -55 \\
|N_{14}| &= -6+16+16-(16-4+24) = -10 \\
M_{31} &= (-5)(+1)(-1)+(-5)(-1)(-99)+(-9)(+1)(-55)+(-5)(-1)(-10) = -45
\end{aligned}
$$

Menor $M_{32}$ (se quita la fila 3 y la columna 2):

$$
M_{32}= \begin{vmatrix}
-5 & -5 & -9 & -5 \\
-9 & -1 & -2 & -1 \\
-9 & -2 & -4 & -3 \\
4 & 1 & 3 & 7
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= 28+6+6-(4+9+28) = -1 \\
|N_{12}| &= 252+24+27-(16+81+126) = 80 \\
|N_{13}| &= 126+12+9-(8+27+63) = 49 \\
|N_{14}| &= 54+16+18-(16+36+27) = 9 \\
M_{32} &= (-5)(+1)(-1)+(-5)(-1)(80)+(-9)(+1)(49)+(-5)(-1)(9) = 9
\end{aligned}
$$

Menor $M_{33}$ (se quita la fila 3 y la columna 3):

$$
M_{33}= \begin{vmatrix}
-5 & -5 & -9 & -5 \\
-9 & 1 & -2 & -1 \\
-9 & -8 & -4 & -3 \\
4 & 4 & 3 & 7
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= -28+24+24-(16-9+112) = -99 \\
|N_{12}| &= 252+24+27-(16+81+126) = 80 \\
|N_{13}| &= 504-12+36-(32+108-63) = 451 \\
|N_{14}| &= 216-16+72-(64+144-27) = 91 \\
M_{33} &= (-5)(+1)(-99)+(-5)(-1)(80)+(-9)(+1)(451)+(-5)(-1)(91) = -2709
\end{aligned}
$$

Menor $M_{35}$ (se quita la fila 3 y la columna 5):

$$
M_{35}= \begin{vmatrix}
-5 & -5 & -5 & -9 \\
-9 & 1 & -1 & -2 \\
-9 & -8 & -2 & -4 \\
4 & 4 & 1 & 3
\end{vmatrix}
$$

Desarrollo por la fila 1:

$$
\begin{aligned}
|N_{11}| &= -6+16+16-(16-4+24) = -10 \\
|N_{12}| &= 54+16+18-(16+36+27) = 9 \\
|N_{13}| &= 216-16+72-(64+144-27) = 91 \\
|N_{14}| &= 72-8+36-(32+72-9) = 5 \\
M_{35} &= (-5)(+1)(-10)+(-5)(-1)(9)+(-5)(+1)(91)+(-9)(-1)(5) = -315
\end{aligned}
$$

**Resultado:** $|A| = 21708$


---

## Resumen de determinantes

| N.º | Determinante | N.º | Determinante |
|:---:|:---:|:---:|:---:|
| 21 | $-543$ | 29 | $12060$ |
| 22 | $10$ | 30 | $-51591$ |
| 23 | $-1385$ | 31 | $-5263$ |
| 24 | $-2781$ | 32 | $162932$ |
| 25 | $1230$ | 33 | $78822$ |
| 26 | $77$ | 34 | $23082$ |
| 27 | $753$ | 35 | $93135$ |
| 28 | $984$ | 36 | $21708$ |
