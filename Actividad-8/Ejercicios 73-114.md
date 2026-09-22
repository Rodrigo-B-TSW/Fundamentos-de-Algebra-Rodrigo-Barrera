# Actividad #8. Sistemas de numeración

| DATOS | |
| :--- | :--- |
| **Alumno** | Rodrigo Barrera García |
| **Profesor** | Jorge Javier Pedroza Romero |
| **Materia** | Fundamentos de Álgebra |
| **Fecha** | 22/09/2026 |

---
## Binario a Decimal

**73.** `00001111₂`

| 2⁷ | 2⁶ | 2⁵ | 2⁴ | 2³ | 2² | 2¹ | 2⁰ |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| 0 | 0 | 0 | 0 | 1 | 1 | 1 | 1 |

Suma → 8 + 4 + 2 + 1 = **15**

> **00001111₂ = 15₁₀**

---

**74.** `10011001₂`

| 2⁷ | 2⁶ | 2⁵ | 2⁴ | 2³ | 2² | 2¹ | 2⁰ |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| 1 | 0 | 0 | 1 | 1 | 0 | 0 | 1 |

Suma → 128 + 16 + 8 + 1 = **153**

> **10011001₂ = 153₁₀**

---

**75.** `11001100₂`

| 2⁷ | 2⁶ | 2⁵ | 2⁴ | 2³ | 2² | 2¹ | 2⁰ |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| 1 | 1 | 0 | 0 | 1 | 1 | 0 | 0 |

Suma → 128 + 64 + 8 + 4 = **204**

> **11001100₂ = 204₁₀**

---

**76.** `01111011₂`

| 2⁷ | 2⁶ | 2⁵ | 2⁴ | 2³ | 2² | 2¹ | 2⁰ |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| 0 | 1 | 1 | 1 | 1 | 0 | 1 | 1 |

Suma → 64 + 32 + 16 + 8 + 2 + 1 = **123**

> **01111011₂ = 123₁₀**

---

**77.** `00000000 11111111₂`

| 2⁷ | 2⁶ | 2⁵ | 2⁴ | 2³ | 2² | 2¹ | 2⁰ |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 |

(El primer byte es `00000000`, no aporta valor)

Suma → 128 + 64 + 32 + 16 + 8 + 4 + 2 + 1 = **255**

> **00000000 11111111₂ = 255₁₀**

---

**78.** `10 00000000₂`

Solo el bit en la posición 9 está activo:

1 × 2⁹ = **512**

> **10 00000000₂ = 512₁₀**

---

## Binario a Octal

Se agrupa el binario en bloques de **3 bits** (de derecha a izquierda) y se convierte cada bloque a su valor octal (0–7).

**79.** `11010101₂`

Agrupado: `011 | 010 | 101`

| Grupo | Cálculo | Valor |
|:--:|:--:|:--:|
| 011 | 0+2+1 | 3 |
| 010 | 0+2+0 | 2 |
| 101 | 4+0+1 | 5 |

> **11010101₂ = 325₈**

---

**80.** `01101110₂`

Agrupado: `001 | 101 | 110`

| Grupo | Cálculo | Valor |
|:--:|:--:|:--:|
| 001 | 0+0+1 | 1 |
| 101 | 4+0+1 | 5 |
| 110 | 4+2+0 | 6 |

> **01101110₂ = 156₈**

---

**81.** `10110011₂`

Agrupado (con relleno de 0 a la izquierda): `010 | 110 | 011`

| Grupo | Cálculo | Valor |
|:--:|:--:|:--:|
| 010 | 0+2+0 | 2 |
| 110 | 4+2+0 | 6 |
| 011 | 0+2+1 | 3 |

> **10110011₂ = 263₈**

---

**82.** `11111111₂`

Agrupado (con relleno): `011 | 111 | 111`

| Grupo | Cálculo | Valor |
|:--:|:--:|:--:|
| 011 | 0+2+1 | 3 |
| 111 | 4+2+1 | 7 |
| 111 | 4+2+1 | 7 |

> **11111111₂ = 377₈**

---

**83.** `00000011 11000000₂`

Agrupado (bits significativos): `001 | 111 | 000 | 000`

| Grupo | Cálculo | Valor |
|:--:|:--:|:--:|
| 001 | 0+0+1 | 1 |
| 111 | 4+2+1 | 7 |
| 000 | 0+0+0 | 0 |
| 000 | 0+0+0 | 0 |

> **00000011 11000000₂ = 1700₈**

---

**84.** `00000101 01010101₂`

Agrupado (bits significativos): `010 | 101 | 010 | 101`

| Grupo | Cálculo | Valor |
|:--:|:--:|:--:|
| 010 | 0+2+0 | 2 |
| 101 | 4+0+1 | 5 |
| 010 | 0+2+0 | 2 |
| 101 | 4+0+1 | 5 |

> **00000101 01010101₂ = 2525₈**

---

## Binario a Hexadecimal

Se agrupa el binario en **nibbles de 4 bits** y se convierte cada uno a su valor hexadecimal (0–9, A–F).

**85.** `11011010₂`

Agrupado: `1101 | 1010`

| Nibble | Cálculo | Valor |
|:--:|:--:|:--:|
| 1101 | 8+4+0+1 = 13 | D |
| 1010 | 8+0+2+0 = 10 | A |

> **11011010₂ = DA₁₆**

---

**86.** `01111100₂`

Agrupado: `0111 | 1100`

| Nibble | Cálculo | Valor |
|:--:|:--:|:--:|
| 0111 | 0+4+2+1 = 7 | 7 |
| 1100 | 8+4+0+0 = 12 | C |

> **01111100₂ = 7C₁₆**

---

**87.** `10110101₂`

Agrupado: `1011 | 0101`

| Nibble | Cálculo | Valor |
|:--:|:--:|:--:|
| 1011 | 8+0+2+1 = 11 | B |
| 0101 | 0+4+0+1 = 5 | 5 |

> **10110101₂ = B5₁₆**

---

**88.** `11110000 10100101₂`

Agrupado: `1111 | 0000 | 1010 | 0101`

| Nibble | Cálculo | Valor |
|:--:|:--:|:--:|
| 1111 | 8+4+2+1 = 15 | F |
| 0000 | 0 | 0 |
| 1010 | 8+0+2+0 = 10 | A |
| 0101 | 0+4+0+1 = 5 | 5 |

> **11110000 10100101₂ = F0A5₁₆**

---

**89.** `00001111 00001111₂`

Agrupado: `0000 | 1111 | 0000 | 1111`

| Nibble | Cálculo | Valor |
|:--:|:--:|:--:|
| 0000 | 0 | 0 |
| 1111 | 8+4+2+1 = 15 | F |
| 0000 | 0 | 0 |
| 1111 | 8+4+2+1 = 15 | F |

> **00001111 00001111₂ = 0F0F₁₆ (F0F₁₆)**

---

**90.** `10000000 00000001₂`

Agrupado: `1000 | 0000 | 0000 | 0001`

| Nibble | Cálculo | Valor |
|:--:|:--:|:--:|
| 1000 | 8 | 8 |
| 0000 | 0 | 0 |
| 0000 | 0 | 0 |
| 0001 | 1 | 1 |

> **10000000 00000001₂ = 8001₁₆**

---

## Octal a Binario

Cada dígito octal se convierte a su equivalente binario de **3 bits**.

**91.** `325₈`

| Dígito | Binario (3 bits) |
|:--:|:--:|
| 3 | 011 |
| 2 | 010 |
| 5 | 101 |

> **325₈ = 11010101₂**

---

**92.** `156₈`

| Dígito | Binario (3 bits) |
|:--:|:--:|
| 1 | 001 |
| 5 | 101 |
| 6 | 110 |

> **156₈ = 01101110₂**

---

**93.** `377₈`

| Dígito | Binario (3 bits) |
|:--:|:--:|
| 3 | 011 |
| 7 | 111 |
| 7 | 111 |

> **377₈ = 11111111₂**

---

**94.** `01777₈`

| Dígito | Binario (3 bits) |
|:--:|:--:|
| 0 | 000 |
| 1 | 001 |
| 7 | 111 |
| 7 | 111 |
| 7 | 111 |

> **01777₈ = 1111111111₂**

---

**95.** `03700₈`

| Dígito | Binario (3 bits) |
|:--:|:--:|
| 0 | 000 |
| 3 | 011 |
| 7 | 111 |
| 0 | 000 |
| 0 | 000 |

> **03700₈ = 11111000000₂**

---

**96.** `05255₈`

| Dígito | Binario (3 bits) |
|:--:|:--:|
| 0 | 000 |
| 5 | 101 |
| 2 | 010 |
| 5 | 101 |
| 5 | 101 |

> **05255₈ = 101010101101₂**

---

## Hexadecimal a Binario

Cada dígito hexadecimal se convierte primero a decimal y luego a su equivalente binario de **4 bits**.

**97.** `DA₁₆`

| Dígito | Decimal | Binario (4 bits) |
|:--:|:--:|:--:|
| D | 13 | 1101 |
| A | 10 | 1010 |

> **DA₁₆ = 11011010₂**

---

**98.** `7C₁₆`

| Dígito | Decimal | Binario (4 bits) |
|:--:|:--:|:--:|
| 7 | 7 | 0111 |
| C | 12 | 1100 |

> **7C₁₆ = 01111100₂**

---

**99.** `B5₁₆`

| Dígito | Decimal | Binario (4 bits) |
|:--:|:--:|:--:|
| B | 11 | 1011 |
| 5 | 5 | 0101 |

> **B5₁₆ = 10110101₂**

---

**100.** `F0A5₁₆`

| Dígito | Decimal | Binario (4 bits) |
|:--:|:--:|:--:|
| F | 15 | 1111 |
| 0 | 0 | 0000 |
| A | 10 | 1010 |
| 5 | 5 | 0101 |

> **F0A5₁₆ = 1111000010100101₂**

---

**101.** `0F0F₁₆`

| Dígito | Decimal | Binario (4 bits) |
|:--:|:--:|:--:|
| 0 | 0 | 0000 |
| F | 15 | 1111 |
| 0 | 0 | 0000 |
| F | 15 | 1111 |

> **0F0F₁₆ = 0000111100001111₂**

---

**102.** `8001₁₆`

| Dígito | Decimal | Binario (4 bits) |
|:--:|:--:|:--:|
| 8 | 8 | 1000 |
| 0 | 0 | 0000 |
| 0 | 0 | 0000 |
| 1 | 1 | 0001 |

> **8001₁₆ = 1000000000000001₂**

---

## Nombres de Polinomios por su Exponente Más Alto

| # | Polinomio | Grado | Nombre | ¿Por qué? |
|:--:|:--|:--:|:--|:--|
| 103 | 5n + 5 | 1 | Binomio lineal | El mayor exponente es n¹ |
| 104 | -10p³ - 6 + 9p² - 4p⁵ - 2p⁸ | 8 | Polinomio de 8vo grado | El mayor exponente es p⁸ |
| 105 | 7x⁸ | 8 | Monomio de 8vo grado | El único término tiene exponente x⁸ |
| 106 | -2n + n⁴ + 10n⁶ | 6 | Trinomio de 6to grado | El mayor exponente es n⁶ |
| 107 | 5 | 0 | Monomio de grado cero (término constante) | No tiene variable, el exponente implícito es 0 |
| 108 | 5v⁷ | 7 | Monomio de 7mo grado | El único término tiene exponente v⁷ |

---

## Problemas Prácticos

**109.** Amy llena la entrada de concreto en 8 h. Junto con Jill, tardan 3.08 h. ¿Cuánto tardaría Jill sola?

Planteamiento (razones de trabajo):

$$\frac{1}{8} + \frac{1}{t} = \frac{1}{3.08}$$

$$\frac{1}{t} = \frac{1}{3.08} - \frac{1}{8} = 0.3247 - 0.125 = 0.1997$$

$$t = \frac{1}{0.1997}$$

> **Jill tardaría sola ≈ 5 horas**

---

**110.** Jaidee cava el hoyo en 5 h, Ted en 7 h. ¿Cuánto tardarían juntos?

$$\frac{1}{5} + \frac{1}{7} = \frac{7}{35} + \frac{5}{35} = \frac{12}{35}$$

$$t = \frac{35}{12} \approx 2.92 \text{ h}$$

> **Juntos tardarían ≈ 2.92 horas (2 h 55 min)**

---

**111.** El avión de carga sale primero; 4 h después sale el de la Fuerza Aérea a 310 km/h y lo alcanza tras volar 6 h. ¿Velocidad promedio del avión de carga?

Cuando lo alcanza, el avión de carga ya lleva volando: 4 h + 6 h = **10 h**

Distancia recorrida por el de la Fuerza Aérea (= distancia del avión de carga):

$$d = 310 \text{ km/h} \times 6 \text{ h} = 1860 \text{ km}$$

Velocidad del avión de carga:

$$v = \frac{1860 \text{ km}}{10 \text{ h}}$$

> **Velocidad promedio del avión de carga = 186 km/h**

---

**112.** Tren de carga: ida a 35 km/h, regreso a 49 km/h. El regreso tomó 10 h. ¿Cuánto tomó la ida? (misma distancia ambos tramos)

Distancia (usando el regreso):

$$d = 49 \text{ km/h} \times 10 \text{ h} = 490 \text{ km}$$

Tiempo de ida:

$$t = \frac{490 \text{ km}}{35 \text{ km/h}}$$

> **El viaje de ida tomó 14 horas**

---

**113.** 1 yd³ de tierra con 30% de arena se mezcla con 4 yd³ con 20% de arena. ¿% de arena en la mezcla?

Arena total:

$$(1)(0.30) + (4)(0.20) = 0.30 + 0.80 = 1.10 \text{ yd}^3$$

Volumen total = 1 + 4 = 5 yd³

Porcentaje:

$$\frac{1.10}{5} = 0.22$$

> **La mezcla contiene 22% de arena**

---

**114.** James mezcla 7 L de ponche Marca A (11% jugo) con 6 L de Marca B (24% jugo). ¿Qué % de la mezcla es jugo de fruta?

Jugo total:

$$(7)(0.11) + (6)(0.24) = 0.77 + 1.44 = 2.21 \text{ L}$$

Volumen total = 7 + 6 = 13 L

Porcentaje:

$$\frac{2.21}{13} = 0.17$$

> **La mezcla contiene 17% de jugo de fruta**
