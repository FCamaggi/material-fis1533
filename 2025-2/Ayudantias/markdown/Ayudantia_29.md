---
title: "Ayudantia 29"
source_enunciado: "N/A"
source_solucion: "Electro/2025-2/Ayudantias/Soluciones/Ayudantia_29_Solucion.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Ayudantia 29

## Enunciado

> *(Enunciado no disponible en el repositorio)*

---

## Solución

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Enunciado Ayudantía 29
25 de Noviembre 2025 - Profesora Macarena Domínguez
Ayudante: Luis Rivera Ly - luisriveraly@uc.cl

Corriente Alterna

1.1

Corriente Alterna - Fasores

En la respuesta de un circuito de orden mayor a cero se distinguen dos regímenes: transitorio
y permanente. Los circuitos de corriente alterna son circuitos alimentados por una fuente de
voltaje de la forma:
g(t) = A cos (wt)

(1)

Donde A es la amplitud de la señal y w su frecuencia angular.
Luego, la respuesta forzada (i.e en régimen permanente) será:

xp (t) = Ap cos (wt + ϕ)

(2)

Donde ϕ es su fase.

Con ello, es posible representar la señal mediante un fasor, o sea, un número complejo en
coordenadas polares:
 
p
b
z = a + jb = a + b ∠ arctan
(3)
a
√

Donde A ≡ a2 + b2 y ϕ ≡ arctan ab es la magnitud y fase de la señal, respectivamente.
También, se puede reescribir la fase mediante una exponencial compleja:

z = Aejθ

(4)

Utilizando la fórmula de Moivre:

ejθ = cos (θ) + j sin (θ)
Puede ser importante conocer algunas de las operatorias fasoriales:

A1 ∠ϕ1 · A2 ∠ϕ2 = A1 A1 ∠ϕ1 + ϕ2
A1 ∠ϕ1
A1
=
∠ϕ1 − ϕ2
A2 ∠ϕ2
A2

(5)

---

### Página 2

1.2

Corriente Alterna - Fasores

Gracias al dominio en frecuencia, es posible generalizar el concepto de resistencia y definir la
impedancia de resistencias, capacitores e inductores:
ZR = R
ZC =
jwC
ZR = jwL

(6)
(7)
(8)

De esta manera, podemos decir que:

Z = R + jX
Y =
= G + jB
Z

(9)
(10)

Donde Y es la admitancia, X la reactancia, G la conductancia y B la susceptancia.
Además, si X > 0 estamos en presencia de un inductor, mientras que si X < 0 de un capacitor.

1.3

Corriente Alterna - Potencia

La potencia instantánea de un circuito con una fuente de voltaje V (t) que entrega una corriente
I(t) está dada por:
P (t) = V (t)I(t)

(11)

Sin embargo, es más útil conocer la potencia media durante todo un período:

⟨P (t)⟩ =

T

Z T
P (t) dt

(12)

Mediante fasores, la potencia promedio puede ser determinar en forma equivalente como:

⟨P (t)⟩ = V I ∗

(13)

Donde I ∗ es el conjugado de la corriente. A partir de lo anterior,
y utilizando valores cuadráticos medios, podemos decir que:

⟨P (t)⟩ = Vrms Irms cos (ϕ)

(14)

---

### Página 3

1.3.1

“Problemas Resueltos de Electromagnetismo”, 16.11, Rodrigo Chi

Considere el siguiente circuito eléctrico en régimen estacionario:
a) Determine la impedancia de entrada vista por la fuente de voltaje.
b) Si la señal de entrada viene dada por v(t) = 4 cos(2π4 + π/6) V en RMS, encuentre
el fasor de corriente equivalente del circuito e Ix .

Figura 1. Esquema Circuito.

---

### Página 4

1.3.2

“Problemas Resueltos de Circuitos”, 17.5

Considere el siguiente circuito eléctrico en régimen estacionario:

Figura 2. Esquema Circuito.
Donde Iin = 1.076∠ − 8.3◦ es la corriente que sale de la fuente de voltaje y su magnitud
está en valor RMS.
a) Determine la potencia compleja alimentada por la fuente de voltaje, la cual no
está en valor RMS.
b) Si la potencia compleja recibida por Z1 es 6.945 + j13.89 VA, determine los valores
de R1 y L1 .
c) Si la potencia compleja recibida por Z3 es 4.63 + j6.85 VA, determine los valores
de R2 y C2 .
Posterior a esto, se le pide que modifique el circuito anterior para asegurar que la
impedancia de entrada sea igual a 30 Ω para una señal DC (w = 0). Además, se
pide que la impedancia de entrada sea igual a 100 Ω para entradas de muy alta
frecuencia (w → ∞). Usted propone el siguiente esquemático:

Figura 3. Esquema Circuito.
d) Determine los valores de R4 y R5 que4cumplen lo pedido.
