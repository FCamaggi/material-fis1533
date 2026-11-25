---
title: "Mini Control Formativo   Ley de Gauss"
source_enunciado: "Electro/2025-2/Ayudantias/Mini_Controles_Formativos/Enunciados/Enunciado_Mini_Control_Formativo___Ley_de_Gauss.pdf"
source_solucion: "Electro/2025-2/Ayudantias/Mini_Controles_Formativos/Soluciones/Solución_Mini_Control_Formativo___Ley_de_Gauss.pdf"
extraction_mode: "pdftotext_cleaned"
---

# Mini Control Formativo   Ley de Gauss

## Enunciado

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Solución Mini Control Formativo
Ley de Gauss
2° Semestre 2025 - Cuerpo de Ayudantes FIS1533
Ayudante Coordinador: Luis Rivera Ly - luisriveraly@uc.cl

“I1 2022-2”, Problema 5, Facultad de Física
En la figura se aprecia una esfera maciza de radio R de densidad de carga uniforme ρ0 ,
encerrada por un cascarón esférico concéntrico a ella, de radio 2R, con grosor de pared
despreciable y densidad superficial de carga uniforme σ desconocida. Determine el valor
0R
de σ, de manera que el campo eléctrico neto en el punto P de la figura sea ke πρ
r̂.

Figura 1. Esquema sobre el cascarón y la esfera.
a) −ρ120 R
b) −ρ180 R
c) −ρ300 R
d) −ρ360 R
e) Ninguna de las anteriores

---

### Página 2

“I1 2015-1”, Problema 5, Facultad de Física
La figura muestra las líneas de campo producidas por tres cargas de magnitud +1C,
+1C y −1C (aunque no necesariamente en este orden). La superficie gaussiana en la
figura es una esfera que contiene dos de las cargas. ¿Qué se puede decir acerca del flujo
eléctrico a través de esta superficie?

Figura 2. Esquema sobre las cargas.
a) Es − 2C
ε0
b) Es 2C
ε0
c) Es 0
d) Dependerá de la distancia a la que se encuentre las cargas que están adentro
e) Dependerá de la distancia a la que se encuentre la carga que está afuera

---

## Solución

### Página 1

Pontificia Universidad Católica de Chile
Facultad de Física
FIS1533 - Electricidad y Magnetismo

Solución Mini Control Formativo
Ley de Gauss
2° Semestre 2025 - Cuerpo de Ayudantes FIS1533
Ayudante Coordinador: Luis Rivera Ly - luisriveraly@uc.cl

“I1 2022-2”, Problema 5, Facultad de Física
En la figura se aprecia una esfera maciza de radio R de densidad de carga uniforme ρ0 ,
encerrada por un cascarón esférico concéntrico a ella, de radio 2R, con grosor de pared
despreciable y densidad superficial de carga uniforme σ desconocida. Determine el valor
0R
de σ, de manera que el campo eléctrico neto en el punto P de la figura sea ke πρ
r̂.

Figura 1. Esquema sobre el cascarón y la esfera.
a) −ρ120 R
b) −ρ180 R
c) −ρ300 R
d) −ρ360 R
e) Ninguna de las anteriores

---

### Página 2

#### Solución
Paso 0: ¿Cómo plantear el ejercicio?
Se pide determinar el valor de σ de manera que el campo eléctrico cumpla la condición dada en
el punto P . Como se está hablando de una esfera, es posible aplicar Ley de Gauss utilizando
una esfera concéntrica de radio = r” arbitrario:
I
Qenc
E · ds =
ε0
S
No se entrega explícitamente la carga contenida en la esfera y el cascarón,
por lo que se tendrá que utilizar la definición de carga:

ZZ
Q=
σ dS
S
ZZZ
Q=
ρ dV
V

Además, y como se presentan = cortes visuales” relacionados con un cambio
en la densidad de carga, se debe trabajar por intervalos: r < R, R < r < 2R y r > 2R.

Paso 1: Ley de Gauss - Er>2R
Como el punto a evaluar se encuentra en la región r > 2R, solo se calculará el campo eléctrico
para la configuración en tal región mediante Ley de Gauss:
I
Qenc
Er>2R · ds =
ε0
Como es una esfera, el campo solo poseerá componente radial.
Además, la carga encerrada estará determinada por una integral doble y triple en esféricas:

RRR

I
Er>2R ·

V ρ dV +

dS =

RR

S σ dS

ε0

Como la densidad de carga de la esfera y del cascarón son uniformes,
se pueden tratar como constantes y salen de la integral.
Ahora, la integral cerrada es en verdad la superficie de la esfera
gaussiana, pues el flujo es ortogonal a esta en todo momento:

Er>2R · 4πr =

ρ0 ·

RRR

V dV + σ ·

RR

S dS

ε0

Las integrales de superficie y volumen se refieren a la superficie y volumen
encerrados por la esfera gaussiana de radio = r”. En este caso, sería toda la
superficie y volumen del cascarón y esfera con carga, respectivamente:

ρ0 · 4πR
3 + σ · 4π(2R)
ε0
R
ρ0 R
Er>2R =
·(
+ 4σ)
ε0 r

Er>2R · 4πr2 =

---

### Página 3

Finalmente, y como el campo eléctrico es un vector, se aplica la componente radial:

Er>2R =

R2
ρ0 R
·(
+ 4σ) r̂
ε0 r

(1)

Evalúando el campo en el punto r = 4R:

Er>2R =

ρ0 R
·(
+ 4σ) r̂
16ε0

(2)

Paso 2: Condición Campo - σ
Luego, se impone la condición para el campo en el punto r = 4R dado por enunciado:
Er>2R =

ρ0 R
ke πρ0 R
+ 4σ) r̂ =
·(
r̂
16ε0

Como la componente vectorial es única y equivalente en la ecuación vectorial, se puede
), se obtiene que:
obviar en el análisis. Reescribiendo la constante de Coulomb (i.e ke = 4πε

ρ0 R
1 πρ0 R
·(
+ 4σ) =
16ε0
4πε0 18
ρ0 R
2ρ0 R
+ 4σ =
−ρ0 R
σ=

(3)

---

### Página 4

“I1 2015-1”, Problema 5, Facultad de Física
La figura muestra las líneas de campo producidas por tres cargas de magnitud +1C,
+1C y −1C (aunque no necesariamente en este orden). La superficie gaussiana en la
figura es una esfera que contiene dos de las cargas. ¿Qué se puede decir acerca del flujo
eléctrico a través de esta superficie?

Figura 2. Esquema sobre las cargas.
a) Es − 2C
ε0
b) Es 2C
ε0
c) Es 0
d) Dependerá de la distancia a la que se encuentre las cargas que están adentro
e) Dependerá de la distancia a la que se encuentre la carga que está afuera

#### Solución
Paso Único: Flujo Eléctrico - Φe
Se pide determinar el flujo eléctrico que atraviesa la superficie de la figura:
Z
Φe =
E · ds
S

Como la superficie es una esfera gaussiana, se puede decir que:

I
E · ds =

Φe =
S

Qenc
ε0

La esfera encierra dos de las cargas. Recordando la disposición de las líneas
de campo para cargas puntuales, se concluye de que son una carga positiva
y una carga negativa. Reemplazando por los valores entregados por enunciado:

Φe =

Qenc
+1C − 1C
=
=0
ε0
ε0
